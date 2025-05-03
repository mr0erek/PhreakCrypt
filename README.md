# PhreakCrypt

Welcome to **PhreakCrypt**, a powerful all-in-one Python tool for cryptographic operations with a hacking edge. It supports encryption, decryption, encoding, decoding, hashing, obfuscation, and vector-based encryption for AI embeddings, making it ideal for cybersecurity enthusiasts, developers, and AI practitioners. Whether you're securing sensitive data or protecting AI embeddings for similarity searches, CyberCrypt has you covered with a sleek, hacker-inspired interface.

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
python crypto_tool.py encrypt --algorithm aes --data "Hello, World!"
```
