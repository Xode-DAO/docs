# 🐧 Set Up Windows Subsystem for Linux (WSL) and Install Rust

This guide walks you through enabling **Windows Subsystem for Linux (WSL)** on Windows, installing Ubuntu, and setting up Rust for development.

---

## 🖥 Check Your Windows Version

* If you have **Windows 10, version 2004 (Build 19041 or higher)** or **Windows 11**, WSL is available by default.
* For **older versions** of Windows, follow the [WSL manual installation steps](https://learn.microsoft.com/en-us/windows/wsl/install-manual) for older builds.
* If your computer has **Windows 10, version 1903 or higher**, you can download and install **WSL 2**.

---

## ⚙ Enable WSL

1. Open **Windows PowerShell** or **Command Prompt** from the Start menu.
2. Right-click and select **Run as administrator**.
3. In the terminal, run:

   ```bash
   wsl --install
   ```

---

## 🌐 Install a Specific Linux Distribution (Optional)

* To view available distributions:

  ```bash
  wsl --list --online
  ```
* To install Ubuntu 24.04:

  ```bash
  wsl --install Ubuntu-24.04
  ```

---

## 👤 Create Your UNIX User Account

* Enter a **UNIX username** when prompted.
* Set and confirm a **password** for your UNIX user.
* Restart your computer when installation is complete.

---

## 📦 Install Required Packages and Rust

1. **Open PowerShell** as Administrator.

2. From the Start menu, launch the installed **Ubuntu** distribution.

3. Update Ubuntu packages:

   ```bash
   sudo apt update
   ```

   Enter your UNIX user password when prompted.

4. Install required packages:

   ```bash
   sudo apt install --assume-yes git clang curl libssl-dev llvm libudev-dev make protobuf-compiler
   ```

5. Download and run the Rust installation script:

   ```bash
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```

   Follow the prompts for a default installation.

6. Update your shell environment:

   ```bash
   source ~/.cargo/env
   ```

7. Verify Rust installation:

   ```bash
   rustc --version
   ```

---

## 📚 Additional Resources

* [WSL Documentation](https://learn.microsoft.com/en-us/windows/wsl/)
* [Rust Installation Guide](https://www.rust-lang.org/tools/install)
