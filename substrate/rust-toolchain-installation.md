# 🦀 Installing and Configuring Rust 1.89 for ink!

This guide covers setting up **Rust v1.89** for building and running version 5 ink! smart contracts.

---

## 🛠 Prerequisites

* **Ubuntu** or [**WSL2 on Windows**](https://github.com/villenaj/docs/blob/main/substrate/setup-wsl-rust.md) installed.
* [Rustup](https://rustup.rs/) already installed.

---

## 🚀 Installation Steps

### 1. Update Rustup

Ensure you have the latest rustup version:

```bash
rustup update
```

### 2. Install Rust v1.89

Install the specific Rust toolchain version:

```bash
rustup install 1.89
```

### 3. Set Rust v1.89 as Default

Make this version the default globally:

```bash
rustup default 1.89
```

### 4. Add Rust Source Component

Add the Rust source for this version:

```bash
rustup component add rust-src --toolchain 1.89
```

### 5. Add WebAssembly Target

Add the WebAssembly target for building ink! contracts:

```bash
rustup target add wasm32-unknown-unknown --toolchain 1.89
```

### 6. Add Rust Source for Specific Architecture (Optional)

For Linux x86\_64:

```bash
rustup component add rust-src --toolchain 1.89-x86_64-unknown-linux-gnu
```

---

## ✅ Verification

Check that the correct version is active:

```bash
rustup show
```

The output should confirm Rust **1.89.x** is in use.
```
Default host: x86_64-unknown-linux-gnu
rustup home:  /home/user/.rustup

installed toolchains
--------------------
stable-x86_64-unknown-linux-gnu
1.89-x86_64-unknown-linux-gnu (active, default)

active toolchain
----------------
name: 1.89-x86_64-unknown-linux-gnu
active because: it's the default toolchain
installed targets:
  wasm32-unknown-unknown
  x86_64-unknown-linux-gnu
```
