# DraftTracks v3 Core

> 🧱 Core smart contracts for the [DraftTracks](https://drafttracks.com) Decentralized Artist Exchange (DEX), adapted from Uniswap v3. Enables on-chain trading, liquidity provisioning, and governance of artist tokens powered by $TRACK.

---

## 🔍 Overview

This repository contains the core contracts that power the **DraftTracks DEX**, a protocol where fans can trade, stake, and govern the rise of human and AI artists through artist tokens and $TRACK.

Built on top of [Uniswap v3-core](https://github.com/Uniswap/v3-core), this fork provides the decentralized liquidity and swap infrastructure needed for:

- Trading $TRACK and artist tokens
- Creating liquidity pools with configurable fees
- NFT-based LP positions and incentives
- Future integration with on-chain battle logic and AI producers

---

## 🧱 Core Components

| Contract                  | Description |
|---------------------------|-------------|
| `UniswapV3Factory.sol`    | Deploys pools and tracks authorized fee tiers |
| `UniswapV3Pool.sol`       | Handles swaps, liquidity, and tick management |
| `UniswapV3PoolDeployer.sol` | Orchestrates pool initialization |
| `Tick.sol`                | Tracks per-price-level liquidity |
| `Observation.sol`         | Stores time-weighted average price data for oracles |
| `DraftTracksHooks.sol` *(planned)* | Optional logic for artist battles, staking boosts, and fan rewards |

---

## 🔗 Related Repositories

- [`drafttracks-v3-periphery`](https://github.com/DraftTracks/drafttracks-v3-periphery) — Swap routing, LP NFTs, and external interface contracts
- [`drafttracks-token`](https://github.com/DraftTracks/track-token) — The official $TRACK ERC-20 token
- [`drafttracks-artist-factory`](https://github.com/DraftTracks/artist-token-factory) — Artist token creation and registration

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/DraftTracks/drafttracks-v3-core.git
cd drafttracks-v3-core
npm install
````

### 2. Compile Contracts

```bash
npm run compile
```

✅ This repo is usually deployed alongside [`drafttracks-v3-periphery`](https://github.com/DraftTracks/drafttracks-v3-periphery).

---

## 🛠 Deployment Guide (Polygon / Base)

1. Deploy core contracts from this repo:

   * `UniswapV3Factory`
   * `UniswapV3PoolDeployer`

2. Deploy periphery contracts:

   * `SwapRouter`
   * `NonfungiblePositionManager`

3. Deploy \$TRACK and artist tokens

4. Create liquidity pools:
   e.g. `$TRACK / $GABBY`, `$TRACK / $NEOT`, `$TRACK / $ROXY`

5. Manage trading, staking, and LPs through your mobile app or custom frontend

---

## 🎯 DraftTracks Use Cases

* 🎧 Trade \$TRACK ↔ artist tokens
* 🛠 LP with unique artist-based fee tiers
* 🖼 Use LP NFTs to track performance or award fan badges
* 🧠 Future support for AI-driven agents, tokenized performance boosts, and reward hooks

---

## 🔐 License

This project is a fork of [Uniswap v3-core](https://github.com/Uniswap/v3-core), licensed under the **Business Source License 1.1 (BSL-1.1)**.

> Use is non-commercial until **April 1, 2025**. After that, BSL converts to a permissive GPL license.

---

## 📣 Contact

Built and maintained by the DraftTracks protocol team.
Explore the future of tokenized music careers and fan-powered artist ecosystems.

* 💼 Jason Amos – `jay@drafttracks.com`
* 🌐 [https://drafttracks.com](https://drafttracks.com)
