> [!NOTE]
> **This whole project is done via vibe-coding, expect [Exmaples Demo](#-Examples) and this message**

# PhreakCrypt

Welcome to **PhreakCrypt**, a powerful all-in-one Python tool for cryptographic operations with a hacking edge. It supports encryption, decryption, encoding, decoding, hashing, obfuscation, and vector-based encryption for AI embeddings, making it ideal for cybersecurity enthusiasts, developers, and AI practitioners. Whether you're securing sensitive data or protecting AI embeddings for similarity searches, PhreakCrypt has you covered with a sleek, hacker-inspired interface.

## Installation

1. Ensure you have Python 3.7 or later installed.
2. Install the required dependencies using pip:


```bash
git clone --depth 1 https://github.com/mr0erek/PhreakCrypt.git; cd PhreakCrypt; python -m venv venv; pip3 install -r requirements.txt
```

> [!Note]
> For Homomorphic Encryption (HE), you need to install PySEAL separately from Microsoft SEAL, as it requires C++ dependencies and is not included by default.
##
# Usage  
**PhreakCrypt** uses a command-line interface powered by `argparse`. Run commands in the format:


```bash
python3 pheakcrypt.py <operation> --algorithm <algorithm> --data <data> [options]

```
### Available operations includes :
> encrypt, decrypt, encode, decode, hash, obfuscate, deobfuscate, encrypt_vector, and decrypt_vector. Options vary by operation, such as --algorithm, --encoding, --shift, --key, and --data.
##

# Examples:

### 1. Symmetric Encryption (AES)
```bash
python3 phreakcrypt.py encrypt --algorithm aes --data "Hello, World!"
```
> **Output**
> `Encrypted: gAAAAABm... (base64-encoded string)
Key: b'X9f...==' (Fernet key)`
##
### 2. Decryption (AES) Decrypt AES-encrypted data using the provided key.

```bash
python3 phreakcrypt.py decrypt --algorithm aes --key "X9f...==" --data "gAAAAABm..."
```
> **Output**
>  `Decrypted: Hello, World!`
##
### 3. Encoding (Base64) Encode text to Base64.
```bash
python3 phreakcrypt.py encode --encoding base64 --data "Hello, World!"
```
> **Output**
> -> Encoded: SGVsbG8sIFdvcmxkIQ==
##
### 4. Hashing (SHA-256)
```bash
python3 phreakcrypt.py hash --algorithm sha256 --data "Hello, World!"
```
> **Output**
> -> Hashed: dffd6021bb2bd5b0af676290809ec3a53191dd81c7f70a4b28688a362182986f
##
### 5. Deobfuscation (Caesar Cipher)
Deobfuscate Caesar cipher text with a shift of 3.

```bash 
python3 phreakcrypt.py obfuscate --shift 3 --data "Hello, World!"
```
> **Output**
> -> Deobfuscated: Hello, World!

##

### 6. Vector Encryption (Property-Preserving Encryption - PPE) Encrypt a vector (e.g., AI embedding) using simulated PPE, preserving relative distances.

```bash 
python3 phreakcrypt.py decrypt_vector --algorithm ale --key "X9f...==" --data "gAAAAABm..."
```
#### Sooner will update with more examples
