# 📦 Installing Cargo-Contract v3.2.0 and Creating a Smart Contract

This guide explains how to install **cargo-contract v3.2.0** and create, test, and build a smart contract.

---

## 🛠 Prerequisites

* [Rust](https://www.rust-lang.org/tools/install) (v1.89 or compatible)
* `rustup` configured with WebAssembly target `wasm32-unknown-unknown`
* Ubuntu or WSL2 environment

---

## 🚀 Install Cargo-Contract v3.2.0

Use the following command to install or upgrade cargo-contract:

```bash
cargo install --force --locked cargo-contract --tag v3.2.0 --git https://github.com/use-ink/cargo-contract
```

> The `--force` flag reinstalls even if it’s already installed. The `--locked` flag ensures dependency lockfiles are respected.

---

## 📝 Create a New Smart Contract

Generate a new project:

```bash
cargo contract new <project-name>
```

Replace `<project-name>` with your desired contract name.

---

## 📂 Navigate to the Project

Move into your project directory:

```bash
cd <project-name>
```

---

## ✅ Run Tests

Run the included unit tests:

```bash
cargo test
```

---

## 🏗 Build the Contract

Build the smart contract in debug mode:

```bash
cargo contract build
```

Or build in release mode for optimized output:

```bash
cargo contract build --release
```

---

## 📚 Additional Resources

* [Cargo-Contract v3.2.0 Release Notes](https://github.com/use-ink/cargo-contract/releases/tag/v5.0.3)
