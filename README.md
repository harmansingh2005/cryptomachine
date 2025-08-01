# 🔐 CryptoMachine

**CryptoMachine** is a simple yet effective file encryption and decryption GUI tool built with Python and Tkinter. It allows you to securely encrypt any file using AES encryption with a user-defined secret key, and decrypt it later using the same key.

---

## Features

- AES-256 encryption using password-derived keys
- GUI-based interface with `tkinter`
- Encrypt **any file** on your computer
- Decrypt using the same secret key
- Real-time progress feedback
- Cancel encryption/decryption mid-process
- Simple, beginner-friendly, and open-source

---

## Download

[![Download CryptoMachine](https://img.shields.io/badge/Download-EXE-blue?style=for-the-badge&logo=windows)](https://github.com/harmansingh2005/downloadcryptomachine)

> If you prefer to run the source code directly, follow the installation guide below.

## 🛠️ Installation (CLI)

> Python 3.6+ required

1. **Clone the repository:**

```bash
gh repo clone harmansingh2005/downloadcryptomachine

```
2. **Install dependencies**
```bash
pip install pycryptodome
```
3. **Run the app**
```bash
python CryptoMachine.py
```

---

## How To Use?
- Open the app and click SELECT FILE to pick the file you want to encrypt or decrypt.
- Enter a Secret Key. (Remember it! You’ll need it to decrypt.)
- Click ENCRYPT to encrypt the selected file. A .kryp file will be created.
- To decrypt, select a .kryp file, enter the original secret key, and click DECRYPT.
- Click RESET to clear all input fields.
- Click CANCEL anytime during processing to abort.
    - 📝 Encrypted files will look like: myphoto.jpg.kryp
    - 📝 Decrypted files will be saved as: myphoto__dekrypted__.jpg

---

## Security Notes

- Uses AES in CFB mode (no padding required).
- Secret key and salt are hashed with SHA256 to derive strong 256-bit and 128-bit keys.
- The secret key is never stored or transmitted — decryption is only possible if the correct key is provided.
- If the secret key is lost, there is no recovery for encrypted files.
  
---

## Future Improvements

- Add drag-and-drop file support
- Mask password field input
- Support batch file encryption
- Show estimated time remaining
- Portable .exe/.app builds for all platforms
- Add command-line interface (CLI) mode
  
  
   
