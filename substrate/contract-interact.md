# Interacting with a Smart Contract in PolkadotJS Portal

This guide starts from the point where your contract is already uploaded and instantiated. It covers only how to interact with it.

---

## Interact with the deployed contract

Once your contract appears in the list under **Developer → Contracts**, you can perform two kinds of calls:

* **Read** messages (do not alter chain state, free, no signature).
* **Execute** messages (alter chain state, require signing & fees).

### Calling a `read` message (query)

1. Open the contract instance in **Developer → Contracts**.

   ![alt text](https://github.com/user-attachments/assets/622d15d5-8955-4792-937d-29d8de827b3b "Uploaded contract")

3. Under **Messages**, locate a message marked as `read`.
  
5. Select one of the `read` message.

   ![alt text](https://github.com/user-attachments/assets/aa8cf89c-4498-409d-a6f6-b62759938a14 "Query function")

6. Click **Read** to run it. The returned value displays below the button.

   ![alt text](https://github.com/user-attachments/assets/b740007c-0655-4189-9dae-587da44f9596 "Read the function")


### Calling an `execute` (transaction)

1. Select a message marked as `exec`.
  
3. Click **Execute** to proceed the contract call.

   ![alt text](https://github.com/user-attachments/assets/85681837-9882-4b2c-8320-764d81d82e05 "Execute a contract")

4. Click **Sign and Submit** to sign the transaction.

   ![alt text](https://github.com/user-attachments/assets/886d9cf4-9b1f-4686-8ba6-a0bbd7e38e0e "Sign and submit")

5. Enter your extension wallet password and click **Sign the transaction**.

   ![alt text](https://github.com/user-attachments/assets/b0e74a99-7894-4c41-b6cc-0550382c2db8 "Sign the transaction")

6. Once transaction is valid and done, you'll see the success message.

   ![alt text](https://github.com/user-attachments/assets/9cd7f2fd-66bf-4860-9a81-2f94c78ed55c "Successful notification")

7. You can check again the data if it mutated by calling `read` function again.

    ![alt text](https://github.com/user-attachments/assets/32bada15-b322-4cb6-bbc3-250f936319f9 "Query again")


---

## Tips

* **Gas limit**: Always start with Portal’s suggested limit.
* **Events**: After each transaction, check emitted events to see execution results.
* **Storage**: Use read-only messages (getters) to inspect contract state.
