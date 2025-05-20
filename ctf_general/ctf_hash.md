***MD5*** (Message-Digest Algorithm 5) is a widely used cryptographic hash function that produces a 128-bit (16-byte) hash value, typically represented as a 32-character hexadecimal number.

Key points about MD5:
Input: any length of data (message)

Output: fixed-length 128-bit hash (32 hex chars)

Commonly used to verify data integrity (e.g., checksums)

Considered cryptographically broken and unsuitable for security because of vulnerabilities to collision attacks

***SHA-1*** (Secure Hash Algorithm 1)
Output size: 160 bits (20 bytes), usually shown as a 40-character hexadecimal string.

Designed by: NSA, published in 1995.

Purpose: Originally designed as a cryptographic hash function to ensure data integrity and digital signatures.

Algorithm type: Iterative hash function based on the Merkle–Damgård construction.

Security:

Now considered cryptographically weak due to discovered collision vulnerabilities (two different inputs producing the same hash).

Collisions have been practically demonstrated, so SHA-1 should not be used for security-sensitive applications.

Use cases:

Older systems still use it for checksums or legacy compatibility, but modern systems avoid SHA-1.

***SHA-256*** (Secure Hash Algorithm 256-bit)
Output size: 256 bits (32 bytes), usually shown as a 64-character hexadecimal string.

Part of: SHA-2 family of hash functions (which includes SHA-224, SHA-256, SHA-384, SHA-512, etc.)

Designed by: NSA, published in 2001.

Purpose: A stronger cryptographic hash function designed to replace SHA-1.

Security:

Currently considered secure and collision-resistant (no practical collisions found).

Used widely in cryptography, blockchain, TLS certificates, and digital signatures.

Use cases:

Secure password hashing (often combined with salt and key stretching), digital signatures, integrity verification, blockchain hashes (e.g., Bitcoin), SSL/TLS certificates.


***hash generator***:
https://md5calc.com/hash/sha256#google_vignette

