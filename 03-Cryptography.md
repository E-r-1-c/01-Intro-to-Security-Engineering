# Introduction to Cryptography

Cryptography is the practice of protecting information so that only the intended recipients can understand it. It ensures confidentiality, integrity, and authenticity.

---

## Symmetric Encryption
- **Single key** used for both encryption and decryption.  
- Requires a secure channel to share the key.  
- **Advantages**: Fast and efficient.  
- **Disadvantages**: Key distribution problem — if key is stolen, all communication is compromised.  
- **Common Algorithms**: AES, DES, 3DES, IDEA, Blowfish, Twofish, Camellia.  
- **Operation Types**:
  - **Block Cipher**: Encrypts data in fixed-size blocks.  
  - **Stream Cipher**: Encrypts data one byte at a time.

---

## Asymmetric Encryption
- **Public key** for encryption, **private key** for decryption.  
- Eliminates key distribution problem.  
- **Use Cases**: Secure messaging, digital signatures, key exchange.  
- **Common Algorithms**: RSA, ECC.  
- **Applications**:
  - **Confidentiality**: Encrypt with recipient’s public key.  
  - **Integrity & Authenticity**: Sign with private key, verify with public key.  

---

## Diffie-Hellman Key Exchange
- Allows two parties to agree on a shared secret over an insecure channel.  
- Steps:
  1. Agree on public numbers (prime q and generator g).  
  2. Each chooses a private number (a, b).  
  3. Exchange coded numbers derived from private values.  
  4. Both compute the shared secret key independently.  
- Vulnerable to **Man-in-the-Middle attacks** if identity is not verified.

---

## Hashing
- Converts data of any size into a fixed-length string called a **hash** or **message digest**.  
- **Properties**:
  - One-way: cannot easily reverse.  
  - Sensitive to changes: small modification changes the hash.  
- **Uses**: Password storage, data integrity verification.  
- **Common Algorithms**: SHA-256, SHA-512, SHA-384, SHA-1, MD5 (deprecated).  
- **HMAC**: Hash-based Message Authentication Code — uses a secret key with a hash to verify authenticity and integrity.

---

## PKI and SSL/TLS
- **Public Key Infrastructure (PKI)**: System of digital certificates, certificate authorities (CAs), and trust relationships.  
- **Purpose**: Ensure identity of entities, secure communication.  
- **SSL/TLS Handshak**
