# Chapter 4: Hash Functions and Digital Signatures

## What is a Hash Function?
A hash function takes an input and produces a fixed-length output, called a hash. It is used for data integrity and authentication.

## Common Hash Functions
- **SHA-256 (Secure Hash Algorithm 256-bit)** – Used in Bitcoin and secure authentication.
- **MD5 (Message Digest Algorithm 5)** – Fast but insecure due to vulnerabilities.
- **SHA-3** – The latest standard in secure hashing.

## Example of SHA-256 Hashing
```python
import hashlib

message = b"Hello, World!"
hash_object = hashlib.sha256(message)
print(hash_object.hexdigest())
```

## Digital Signatures
Digital signatures use asymmetric encryption to verify the authenticity of messages.
- **Signing** – The sender encrypts a hash with their private key.
- **Verification** – The receiver decrypts the hash using the sender’s public key.

## Use Cases
- **Document verification**
- **Software authenticity**
- **Blockchain transactions**
