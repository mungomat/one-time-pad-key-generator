# One-Time Pad Key Generator

This project contains a [self-contained HTML tool (index.html)](https://mungomat.github.io/one-time-pad-key-generator) that securely splits a secret (like a master password or a private key) into two parts based on the one-time pad principle. The security of the system relies on storing the two generated keys in physically separate locations.

The entire tool is self-contained in a single HTML file and is designed for offline use to ensure maximum security.

## Features

- Secure Splitting: Uses the information-theoretically secure XOR operation to split a secret into a random key and an encrypted key.
- Robust Verification: Each key contains multiple hashes to verify its own integrity, that of its counterpart, and the pair's association. An automatic self-test after generation ensures that every key pair is valid.
- PDF Generation: Creates a printable PDF document for each key, including the key string, a scannable QR code, and optional custom notes.
- Bilingual: The user interface can be switched between German and English.
- Flexible Input: Supports secrets as text (UTF-8) or as a hexadecimal string.

## Offline Usage

This tool is intended for offline use. To use it securely, follow these steps:
- Download the one_time_pad_key_generator.html file.
- Disconnect your computer from the internet.
- Open the downloaded HTML file in any modern web browser (e.g., Firefox, Chrome, Edge).

All necessary scripts are either embedded directly or are cached by the browser after the first load, meaning no internet connection is required for operation.

## ⚠️ Disclaimer

This is a demonstration project for a cryptographic concept. It has not been audited by independent security experts. The cryptographic implementation and the protocol could contain flaws.

Use is exclusively at your own risk. Never store critical data using only this tool without being aware of the risks or having additional backups.
