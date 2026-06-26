# StellarPay

### Decentralized Escrow Platform Built on Stellar & Soroban

🎥 **Demo Video**

https://drive.google.com/file/d/1XdiRBa6sInlLqmFSyftHdSAv9h8t1sje/view

🌐 **Live Demo**

[StellarPay](https://stellarpay21.netlify.app/)

---

# Overview

StellarPay is a decentralized escrow platform built on the Stellar Testnet using Soroban Smart Contracts.

The platform enables users to securely lock XLM into escrow agreements, release or refund funds, manage disputes, and maintain an on-chain reputation score. It also provides analytics, transaction tracking, live activity updates, and multi-wallet support through a frontend-first architecture.

---

# Features

- Multi-Wallet Support (Freighter, Albedo, xBull)
- Wallet Connect / Disconnect
- XLM Balance Display
- Escrow Creation
- Release & Refund Workflow
- Dispute Resolution
- Reputation Dashboard
- Trust Leaderboard
- Analytics Dashboard
- Event Feed
- Transaction Lifecycle Tracking
- Mobile Responsive UI
- Soroban Smart Contract Integration
- GitHub Actions CI/CD
- Frontend & Smart Contract Tests

---

# Tech Stack

## Frontend

- React
- Vite
- Tailwind CSS
- TypeScript

## Blockchain

- Stellar SDK
- Soroban SDK
- Horizon API
- Soroban RPC

## Wallets

- Freighter
- Albedo
- xBull

## Deployment

- Netlify

## CI/CD

- GitHub Actions

---

# Architecture

```mermaid
flowchart LR

User --> Wallet

Wallet --> Frontend

Frontend --> Horizon

Frontend --> SorobanRPC

SorobanRPC --> EscrowContract

EscrowContract --> ReputationContract

EscrowContract --> StellarTestnet

ReputationContract --> StellarTestnet
```

---

# User Flow

```text
Connect Wallet
        ↓
Create Escrow
        ↓
Lock XLM
        ↓
Release / Refund
        ↓
Reputation Updated
        ↓
Transaction Completed
```

---

# Screenshots

## Dashboard

<img width="1916" height="931" src="https://github.com/user-attachments/assets/e5f894e0-820d-4a5d-a62c-142a3008d139" />

---

## Wallet Integration

<img width="1912" height="970" src="https://github.com/user-attachments/assets/c44d9c0e-19fa-4316-a3fe-a48fcd3301ad" />

---

## Reputation Dashboard

<img width="1919" height="932" src="https://github.com/user-attachments/assets/54030de3-bf3c-4dc9-9400-a1adc1cef697" />

---

## Escrow Manager

<img width="1919" height="930" src="https://github.com/user-attachments/assets/93ad8301-d69c-4888-88c3-55e8a4535bc1" />

---

## Activity Feed

<img width="1907" height="929" src="https://github.com/user-attachments/assets/e79f3328-b62d-4e5b-a678-832a21432cb5" />

---

## Analytics Dashboard

<img width="1915" height="932" src="https://github.com/user-attachments/assets/a3f36208-b1fc-400d-a68f-d1c5d0ad2713" />

---

## Mobile Responsive UI

<img width="380" height="810" src="https://github.com/user-attachments/assets/e31dc753-0134-4151-94b2-f47968b55b73" />

---

## CI/CD Pipeline

<img width="1917" height="976" src="https://github.com/user-attachments/assets/551f7767-89a2-4fe7-aeec-a55a6bf1009f" />

---

# Smart Contracts

## Escrow Contract

Functions

- Create Escrow
- Release Funds
- Refund Funds
- Cancel Escrow
- Open Dispute

**Contract Address**

```text
<ESCROW_CONTRACT_ADDRESS>
```

---

## Reputation Contract

Functions

- Create Profile
- Update Reputation
- Fetch Reputation
- Trust Score

**Contract Address**

```text
<REPUTATION_CONTRACT_ADDRESS>
```

---

# Transaction Verification

**Transaction Hash**

```text
<YOUR_TRANSACTION_HASH>
```

Verify Transaction

https://stellar.expert/explorer/testnet/tx/<YOUR_TRANSACTION_HASH>

---

# Project Structure

```bash
src/
├── components/
├── hooks/
├── pages/
├── services/
├── contexts/
├── utils/

contracts/
├── escrow/
└── reputation/

tests/

.github/
└── workflows/
```

---

# Local Setup

```bash
git clone https://github.com/aruu-27/StellarPay.git

cd StellarPay

npm install

npm run dev
```

---

# Build

```bash
npm run build
```

---

# Run Tests

Frontend

```bash
npm test
```

Contracts

```bash
cargo test
```

---

# Deployment

```bash
npm run build
```

Deploy the generated `dist/` folder to **Netlify**.

---

# CI/CD

GitHub Actions automatically performs:

- Install Dependencies
- Build Application
- Frontend Tests
- Smart Contract Tests

---

# Stellar Level 3 Checklist

- Wallet Connection
- Multi-Wallet Support
- Balance Fetching
- Smart Contract Deployment
- Frontend Contract Calls
- Event Streaming
- Transaction Tracking
- Error Handling
- Loading States
- Mobile Responsive UI
- Frontend Tests
- Smart Contract Tests
- GitHub Actions CI/CD
- Documentation
- Live Demo
- Demo Video

---

# License

MIT License
