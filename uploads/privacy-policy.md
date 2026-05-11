# Privacy Policy

**Last Updated:** May 10, 2026
**Effective Date:** May 10, 2026

---

> **The short version:** OchiJump has no backend servers. We do not collect your name, email address, location, or any personal identifiers on our own systems. Almost everything stays on your device. The one exception is the Solana blockchain — it is public by design.

---

## 1. Who We Are

This Privacy Policy describes how **TwinPixelsLab** ("we," "us," or "our") handles information in connection with **OchiJump**, a mobile platformer game available exclusively for Solana Mobile-compatible devices.

---

## 2. Data We Do NOT Collect

We do not operate backend servers or databases. As a result, we do **not** collect, store, or process:

- Your name, username, or email address
- Your phone number or physical address
- Your geographic location or GPS data
- Device identifiers (IMEI, advertising ID)
- Biometric data
- Financial credentials or payment card information
- Demographic information
- Behavioral analytics or usage telemetry

OchiJump contains **no analytics SDKs** (such as Firebase Analytics, Mixpanel, or Amplitude), **no advertising SDKs**, and **no crash-reporting services** (such as Sentry or Bugsnag).

---

## 3. Data Stored Locally on Your Device

OchiJump stores a small amount of data in your device's local storage using the `react-native-mmkv` library. This data never leaves your device and is never transmitted to TwinPixelsLab servers.

| Key | What it is | Why |
|---|---|---|
| `ochi_wallet_pubkey` | Your Solana wallet's Base58 public key | So you don't have to reconnect your wallet every time you launch the app |
| `solana_auth_token` | Mobile Wallet Adapter session token | Maintains your wallet authorization session without re-prompting |
| Game progress & high scores | Your in-game records and unlocked content state | Local save data |

**All locally stored data is deleted when you uninstall OchiJump.**

---

## 4. Blockchain & Public Data

This is the most important section for Web3 users.

### 4.1 What Goes On-Chain

When you make an in-game purchase, a transaction is submitted to the **Solana blockchain**. This transaction is permanent and publicly visible. The following information is recorded on-chain:

- Your **wallet's public address** (e.g., `7xKX...3fQz`)
- The **item(s) purchased** (encoded as bits in your `PlayerInventory` account)
- The **SOL amount transferred** to the OchiJump treasury wallet
- The **timestamp** of the transaction

### 4.2 Your PlayerInventory PDA Is Public

Your in-game item inventory is stored in a **Program Derived Address (PDA)** account managed by the OchiJump smart contract (Program ID: `DmxfvDvSkm6XEnt7VXMGjpTpt9vkFu7j3vQNbHg8Ds8w`). This account is tied to your wallet's public key and is **readable by anyone** who queries the Solana blockchain.

This means any person or service that analyzes the blockchain can associate your wallet address with the specific content you have purchased in OchiJump.

### 4.3 These Are NOT NFTs or Tokens

Your purchased items are stored as **technical state records** in the PDA — they are **not** NFT tokens, cNFTs, or SPL tokens. They will not appear in your wallet's token or NFT gallery. They are not tradable or transferable. This distinction does not change the fact that the underlying data is publicly readable on-chain.

### 4.4 We Cannot Delete On-Chain Data

The nature of a public blockchain is that records are **permanent and immutable**. TwinPixelsLab has no ability to delete or modify your on-chain transaction history or inventory PDA.

**The right to erasure (right to be forgotten) does not apply to on-chain data.** If this is a concern for you, please consider this before connecting your wallet and making purchases.

Anyone can view Solana transactions using public blockchain explorers such as [Solana Explorer](https://explorer.solana.com) or [Solscan](https://solscan.io).

---

## 5. Android Permissions Explained

OchiJump requests the following Android permissions:

### `android.permission.INTERNET`
Used exclusively to communicate with Solana RPC endpoints (Helius and the public Solana mainnet). These calls are used to:
- Read the current state of the OchiJump smart contract (store configuration, prices)
- Fetch your existing item inventory from the blockchain
- Submit signed purchase transactions to the Solana network

No personal data is included in these requests. All transmitted data consists of public blockchain queries.

### `android.permission.VIBRATE`
Used to provide haptic feedback during gameplay (e.g., when your character lands on a platform). No data is collected through this permission.

---

## 6. Third-Party Services

OchiJump uses the following third-party services. We do not control their data practices — please review their privacy policies for details.

### Helius (helius.dev)
Our primary Solana RPC provider. When the Game communicates with the blockchain, requests are routed through Helius. Helius may log your IP address and request metadata (which are standard practices for any network API).
- Privacy Policy: https://www.helius.dev/privacy-policy

### Solana Foundation (Public RPC)
Used as a fallback RPC endpoint. Similar logging may apply.
- Privacy Policy: https://solana.com/privacy-policy

### Device Wallet App (e.g., Phantom on Solana Seeker)
Wallet authorization and transaction signing occur within your device's native wallet application via the **Solana Mobile Wallet Adapter (MWA)** protocol. OchiJump communicates with your wallet using a local device intent — we never receive your private keys or seed phrase.
- Please refer to your wallet app's privacy policy for details on how it handles data.

---

## 7. Children's Privacy

OchiJump is not directed to children under the age of 13. We do not knowingly collect personal information from children under 13. Users between 13 and 17 may use the Game only with parental or guardian consent.

If you believe a minor has provided personal information in connection with OchiJump, please contact us and we will take appropriate steps.

---

## 8. Your Rights and Choices

### Deleting Local Data
To delete all locally stored data (wallet public key, auth token, game progress), simply **uninstall OchiJump** from your device.

### Disconnecting Your Wallet
You can disconnect your wallet at any time using the in-game Disconnect option. This removes your wallet's public key from local storage. You should also revoke OchiJump's authorization within your wallet application.

### On-Chain Data
On-chain records — including your `PlayerInventory` PDA and all transaction history — **cannot be deleted** by TwinPixelsLab or by you. This is a fundamental property of public blockchains. If you wish to stop any new on-chain data being associated with your wallet, simply stop making purchases and disconnect your wallet from the Game.

---

## 9. Data Retention

- **Local device data** is retained until you uninstall the app.
- **On-chain data** is permanent by the nature of the Solana blockchain and is not subject to our control.
- We retain no personal data on our servers because we have no servers that store user data.

---

## 10. Security

We take the following steps to protect your information:

- **HTTPS only.** All network communications from the Game use encrypted HTTPS connections (`android:usesCleartextTraffic="false"` in our Android manifest).
- **No cloud backup.** Android's automatic backup is disabled for OchiJump (`android:allowBackup="false"`), preventing local game data from being synced to Google servers.
- **No private key handling.** Transaction signing occurs entirely within your wallet app. OchiJump never touches your private key.

---

## 11. Changes to This Policy

We may update this Privacy Policy from time to time. Changes will be reflected by the updated "Last Updated" date at the top of this document. We will notify you of material changes through an in-app notice or via the app store update notes.

Your continued use of OchiJump after changes are posted constitutes your acceptance of the revised Privacy Policy.

---

## 12. Contact

If you have any questions or concerns about this Privacy Policy, please reach out:

**TwinPixelsLab**
Email: contact@twinpixelslab.com
Website: https://twinpixelslab.com
