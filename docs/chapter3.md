# Chapter 3: Asymmetric Encryption

## What is Asymmetric Encryption?
Asymmetric encryption uses a pair of keys:
- **Public Key** – Used for encryption.
- **Private Key** – Used for decryption.

## Common Algorithms
- **RSA (Rivest-Shamir-Adleman)** – A widely used public-key algorithm.
- **ECC (Elliptic Curve Cryptography)** – Provides strong security with smaller key sizes.
- **Diffie-Hellman** – A method for secure key exchange.

## Example of RSA Encryption
```python
from Crypto.PublicKey import RSA
from Crypto.Cipher import PKCS1_OAEP

key = RSA.generate(2048)
cipher = PKCS1_OAEP.new(key.publickey())
ciphertext = cipher.encrypt(b"Secret Message")
```

## Use Cases
- **Secure communications (SSL/TLS)**
- **Digital signatures**
- **Cryptocurrency transactions**
