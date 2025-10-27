# Ethereum Improvement Proposals (EIPs)

## What are EIPs?
Ethereum Improvement Proposals (EIPs) are standardized documents that describe new features, processes, or improvements for the Ethereum network.  
They serve as the main mechanism for proposing changes and recording design decisions. Each EIP follows a lifecycle from **Draft → Review → Last Call → Final**.  
When an EIP reaches the **Final** stage, it is officially adopted or implemented into the Ethereum protocol.

---

## 🧩 Final EIPs Explained

### 🪙 EIP-1559: Fee Market Change for ETH 1.0 Chain
**Status:** Final  
**Link:** [EIP-1559 on eips.ethereum.org](https://eips.ethereum.org/EIPS/eip-1559)

**Overview:**  
EIP-1559 introduced a new transaction fee mechanism to replace the traditional first-price auction model. Instead of users bidding blindly for gas, a **base fee** is automatically adjusted according to network demand and **burned** rather than paid to miners.

**Key Points:**
- Introduces a dynamic **base fee** that adjusts based on block congestion.  
- Users pay `max_fee = base_fee + tip`, where the **base fee** is burned and **tip** goes to the miner.  
- Helps make transaction fees more predictable.  
- Adds a deflationary element to ETH since part of the fees are destroyed.

**Impact:**  
EIP-1559 improved user experience, stabilized gas prices, and reduced ETH inflation. It’s considered one of Ethereum’s most impactful upgrades since it changed the network’s economic model.

**Conclusion:**  
EIP-1559 represents a critical shift toward predictable gas pricing and sustainable token economics for Ethereum.

---

### 🔄 EIP-3675: Upgrade Consensus to Proof-of-Stake
**Status:** Final  
**Link:** [EIP-3675 on eips.ethereum.org](https://eips.ethereum.org/EIPS/eip-3675)

**Overview:**  
EIP-3675 formalized Ethereum’s transition from **Proof-of-Work (PoW)** to **Proof-of-Stake (PoS)**. This proposal defined how Ethereum’s mainnet merged with the Beacon Chain, eliminating mining and adopting validator-based consensus.

**Key Points:**
- Established a **terminal total difficulty (TTD)** to trigger the Merge.  
- Deprecated PoW block validation and replaced it with PoS logic.  
- Updated block headers and fork choice rules.  
- Removed mining-based rewards, introducing staking incentives instead.

**Impact:**  
This EIP powered **The Merge**, one of the most significant events in blockchain history. It reduced Ethereum’s energy consumption by ~99.95% and laid the foundation for future scalability and sustainability.

**Conclusion:**  
EIP-3675 transformed Ethereum’s security model and environmental impact, marking a new era for the network’s consensus mechanism.

---

### 💾 EIP-4844: Shard Blob Transactions
**Status:** Final  
**Link:** [EIP-4844 on eips.ethereum.org](https://eips.ethereum.org/EIPS/eip-4844)

**Overview:**  
EIP-4844 introduces **blob-carrying transactions**, which include large chunks of data (called blobs) that are not directly accessible by the EVM but are used to improve **data availability** for Layer 2 rollups.

**Key Points:**
- Adds a new transaction type for storing blob data.  
- Blob data is temporary and cheaper than normal calldata.  
- Significantly lowers costs for rollups (e.g., Optimism, Arbitrum).  
- Forms a foundation for future **full sharding** upgrades.

**Impact:**  
By reducing data storage costs and increasing throughput, EIP-4844 accelerates Ethereum’s roadmap toward scalability and efficiency.

**Conclusion:**  
EIP-4844 is a vital step in making Ethereum rollup-centric, improving performance without sacrificing decentralization.

---

## 📚 References
- [EIP-1: Ethereum Improvement Proposals](https://eips.ethereum.org/EIPS/eip-1)
- [EIP-1559: Fee Market Change](https://eips.ethereum.org/EIPS/eip-1559)
- [EIP-3675: Proof-of-Stake Upgrade](https://eips.ethereum.org/EIPS/eip-3675)
- [EIP-4844: Shard Blob Transactions](https://eips.ethereum.org/EIPS/eip-4844)

---
