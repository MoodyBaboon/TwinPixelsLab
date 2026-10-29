# Privacy Policy

**Last Updated:** October 21, 2026
**Effective Date:** October 16, 2026 (OchiJump 2.0.0)

---

> **The short version:** OchiJump saves your game to our own cloud backend, runs public leaderboards, keeps a ledger of the in-game currency you earn and spend, and records how the game is played so we can make it better. That data is tied to a random install ID and to your game account — not to your name. We **never** collect your real name, email address, phone number, physical address or location, and we **never** have access to your private keys or the ability to move your funds. You can switch usage analytics off at any time in **Settings → Privacy → Share usage data**. Raw gameplay and usage records are permanently deleted after **180 days**.

---

## 1. Who We Are

This Privacy Policy describes how **TwinPixelsLab** ("we," "us," or "our") handles information in connection with **OchiJump**, a mobile platformer game (the "Game").

This version describes OchiJump 2.0.0 and later: game accounts that work without a wallet, in-game currencies, the hard-currency purchase gateway, and usage analytics. It replaces every earlier version.

---

## 2. Data We Collect

Everything below flows only to our own backend, hosted on Supabase (see Section 11). We do not use third-party analytics or advertising SDKs.

### 2.1 Your Game Account

- **Guest account.** The first time the Game has something to save for you (a finished run, a purchase, a redeemed code), it creates a game account on our server with a random internal identifier. No wallet, email or sign-in is needed.
- **Linked wallet (optional).** If you connect a Solana wallet, we store its **public address** (Base58 public key) and, if you have one, your **`.sol` / `.skr` domain name**, so your account can be restored on another device. A device can hold several accounts and switch between them.
- **Sessions.** We issue session tokens that keep the Game signed in to your account, and keep a technical record of when they were issued and last used (including the app's user-agent string) for security.

### 2.2 Install Identifier

A random UUID the Game generates on first launch (the "install ID") groups the records of one installation. It is **not** your device's hardware identifier, advertising ID or IMEI, and it changes if you reinstall the Game.

### 2.3 Gameplay Records (Runs)

For each run: the location and mode, the run's random seed, its duration, how it ended, the height reached, jumps, enemies defeated, items collected, the skin played, revives taken, and the app version and platform (e.g. Android). These power the leaderboards and the in-game rewards for a run.

### 2.4 Usage Analytics

To understand how the Game is played and improve it, the Game records events such as:

- when the app is opened and sent to the background, and how long a session lasts;
- which screens and tabs you visit;
- your interactions with the shop and purchase screens — which items you looked at, whether you opened a purchase, and whether it succeeded, was cancelled or was refused (for example for insufficient in-game currency);
- the hero, skins, weapon skins, implants and other equipment you choose, and changes to them;
- in-run statistics such as which weapons, upgrades and implants you used and how often, which enemies you defeated, revives offered and taken, and the buttons you chose at the end of a run;
- your progress: levels reached, rewards claimed, achievements completed;
- your interactions with the Ochi-Pet pocket pet and its mini-games;
- changes to your settings, tutorial steps shown, sign-in outcomes, and error reports when the Game crashes;
- how smoothly a run played: how many frames were drawn and how many were late.

Each event is recorded with the time it happened, a random session identifier, your install ID, your game account (if one exists), and the app version and platform. **Usage analytics never include your wallet address.** You can switch them off (Section 4).

Once per app launch the Game also records the **kind** of device it runs on: its make and model (for example "Samsung SM-S911B"), the operating-system version, the device's language and region setting (for example "uk-UA" — a setting, not your location) and the app store that installed the Game. This tells us which phones a crash or a slow frame happens on. It describes the type of device, not your particular device: it is not a hardware identifier and cannot single you out.

We may collect usage analytics from only a random share of installations, to keep the amount of data small. Whether an installation is in that share is decided by its install ID, so it is either included or not; error reports are always sent.

### 2.5 Economy Records

The Game keeps a ledger of your in-game economy, synchronised with our server: soft and hard currency earned and spent (and on what — for example a shop item, a revive or a re-roll), items granted or used up, promo codes redeemed, and the resulting balances and owned items. This record is what lets your purchases and balances follow your account and lets us detect and correct errors and fraud.

### 2.6 Hard-Currency Purchases

When you buy hard currency with SOL or SKR, we create a signed price quote and record it together with your **wallet address**, the bundle, the currency and amount, its approximate US-dollar value, and its status. When the payment lands on the blockchain we record its **transaction signature**, slot and time, and credit the hard currency to your account.

### 2.7 Leaderboards

Your best height is published on **public** leaderboards under a display name: your `.sol` / `.skr` domain or a shortened wallet address if your account has a wallet, otherwise a randomly generated name. Daily Run results are published the same way.

### 2.8 Cloud Save

Your progress — experience, unlocked locations and skins, and related configuration — is saved to your account on our server so it can be restored on a new device.

### 2.9 Standard Request Metadata

Like any internet service, our infrastructure and providers may log technical metadata such as your **IP address** and request timestamps. We use it only for security, abuse prevention and rate limiting — not to build a profile of you.

---

## 3. Data We Do NOT Collect

We do **not** collect, store or process:

- your real name, email address, phone number or physical address;
- your geographic location or GPS data;
- your device's hardware identifiers, advertising ID or IMEI;
- contacts, photos, microphone or camera data;
- biometric data;
- payment-card or bank details (real-money payments are made from your own wallet; see Section 7).

OchiJump does **not** embed third-party behavioural-analytics or advertising SDKs (such as Firebase Analytics, Mixpanel or Amplitude) and does **not** use third-party crash-reporting services (such as Sentry or Bugsnag). All telemetry and analytics flow only to our own backend.

---

## 4. Your Analytics Choice

**Settings → Privacy → Share usage data** controls the usage analytics described in Section 2.4. It is **on** by default.

When you switch it **off**:

- the Game stops sending usage analytics from that device, effective immediately;
- one event recording that you switched it off is sent, so we know how many players opt out;
- error reports (crash information) are still sent, because we need them to keep the Game working;
- gameplay records (Section 2.3), economy records (2.5), purchases (2.6), leaderboards (2.7) and cloud save (2.8) are **not** affected — they are part of how the Game works, not analytics.

Switching it off does not delete what was sent before; to request deletion, see Section 10. The setting belongs to the device and applies to every account used on it.

---

## 5. How We Use Data

- to run the Game: your account, cloud save, purchases, balances, rewards and leaderboards;
- to keep it fair and secure: detecting cheating, abuse and fraud, and correcting errors in the economy;
- to improve it: understanding which features are used, where players get stuck or leave, how long sessions last and how many players return, and balancing difficulty and prices;
- to fix bugs: crash reports and app-version/platform information.

We do **not** sell your data, do not use it for advertising, and do not share it with third parties except the service providers in Section 11, which process it on our behalf.

---

## 6. Data Retention

- **Raw gameplay and usage records** (individual runs and analytics events) are **permanently deleted 180 days** after they are created, by an automated scheduled job.
- **Economy records and purchase records** (Sections 2.5–2.6) are kept for as long as your account exists, because they are your balances and purchases, and because we need them to resolve disputes and detect fraud.
- **Leaderboard standings and cloud-saved progress** are kept for as long as your account exists.
- **Idle guest accounts** that hold nothing of value (no currency, no items, no purchases, no linked wallet) may be deleted after a period of inactivity; their past gameplay and usage records then remain only under the install ID, without an account.
- **Local device data** remains until you uninstall the Game.
- **On-chain data** is permanent and outside our control (Section 8).

---

## 7. Wallets, Payments & Your Keys

- We store your wallet's **public address** and, optionally, its **`.sol` / `.skr` domain name**. Both are public by nature.
- To sign in, your wallet signs a one-time "Sign In With Solana" message proving you control it. Nothing is moved or spent.
- To buy hard currency, the Game asks our server for a price quote, and your wallet app shows you the exact transfer before you approve it. The transfer goes from your wallet to our treasury through our on-chain payment program; we only see the resulting public transaction.
- **We never receive, store or have access to your private keys or seed phrase**, and we have **no ability to initiate, approve or reverse any transaction** on your behalf. All signing happens inside your own wallet app via the Solana Mobile Wallet Adapter (MWA) protocol.

---

## 8. Blockchain & Public Data

A hard-currency purchase is a transaction on the **Solana blockchain**, which is permanent and publicly visible. It shows:

- your **wallet's public address**;
- the **amount of SOL or SKR** transferred to the OchiJump treasury;
- a reference to the price quote, and the **time** of the transaction;
- that it was processed by the OchiJump payment program (Program ID: `ochiMq7xDD9QHa8bgcjfQf6qf4zCRsamTUKicFmsurX`).

The hard currency you receive and the items you buy with it are **records in our game backend**, not tokens or NFTs on the blockchain.

Purchases made with earlier versions of the Game, through our former on-chain store program, were recorded on-chain against the purchasing wallet and remain publicly readable there; the content they unlocked is honoured in your account.

Records on a public blockchain are **permanent and immutable**. TwinPixelsLab cannot delete or modify on-chain transaction history, and **the right to erasure does not apply to on-chain data**. Anyone can view Solana transactions using public explorers such as [Solana Explorer](https://explorer.solana.com) or [Solscan](https://solscan.io).

---

## 9. Data Stored Locally on Your Device

OchiJump stores data in your device's local storage (`react-native-mmkv`), including:

| What it is | Why |
|---|---|
| The install ID | Groups your records (Section 2.2) |
| Your game accounts' profiles and session tokens | Keep you signed in; let the device switch accounts |
| Your wallet's public address and the wallet-adapter session token | So you don't have to reconnect your wallet every launch |
| Game progress, scores, unlocked content, equipment, Ochi-Pet state | Your local save (also synced to your account) |
| The economy journal | Purchases and balance changes made offline, until they reach the server |
| Unsent gameplay and analytics records | Sent when the network is available |
| A saved in-progress run | So an interrupted run is not lost |
| The install date, launch count and last-background time | To measure sessions (Section 2.4) |
| Your settings, including "Share usage data" | Your preferences |

Android's automatic backup is disabled for OchiJump. **All locally stored data is deleted when you uninstall the Game.**

---

## 10. Your Rights and Choices

### Usage Analytics
Switch it off at any time: **Settings → Privacy → Share usage data** (Section 4).

### Disconnecting Your Wallet
You can disconnect your wallet in the Game at any time; the device returns to its guest account. You should also revoke OchiJump's authorization in your wallet app.

### Access and Deletion
You may ask for a copy of, or deletion of, the data associated with your account — your profile, cloud save, leaderboard entries, economy and purchase records, and gameplay and usage records — by contacting us (Section 15). We will need to verify that the account is yours (for a wallet account, by a signed message; for a guest account, from the device that holds it). We may keep records we are legally required to keep, or need to resolve a dispute or prevent fraud, for as long as that requires. Raw gameplay and usage records are deleted automatically after 180 days regardless.

### Deleting Local Data
Uninstall OchiJump.

### On-Chain Data
On-chain records cannot be deleted by TwinPixelsLab or by you (Section 8).

---

## 11. Third-Party Services

We do not control their data practices — please review their privacy policies.

### Supabase (supabase.com)
Our cloud backend provider (database, authentication and serverless functions) for accounts, cloud save, economy and purchase records, gameplay and usage analytics, and leaderboards. It may process technical request metadata such as IP addresses.
- Privacy Policy: https://supabase.com/privacy

### Helius (helius.dev)
Our primary Solana RPC provider. When the Game reads the blockchain or submits a signed transaction, requests may be routed through Helius, which may log your IP address and request metadata.
- Privacy Policy: https://www.helius.dev/privacy-policy

### Solana Foundation (Public RPC)
Used as a fallback RPC endpoint. Similar logging may apply.
- Privacy Policy: https://solana.com/privacy-policy

### Your Wallet App (e.g. the Solana Seeker's wallet, Phantom)
Wallet authorization and transaction signing happen inside your wallet app via the Solana Mobile Wallet Adapter (MWA) protocol. Please refer to its privacy policy.

---

## 12. Android Permissions Explained

### `android.permission.INTERNET`
Used to communicate with our backend (accounts, cloud save, economy, purchases, gameplay and usage records, leaderboards) and with Solana RPC endpoints (balances, payment transactions). No private keys are ever included in these requests.

### `android.permission.VIBRATE`
Used for haptic feedback during gameplay. No data is collected through this permission.

---

## 13. Children's Privacy

OchiJump is not directed to children under the age of 13. We do not knowingly collect personal information from children under 13. Users between 13 and 17 may use the Game only with parental or guardian consent.

If you believe a minor has provided personal information in connection with OchiJump, please contact us and we will take appropriate steps.

---

## 14. Security

- **HTTPS only.** All network communication is encrypted (`android:usesCleartextTraffic="false"`).
- **No direct database access.** The Game reaches our database only through controlled server-side functions with row-level security.
- **Signed prices.** Every hard-currency price is signed by our server and checked by the Game before your wallet opens.
- **No private-key handling.** Transaction signing happens entirely in your wallet app.
- **No cloud backup of local data.** Android's automatic backup is disabled (`android:allowBackup="false"`).

No method of transmission or storage is 100% secure, but we work to protect your data using industry-standard practices.

---

## 15. Changes to This Policy & Contact

We may update this Privacy Policy from time to time. Changes are reflected by the "Last Updated" date above; we will tell you about material changes through an in-app notice or the app store's update notes. Your continued use of OchiJump after changes are posted constitutes acceptance of the revised Policy.

For questions, or to request access to or deletion of your data:

**TwinPixelsLab**
Email: contact@twinpixelslab.com
Website: https://twinpixelslab.com
