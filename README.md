# 🔐 VaultMate

**VaultMate** is a local-first password manager with a built-in password strength analyzer. It encourages better password hygiene by evaluating password entropy, reuse, and exposure (using HaveIBeenPwned APIs). VaultMate runs securely offline with optional cloud sync encryption using user-provided keys, ensuring that your sensitive data remains under your control.

VaultMate is designed to provide a simple, secure, and offline-first solution for managing passwords while giving you insights into the strength and safety of your credentials.

## 📌 Features

- 🔒 **Local-First Password Management**:
  - Passwords are stored securely on your local device, ensuring that your data is never exposed to third parties
  - Optional cloud synchronization with end-to-end encryption using user-provided keys for an added layer of security
  - Supports complex passwords, PINs, and even 2FA tokens for a comprehensive solution

- 🧠 **Password Strength Analyzer**:
  - Built-in password strength checker that evaluates entropy and overall complexity
  - Provides recommendations to improve weak passwords (e.g., increasing length, adding special characters)
  - Highlights weak, reused, and commonly used passwords to improve password hygiene

- 🔐 **Exposure Check (HaveIBeenPwned)**:
  - Automatically checks your passwords against the **HaveIBeenPwned** database for known data breaches
  - Notifies users if any passwords are exposed in previous breaches, recommending immediate password changes

- 🔄 **Cloud Sync with Encryption**:
  - Optional secure cloud synchronization to back up your password vault across multiple devices
  - Fully encrypted using user-provided keys, ensuring that only you have access to your data
  - Data never leaves your control, minimizing the risk of cloud-based data breaches

- 🚀 **Offline-First Operation**:
  - Fully functional without an internet connection, ensuring that you always have access to your passwords
  - Encryption and storage occur locally, making it a privacy-focused solution for password management
  - Internet access only required for optional cloud sync or HaveIBeenPwned checks

- 🧑‍💻 **Cross-Platform Support**:
  - Available for multiple platforms, including macOS, Windows, and Linux
  - Simple, clean user interface for easy management and access to your passwords

- 🔑 **Two-Factor Authentication (2FA) Support**:
  - Store and manage 2FA tokens for supported services directly within VaultMate
  - Automatically fill in 2FA codes when logging into services that require it

## 🛠️ Tech Stack

- **Frontend**: Electron.js (cross-platform desktop app)
- **Backend**: Node.js (local encryption and database management)
- **Encryption**: AES-256, RSA, Argon2 (for password hashing)
- **Cloud Sync**: Custom encryption using user-provided keys (AES)
- **APIs**: HaveIBeenPwned API (for breach checks)
- **Storage**: SQLite (local password storage)

## 🚀 Getting Started

### Prerequisites

- Node.js 14+
- Git
- Local desktop environment (Windows, macOS, Linux)

### Installation & Usage

1. Clone the repository:

```bash
git clone https://github.com/your-username/vaultmate.git
cd vaultmate
