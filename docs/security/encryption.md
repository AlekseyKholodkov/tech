# 🔐 Encryption Process

## What is Encryption?

**Encryption** is the process of transforming readable data (**plaintext**) into an unreadable format (**ciphertext**) to protect it from unauthorized access. Only those with the correct **key** can decrypt the data and recover the original plaintext.

---

## 🛠️ How Encryption Works

### 1. Plaintext Input
This is the original data you want to protect—e.g., a message, file, or password.

### 2. Encryption Algorithm
An algorithm (e.g., AES, RSA) processes the plaintext using an **encryption key** to convert it into ciphertext.

- **Symmetric encryption**: The same key is used for both encryption and decryption (e.g., AES).
- **Asymmetric encryption**: Uses a **public key** for encryption and a **private key** for decryption (e.g., RSA, ECC).

### 3. Ciphertext Output
The result is scrambled data that appears meaningless without the correct key.

### 4. Decryption
The reverse process. The encrypted data is turned back into plaintext using the appropriate decryption key.

---

## 🔑 Example: Symmetric Encryption (AES)

```plaintext
Plaintext:  "Hello, World!"
Key:        "secretkey123"
↓ Encryption (AES)
Ciphertext: "6a9f8f3e9a2f..."
↓ Decryption (AES with same key)
Plaintext:  "Hello, World!"
```

## 🧱 Common Encryption Algorithms

| Type         | Algorithm | Description                                | Common Use Cases                             |
|--------------|-----------|--------------------------------------------|----------------------------------------------|
| Symmetric    | AES       | Fast, secure encryption standard            | File encryption, databases, disk encryption  |
| Symmetric    | ChaCha20  | Stream cipher, faster on some hardware      | VPNs, mobile encryption                      |
| Asymmetric   | RSA       | Public-private key encryption               | Secure email, digital signatures, key exchange |
| Asymmetric   | ECC       | Efficient alternative to RSA with smaller keys | IoT devices, mobile apps, TLS                |
| Hybrid       | TLS       | Combines symmetric & asymmetric encryption  | HTTPS, secure web traffic                    |
| Hybrid       | mTLS      | TLS with mutual authentication using certificates | Secure service-to-service communication, APIs, microservices |


