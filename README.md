# 🌾 Cafers — Decentralized Agro Marketplace on Hedera

**Cafers** is a decentralized agro marketplace enabling **secured, transparent, and borderless trading** for African farmers, aggregators, and retailers — powered by **Hedera Hashgraph**.

---

## 🚀 Project Title & Track
**Title:** Cafers — Decentralized Agro Marketplace  
**Track:** DLT for Operations (PoC → Prototype)

---

## 🌍 About Cafers
Cafers bridges Africa’s fragmented agricultural ecosystem using blockchain technology.  
By leveraging Hedera’s micro-fee architecture, ABFT consensus, and carbon-negative infrastructure, we empower smallholder farmers with fair, traceable, and borderless trade.

---

## ⚙️ Hedera Integration Summary

### 🧩 Hedera Consensus Service (HCS)
Used for **immutable, ordered logging** of supply chain events such as product listings, sales, and delivery confirmations.  
**Why:** Predictable micro-fees ($0.0001 per message) guarantee operational cost stability for low-margin logistics in Africa.  
**Transaction Types:**  
`TopicCreateTransaction`, `TopicMessageSubmitTransaction`, `TopicMessageQuery`  
**Economic Justification:**  
Low and predictable fees make large-scale event logging affordable for thousands of smallholder farmers.

---

### 💰 Hedera Token Service (HTS)
Used to mint and manage **CafersCredits (CFC)** — digital tokens representing subsidies, credits, or marketplace loyalty points.  
**Why:** Native HTS provides efficient, low-cost, and auditable token transfers ideal for micro-payments.  
**Transaction Types:**  
`TokenCreateTransaction`, `TokenMintTransaction`, `TokenAssociateTransaction`, `TokenTransferTransaction`  
**Economic Justification:**  
Predictable token transfer costs allow financial inclusion and incentivized participation without overburdening users.

---

### 🔐 Hedera Smart Contracts (EVM)
Used for **escrow and automated trade settlements** when delivery confirmations are logged on HCS.  
**Why:** Enables trustless payments and ensures buyers’ funds are only released when verified events occur.  
**Transaction Types:**  
`ContractCreateTransaction`, `ContractExecuteTransaction`, `ContractCallQuery`  
**Economic Justification:**  
Low gas-like fees and fast ABFT finality make contract-based trade automation practical for small-value transactions.

---

### 🔎 Mirror Nodes
Used to **fetch, verify, and display** consensus data and topic messages for users in the frontend.  
**Why:** Mirror nodes make transaction data verifiable, public, and tamper-proof, improving transparency and trust across the supply chain.

---

## 🧾 Transaction Types Summary
- `TopicCreateTransaction`
- `TopicMessageSubmitTransaction`
- `TopicMessageQuery`
- `TokenCreateTransaction`
- `TokenMintTransaction`
- `TokenAssociateTransaction`
- `TokenTransferTransaction`
- `ContractCreateTransaction`
- `ContractExecuteTransaction`
- `ContractCallQuery`

---

## 💸 Economic Justification
Hedera’s **micro-fee, high-throughput, and ABFT architecture** ensure:
- Predictable and ultra-low transaction costs for smallholder operations  
- Secure and transparent recordkeeping  
- Financial viability even for low-margin agricultural trades  
- Faster adoption through affordable participation

---

## 🧑‍💻 Deployment & Setup Instructions

### Prerequisites
- Node.js ≥ v18  
- Hedera Testnet account → [Create one here](https://portal.hedera.com/register)

### Step-by-Step
1. **Clone Repo**
   ```bash
   git clone https://github.com/<your-org>/cafers-hedera-poc.git
   cd cafers-hedera-poc