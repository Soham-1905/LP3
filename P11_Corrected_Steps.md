# Practical 11: Create a MetaMask Wallet and Transfer Sepolia Test ETH

## Steps to Perform the Practical

### Step 1: Install MetaMask

1. Open the official MetaMask download page: https://metamask.io/download/.
2. Select **Chrome**.
3. The Chrome Web Store will open. Click **Add to Chrome**.
4. Select **Add extension** when prompted.
5. Open MetaMask from the browser extensions menu. You can pin the extension to the toolbar for easy access.

**Important:** Install MetaMask only from its official website or the official browser extension store. Do not install an extension from an unknown website.

### Step 2: Create a New Wallet

1. Open the MetaMask extension.
2. Select **Create a new wallet**.
3. Follow the setup prompts. MetaMask may offer setup using a **Secret Recovery Phrase** or a supported social sign-in option such as Google.
4. If you choose the Secret Recovery Phrase option, write the 12-word phrase down in the correct order and store it securely offline.
5. Complete the confirmation steps shown by MetaMask.
6. Set a strong wallet password if prompted.

**Security note:** Never share your Secret Recovery Phrase or private key with anyone. Do not enter the phrase on a website or send it in a message. Anyone who has the phrase can control the wallet. If you choose social sign-in, keep the linked account and MetaMask password secure.

### Step 3: Copy Your Wallet Address

1. Open MetaMask.
2. Select the account you want to use.
3. Click the account name or address to copy the public wallet address.

Example format:

```text
0x1234...ABCD
```

This is the **public Ethereum address**. It is safe to share when someone needs to send test ETH to you. Do not confuse it with your private key or Secret Recovery Phrase.

### Step 4: Enable and Select the Sepolia Test Network

1. Open MetaMask.
2. Open the menu and select **Networks**.
3. Find and enable **Show test networks**.
4. Open the network selector and choose **Sepolia**.
5. Confirm that Sepolia is selected before requesting or sending test ETH.

### Step 5: Get Sepolia Test ETH

1. Open MetaMask’s official guide to the Sepolia faucet: https://support.metamask.io/develop/blockchain-networks/testnets/using-the-testnet-faucet/. Follow its current link to the MetaMask Developer Sepolia faucet.
2. Connect your MetaMask wallet. The MetaMask faucet guide states that the connected account may need to be linked to a MetaMask Developer Dashboard account.
3. Check that the displayed address is the account you intend to fund.
4. Click **Request ETH** and complete the prompts, if the faucet is available to you.
5. If that faucet is unavailable, use a Sepolia faucet listed on Ethereum’s official network page: https://ethereum.org/developers/docs/networks/.
6. Check your MetaMask balance or the Sepolia block explorer to confirm that the test ETH arrived.

**Important:** Sepolia ETH is test currency. It has no real-world monetary value and is used only for testing transactions and applications. Keep some test ETH available to pay the network fee for the transfer.

### Step 6: Create a Second Account

1. In MetaMask, open the account selector.
2. Select **Add account** (or **Add account or hardware wallet**, depending on the interface).
3. Choose the option to create a new account and complete the prompts.
4. Select the new account and copy its public address.

For this practical:

```text
Account 1 → Sender
Account 2 → Receiver
```

Both accounts should use the **Sepolia** network. A second account inside MetaMask is sufficient; it does not require installing another wallet.

### Step 7: Send Test ETH

1. Select **Account 1** in MetaMask.
2. Confirm that the selected network is **Sepolia**.
3. Click **Send**.
4. Paste the public address of **Account 2** as the recipient.
5. Enter a small amount of test ETH, for example:

```text
0.001 ETH
```

6. Click **Continue** or **Next**.
7. Carefully review the recipient address, amount, selected network, and estimated network fee.
8. If the details are correct, click **Confirm**.

Do not confirm the transaction if the recipient address or network is incorrect. The sender must have enough Sepolia ETH for both the amount being sent and the network fee.

### Step 8: Find the Transaction Hash

1. After confirming, open the **Activity** section in MetaMask.
2. Find the transfer you just made.
3. Open the transaction details.
4. Copy the **Transaction Hash** (also called the transaction ID).

A transaction hash is a unique identifier for the transaction. The transaction may show as pending before it is confirmed.

### Step 9: Verify the Transaction on the Sepolia Block Explorer

1. Open the Sepolia Etherscan block explorer: https://sepolia.etherscan.io/.
2. Paste the transaction hash into the search bar.
3. Open the matching transaction.
4. Check the transaction details, including:

```text
Transaction Hash
From
To
Value
Transaction Fee
Block
Status
Timestamp
```

Confirm that the transaction status is **Success**. If it is pending, wait for confirmation and check again.

### Step 10: Verify the Receiver Balance

1. Return to MetaMask.
2. Select **Account 2**.
3. Make sure the **Sepolia** network is selected.
4. Check that the received test ETH is reflected in the account balance.

The practical flow is:

```text
Install MetaMask
        ↓
Create a New Wallet
        ↓
Copy the Public Wallet Address
        ↓
Enable and Select Sepolia Testnet
        ↓
Get Sepolia Test ETH from a Faucet
        ↓
Create a Second Account
        ↓
Copy the Receiver Address
        ↓
Send Test ETH from Account 1 to Account 2
        ↓
Confirm the Transaction
        ↓
Copy the Transaction Hash
        ↓
Verify the Transaction on Sepolia Etherscan
        ↓
Check the Receiver Balance
```

## What to Show in Your Practical Record

Take screenshots of the following:

1. MetaMask extension installed and wallet dashboard open.
2. Wallet/account created (show only the public account address; do not show recovery information).
3. Sepolia network selected.
4. Sepolia test ETH balance.
5. Sender account (Account 1).
6. Send transaction screen with the receiver's public address and amount.
7. Transaction confirmation or transaction details.
8. Transaction hash.
9. Transaction details on Sepolia Etherscan showing **Success**.
10. Receiver account (Account 2) showing the received test ETH.

**Never include your Secret Recovery Phrase, private key, or password in screenshots or in your practical record.**

## Result

**Result:** A MetaMask wallet was created and configured on the Sepolia Ethereum test network. Sepolia test ETH was obtained from a faucet and transferred from Account 1 to Account 2. The transaction was verified using its transaction hash on the Sepolia block explorer.

## Official References

- MetaMask download: https://metamask.io/download/
- MetaMask wallet setup: https://support.metamask.io/start/creating-a-new-wallet/
- Show test networks in MetaMask: https://support.metamask.io/configure/networks/how-to-view-testnets-in-metamask/
- MetaMask Sepolia faucet guide: https://support.metamask.io/develop/blockchain-networks/testnets/using-the-testnet-faucet/
- Ethereum Sepolia network and faucet list: https://ethereum.org/developers/docs/networks/
- Send ETH from MetaMask: https://support.metamask.io/manage-crypto/move-crypto/send/how-to-send-tokens-from-your-metamask-wallet
- Sepolia Etherscan: https://sepolia.etherscan.io/
