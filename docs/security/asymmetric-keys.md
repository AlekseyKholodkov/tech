# 🔑 Public and Private Keys in Asymmetric Encryption

## What Is Asymmetric Encryption?

**Asymmetric encryption** (or **public-key cryptography**) uses a pair of mathematically related keys:

- A **public key** that can be freely shared
- A **private key** that must be kept secret

These keys are used together to **encrypt and decrypt data** or to **digitally sign and verify messages**.

---

## 🔐 How It Works

### 1. Encryption & Decryption

| Action         | Key Used        | Who Performs It             |
|----------------|------------------|-----------------------------|
| Encrypt data   | **Public key**   | Anyone                      |
| Decrypt data   | **Private key**  | Owner of the private key    |

**Example:**
- Alice wants to send Bob a confidential message.
- She encrypts it with **Bob’s public key**.
- Only **Bob’s private key** can decrypt it — ensuring **confidentiality**.

---

### 2. Digital Signatures

| Action          | Key Used        | Who Performs It             |
|-----------------|------------------|-----------------------------|
| Sign message    | **Private key**  | Sender                      |
| Verify signature| **Public key**   | Receiver / anyone           |

**Example:**
- Bob signs a document using his **private key**.
- Anyone with **Bob’s public key** can verify the signature — ensuring **authenticity** and **integrity**.

---

## 🧠 Why It's Secure

- The **private key** is never shared.
- It’s mathematically infeasible to reverse-engineer the private key from the public key.
- This makes it safe to communicate securely over untrusted networks.

---

## 🔁 Summary Table

| Use Case                | Public Key Used For        | Private Key Used For        |
|-------------------------|----------------------------|------------------------------|
| Confidential Messaging  | Encrypting data            | Decrypting data              |
| Authentication / Signing| Verifying signature        | Creating digital signature   |

---

## 🔒 Real-World Applications

- **TLS/HTTPS**: Secure communication on the internet
- **SSH**: Secure access to servers
- **PGP/GPG**: Secure email and file encryption
- **JWT Signing**: Verifying identity in APIs

