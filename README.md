# 🐄 CAOW Token Launchpad

This is a dApp built with React and Solana's Web3 libraries to help you **create custom tokens with metadata** on Solana using the **Token 2022 Program**.

---

## 🚀 Features

- Creates a custom **SPL token** on Solana (Token-2022).
- Attaches **on-chain metadata** using the MetadataPointer extension.
- Mints tokens into your wallet automatically.
- Shows the associated token account address (ATA).

---

## 📦 Tech Stack

- React
- Solana Web3.js
- SPL Token 2022
- SPL Metadata Extension
- Phantom Wallet Adapter

---

## 🧠 How It Works

1. **Create Mint Account** – A new token mint is initialized.
2. **Add Metadata Pointer** – Adds pointer to metadata on-chain.
3. **Attach Metadata** – Using your own hosted `metadata.json`.
4. **Create ATA** – Your wallet’s token account is created.
5. **Mint Tokens** – Mints the supply directly to your wallet ATA.

---

## 🐮 Your Token Details

```js
const metadata = {
    mint: mintKeypair.publicKey,
    name: 'CAOW',
    symbol: 'COW    ',
    uri: 'https://raw.githubusercontent.com/NgrTushar/metadata.json/refs/heads/main/metadata.json',
    additionalMetadata: [],
};
```

---

## 🌐 Hosted Metadata

You hosted your metadata using GitHub raw:

🔗 **URI used in token metadata:**

```
https://raw.githubusercontent.com/NgrTushar/metadata.json/refs/heads/main/metadata.json
```

📁 **Contents of `metadata.json`:**
```json
{
  "name": "CAOW",
  "symbol": "COW",
  "uri": "https://your-image-url.com/logo.png",
  "seller_fee_basis_points": 0,
  "creators": null
}
```

---

## 💡 How to Host Your Own metadata.json

1. Create a new repo on GitHub.
2. Upload your `metadata.json`.
3. Open the file and click **"Raw"**.
4. Copy that raw URL.
5. Use that URL as the `uri` in your token metadata.

---

## 🔧 Run Locally

```bash
git clone https://github.com/your-username/caow-token-launchpad.git
cd caow-token-launchpad
npm install
npm run dev
```

- Make sure you're on **Solana Devnet** in Phantom.
- Connect your wallet.
- Click “Create Token” – done!

---

## 🧪 Test & Verify

- Go to [Solana Explorer (Devnet)](https://explorer.solana.com/?cluster=devnet)
- Paste your **mint address** or **associated token address**
- Check token info and metadata

---

