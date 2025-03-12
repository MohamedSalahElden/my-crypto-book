# Chapter 2: Symmetric Encryption

## What is Symmetric Encryption?
Symmetric encryption uses a single key to encrypt and decrypt data. It is fast and efficient but requires secure key exchange mechanisms.

## Common Algorithms
- **AES (Advanced Encryption Standard)** – A widely used block cipher.
- **DES (Data Encryption Standard)** – Older, now considered insecure.
- **Blowfish** – A strong alternative to DES with variable-length keys.

## Example of AES Encryption
```python
from Crypto.Cipher import AES
import os

key = os.urandom(16)  # Generate a random 16-byte key
cipher = AES.new(key, AES.MODE_EAX)
ciphertext, tag = cipher.encrypt_and_digest(b"Secret Message")
```

## Advantages and Disadvantages
✅ Fast and efficient for large data volumes.  
❌ Key distribution can be challenging.