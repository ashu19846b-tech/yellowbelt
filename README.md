# ⭐ StarVote — Stellar Live Poll

A fully on-chain live polling dApp built with **Soroban**, **Stellar Testnet**, and **Next.js 16**. Users connect their wallet, cast one on-chain vote, and view live poll results with real-time updates.

---

## 🔗 Live Demo

https://orange-belt-deploy-ra74.vercel.app

## 📹 Demo Video

https://youtu.be/mpj_mVS9BTk

---

## 🚀 Features

* ✅ Multi-wallet integration (StellarWalletsKit)
* ✅ Soroban smart contract deployed on Stellar Testnet
* ✅ One vote per wallet (on-chain validation)
* ✅ Contract interaction from the frontend
* ✅ Real-time poll result synchronization
* ✅ 4-step transaction status tracker:

  * Signing
  * Broadcasting
  * Confirming
  * Complete
* ✅ Error handling:

  * Wallet not installed
  * Transaction rejected
  * Insufficient balance / network error
* ✅ localStorage caching (30-second TTL)
* ✅ 7/7 Soroban contract tests passing

---

## 💻 Tech Stack

| Layer          | Technology                              |
| -------------- | --------------------------------------- |
| Frontend       | Next.js 16, TypeScript, Tailwind CSS v4 |
| Smart Contract | Rust + Soroban SDK                      |
| Wallet         | StellarWalletsKit                       |
| Network        | Stellar Testnet                         |
| Deployment     | Vercel                                  |

---

## 📜 Smart Contract

**Network:** Stellar Testnet

**Contract Address**

```text
CCYUDN6DSM4YJ3KZ7NSGFSK4UWI76JTCYI6VPVH3WH6MX44T7C2PNB2K
```

### Contract Functions

* `initialize()`
* `vote()`
* `get_results()`
* `get_options()`
* `get_question()`
* `has_voted()`

---

## ✅ Transaction Proof

**Transaction Hash**

```text
9b220fbf5e2c268403830452d08d1de3e5586eee25371a543ec234ad604a83c3
```

**Explorer**

https://stellar.expert/explorer/testnet/tx/9b220fbf5e2c268403830452d08d1de3e5586eee25371a543ec234ad604a83c3

---

## 📸 Screenshots

* Wallet Options
* Wallet Connected
* Transaction Status
* Successful Vote
* Tests Passing (7/7)
* User Rejected Transaction
* Insufficient Balance Error

---

## ⚙️ Setup

### Prerequisites

* Node.js 20+
* Rust
* Stellar CLI
* StellarWalletsKit-supported wallet

### Installation

```bash
git clone https://github.com/Nandini-Jadhav1/orange-belt-deploy.git

cd orange-belt-deploy/contracts/hello-world/live-poll-ui

npm install

npm run dev
```

Create `.env.local`

```env
NEXT_PUBLIC_CONTRACT_ID=CCYUDN6DSM4YJ3KZ7NSGFSK4UWI76JTCYI6VPVH3WH6MX44T7C2PNB2K
NEXT_PUBLIC_RPC_URL=https://soroban-testnet.stellar.org
```

---

## 🚀 Deployment

```bash
cd contracts/hello-world

stellar contract build

stellar contract deploy

stellar contract invoke -- initialize
```

Deploy the frontend to Vercel and set the contract ID as an environment variable.

---

## 🧪 Running Tests

```bash
cd contracts/hello-world

cargo test
```

**Result:** ✅ **7 / 7 tests passing**

---

## 📌 Commit History

```text
feat: complete StarVote dApp with Soroban smart contract
test: add 7 Soroban contract tests
feat: add loading states, transaction tracker and caching
docs: complete README with setup and deployment
docs: add live demo, contract address, transaction proof and screenshots
```

---

## ✅ Submission Checklist

* ✔ Public GitHub Repository
* ✔ README with setup instructions
* ✔ Live Demo
* ✔ Demo Video
* ✔ Multi-wallet integration
* ✔ Smart contract deployed on Testnet
* ✔ Contract called from frontend
* ✔ Transaction status visible
* ✔ Three error types handled
* ✔ Deployed contract address
* ✔ Transaction hash (verifiable on Stellar Expert)
* ✔ Screenshots (wallet, transaction, errors, tests)
* ✔ Minimum 2+ meaningful commits

---

## 📄 License

MIT © 2026
