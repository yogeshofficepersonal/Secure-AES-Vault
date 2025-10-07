# Secure AES Vault: Client-Side Document Encryptor


# 🛡️ Project Overview
The Secure AES Vault is a robust, single-file, web-based tool designed for private, end-to-end file encryption and decryption. Utilizing the powerful Advanced Encryption Standard (AES) via the CryptoJS library, this application ensures maximum privacy by performing all cryptographic operations directly in the user's browser, meaning no files or secret keys ever leave the client machine.

# 🎯 Main Objective
The primary goal of the Secure AES Vault is to empower users with a simple, accessible, and secure method for protecting sensitive documents before sharing them. It functions as a secure utility for generating encrypted files (.enc) that can be safely transmitted over insecure channels, relying on a separately shared secret key for decryption.

# ✨ Key Features
Client-Side Security (Zero-Knowledge): All file processing and AES encryption/decryption take place locally in the browser. There is no backend server or database involved in handling the sensitive document data or the secret key.

AES-256 Encryption: Uses industry-standard AES with passphrase-based key derivation (handled automatically by CryptoJS), providing a high level of cryptographic security.

Universal File Support: Encrypts any file type (documents, images, videos, etc.) by converting the file content into a Base64 Data URL before encryption, preserving file integrity upon decryption.

Simple Sharing Format: Encrypted files are saved with the .enc extension, making them easy to identify and share.

Intuitive User Interface: A clear, modern, and unique design (built with Tailwind CSS) separates the encryption and decryption workflows for ease of use.

Password Visibility Toggle: Includes an integrated eye icon to help users accurately enter and confirm their secret keys.

# 🚀 How to Use (Local Setup)
Since this is a single HTML file with no backend dependencies, deployment is incredibly simple:

# Clone the Repository:

git clone [https://github.com/YourUsername/secure-aes-vault.git](https://github.com/YourUsername/secure-aes-vault.git)

Open the File: Locate the document_encrypter.html file and open it directly in any modern web browser (e.g., Chrome, Firefox, Edge).

# Encryption Process
Select File: Under the "Encrypt Document" section, choose the file you wish to protect.

Set Key: Enter a strong, unique secret password (this is your AES key).

Encrypt: Click the Encrypt & Download .enc File button. The browser will automatically download the encrypted file.

Share Securely: Manually send the .enc file to the recipient. Crucially, share the secret key/password separately via a trusted, secure channel (e.g., a verbal communication, a private, end-to-end encrypted chat app).

# Decryption Process
Select Encrypted File: Under the "Decrypt Document" section, choose the .enc file you received.

Enter Key: Input the exact secret password provided by the sender.

Decrypt: Click the Decrypt & Download Original File button. The original file will be restored and downloaded to your computer.

# ⚠️ Security and Key Management Disclaimer
This project provides the mechanism for strong encryption, but the overall security of the shared document relies entirely on key management:

Key Strength: Always use a long, complex, and unique password for your encryption key.

Key Sharing: The secret key must be shared with the recipient securely, outside of this application's file transfer. If the key is compromised, the document is compromised.

Encryption Standard: The AES implementation uses standard and well-vetted cryptographic practices via the popular CryptoJS library, but it is not a substitute for professional, audited security software.
