# 📄 Installing Substrate Cargo Contract Node (v0.38.0)

This guide explains how to download, install, and run the **Substrate Cargo Contract Node** on Ubuntu (or WSL on Windows). This node is required for testing and deploying version 5 smart contracts built with [ink!](https://use.ink).

---

## 🛠 Prerequisites

* **Ubuntu** or **WSL2 on Windows** installed.
* `wget` and `tar` available (install them if missing):

  ```bash
  sudo apt update && sudo apt install wget tar -y
  ```

---

## 🚀 Installation Steps

### 1. Download the specific node version

We only specify `v0.38.0` as this version uses `pallet-contracts`:

```bash
wget https://github.com/paritytech/substrate-contracts-node/releases/download/v0.38.0/substrate-contracts-node-linux.tar.gz
```

---

### 2. Extract the tarball

Unpack the downloaded file:

```bash
tar -xzf substrate-contracts-node-linux.tar.gz
```

---

### 3. Locate the directory

```bash
cd artifacts/substrate-contracts-node-linux
```

---

### 3. Make the binary executable

```bash
chmod +x substrate-contracts-node
```

---

### 5. Verify the installation

Check the installed version:

```bash
./substrate-contracts-node --version
```

---

### 6. Run the node

Start the node in development mode:

```bash
./substrate-contracts-node
```

*(Use `--help` to view available options)*
