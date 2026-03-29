# PDF Encryptor

A simple web-based tool that lets you password-protect your PDF files entirely in the browser. No files are uploaded to any server — everything runs locally on your machine, keeping your documents 100% private.

## How It Works

1. **Choose a PDF** — Drag and drop a PDF file onto the drop zone, or click to browse and select one from your computer.
2. **Set a Password** — Enter a password (minimum 6 characters). A strength indicator shows how strong your password is in real time. Confirm the password to make sure there are no typos.
3. **Encrypt & Download** — Click the "Encrypt & Download" button. The app encrypts the PDF using the [pdf-lib](https://pdf-lib.js.org/) library right in your browser, then automatically downloads the encrypted file with `_encrypted` appended to the original filename.

## Features

- **Fully client-side** — No server, no uploads. Your files never leave your device.
- **Drag & drop** support for easy file selection.
- **Password strength meter** — Visual feedback on password strength (weak, fair, strong).
- **Input validation** — Checks for file selection, minimum password length, and password confirmation match before encrypting.
- **Instant download** — The encrypted PDF is downloaded automatically after processing.

## Tech Stack

- **HTML / CSS / JavaScript** — Pure frontend, no frameworks.
- **pdf-lib** — JavaScript library used to read and encrypt PDF documents in the browser.

## Usage

Just open `index.html` in any modern browser — no build step or server required.

## Project Structure

```
pdf-encryptor/
├── index.html    # Main HTML page with the 3-step form
├── style.css     # Styling for the UI
├── script.js     # Application logic + bundled pdf-lib library
└── README.md     # This file
```
