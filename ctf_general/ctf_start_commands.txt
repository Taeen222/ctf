Before applying any command 
do these:


1)binwalk

2)exiftool 

3)cat 

4)metadata

5)file 

6)grep :

Commonly Used grep Options
Option	Description
-i	Case-insensitive search: Match pattern regardless of case.
-v	Invert match: Show lines that do not match the pattern.
-r or -R	Recursive search: Search directories and their subdirectories.
-l	Show file names only: Display filenames with matches, not the matching lines.
-n	Show line numbers: Display the line number in the file where the pattern is found.
-c	Count matches: Show the number of matching lines instead of the matching lines themselves.
-w	Whole word search: Match the whole word, not partial matches (e.g., cat will match "cat" but not "catalog").
-o	Show only matching part: Display only the matched parts of the line, rather than the entire line.
-A NUM	After context: Show NUM lines after the match.
-B NUM	Before context: Show NUM lines before the match.
-C NUM	Context: Show NUM lines before and after the match (same as -A and -B combined).
-e	Multiple patterns: Use this option to search for multiple patterns.
-f	Pattern file: Read patterns from a file.
-q	Quiet mode: Suppress all output; just return the exit status. Useful for scripts.
-s	Suppress error messages: Suppresses error messages about nonexistent or unreadable files.
-H	Always print file name: Print the file name even when searching a single file or when output is from stdin.
-h	Suppress file name: Suppress the file name in output (useful when searching multiple files).
-P	Perl-compatible regex: Use Perl-compatible regular expressions (PCRE) for pattern matching.
-E	Extended regular expressions: Enable extended regular expressions (like +, ?, `
-F	Fixed strings: Interpret the pattern as a literal string, not a regular expression (faster).
-x	Exact match: Only print lines that match the pattern exactly (whole line).
-Y	Match only at the start of the line: Equivalent to using ^ in the regular expression.
--color	Highlight matches: Show matched strings in color (usually red).
--binary-files=TYPE	Handle binary files: Specifies how binary files should be handled (e.g., binary, text, or without-match).


