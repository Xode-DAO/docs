# 📤 Uploading Smart Contract to Polkadot-JS Portal

This guide explains how to upload and deploy a compiled ink! smart contract to **Polkadot-JS Portal** using the **XODE Testnet**.

---

## 💰 Fund Your Wallet via Faucet

1. Create or import an account in [**Polkadot-JS Extension**](https://polkadot.js.org/extension).
2. Copy your wallet address.
3. Visit the [XODE Faucet](https://node.xode.net/faucet).
4. Select **Paseo** ecosystem and **XON** token.
5. Click **Submit** to request test tokens for your wallet address.

---

## 🌐 Connect to XODE Testnet Node

1. Open [Polkadot-JS Apps](https://polkadot.js.org/apps/#/explorer?rpc=wss://paseo-rpcnode.xode.net).
2. Click the network in the upper-right of the page.

   ![alt text](https://github.com/user-attachments/assets/27a8234f-d9f2-47b5-baf2-5862e3b613e5 "Choose network")
   
3. Dropdown to **TEST PASEO & PARACHAINS**.

   ![alt text](https://github.com/user-attachments/assets/8840005a-8fa3-45f8-8810-f20089f3df16 "Select Paseo network")
   
4. Scroll down and click **Xode** testnet parachain.

   ![alt text](https://github.com/user-attachments/assets/31d6d5ac-722b-458a-9e56-d6d27c2d8dcd "Xode Testnet")

5. Scroll to the top and click **Switch**

   ![alt text](https://github.com/user-attachments/assets/b6912510-02cb-45b8-9fa0-69305749793c "Switch network")

6. Ensure the connection is set to the XODE testnet node (`wss://paseo-rpcnode.xode.net`).

   ![alt text](https://github.com/user-attachments/assets/851e32c3-b6f0-4307-90a8-deac61252416 "Xode websocket")

8. Confirm that the requested tokens are visible in [**Accounts**](https://polkadot.js.org/apps/?rpc=wss://paseo-rpcnode.xode.net#/accounts) under your selected account.

---

## 📑 Upload and Deploy the Contract

1. Navigate to **Developer > Contracts**.
2. Click **Upload & deploy code**.
3. Choose the funded account for deployment.
4. Upload your compiled contract file. You can locate it in your Windows File Explorer using your installed Ubuntu distribution version dynamically. The path format is:

   ```bash
   \\wsl.localhost\<your-ubuntu-version>\home\<unix-username>\<contract-name>\target\ink
   ```

   Replace `<your-ubuntu-version>` with your actual WSL distribution name (e.g., `Ubuntu`, `Ubuntu-22.04`  or `Ubuntu-24.04`).
   The file to upload is:

   ```bash
   <contract-name>.contract
   ```

   ![alt text](https://github.com/user-attachments/assets/41cc69c0-0f73-4637-ab6b-f169da97a547 "Upload smart contract")
5. Configure any necessary deployment parameters and **Submit**.
   ![alt text](https://github.com/user-attachments/assets/c82694a5-f82d-4306-b2f4-71de185f9092 "Sign and submit")
6. Approve the transaction in the Polkadot-JS wallet popup and wait for confirmation.
  ![alt text](https://github.com/user-attachments/assets/689a0174-db9b-4d2d-bf52-b55778b86eeb "Sign transaction")
7. Ensure that the transaction was successful.
   ![alt text](https://github.com/user-attachments/assets/c0866b1a-8e4b-4be7-8f72-b2a8966bfb31 "Transaction success")

---

## ▶ Execute the Contract

* After uploading the contract, navigate back to **Developer > Contracts**.
* You can now **execute its methods** directly from this section.
  ![alt text](https://github.com/user-attachments/assets/c7d60836-92ae-4e65-a789-16ec1a2df2a8 "Sign and submit")

---

## 📚 Notes

* Ensure your wallet is funded from the faucet before deploying.
* Always sign transactions using your Polkadot-JS wallet when prompted.
* Use sufficient funds in your selected account for gas and storage fees.
* For detailed documentation, visit [Polkadot-JS Apps](https://polkadot.js.org/apps/).
