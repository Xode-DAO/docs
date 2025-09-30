# 📤 Uploading Smart Contract to Polkadot-JS Portal

This guide explains how to upload and deploy a compiled smart contract to **Polkadot-JS Portal** using your local node.

---

## 🌐 Connect to Your Local Node

1. Open [Polkadot-JS Apps](https://polkadot.js.org/apps/#/explorer?rpc=ws://localhost:9944).
2. Ensure the connection is set to your local node (`ws://localhost:9944`).

---

## 📑 Upload and Deploy the Contract

1. Navigate to **Developer > Contracts**.
2. Click **Upload & deploy code**.
3. Choose the account you will use for deployment.
4. Upload your compiled contract file:

   ```
   <projectname>.contract
   ```
   ![alt text](https://github.com/user-attachments/assets/52f94976-4cdc-4cbb-8e3a-c22492b04dc0 "Upload smart contract")
5. Configure any necessary deployment parameters and **Submit**.
   ![alt text](https://github.com/user-attachments/assets/39e2292c-3868-4251-93ab-d916f8b7a9b2 "Sign and submit")
6. Make sure that the transaction is success.
   ![alt text](https://github.com/user-attachments/assets/21afac2c-cba3-4fcd-b157-c7c906631db6 "Sign and submit")

---

## ▶ Execute the Contract

* After uploading the contract, you can now **execute its methods** directly from the **Developer > Contracts** section in Polkadot-JS UI.
  ![alt text](https://github.com/user-attachments/assets/3bd33214-8d3c-4611-b015-9da0fab9cd92 "Sign and submit")

---

## 📚 Notes

* Ensure your node is running and synced before uploading.
* Use sufficient funds in your selected account for gas and storage fees.
* For detailed documentation, visit [Polkadot-JS Apps](https://polkadot.js.org/apps/).
