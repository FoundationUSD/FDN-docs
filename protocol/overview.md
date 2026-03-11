# Protocol Overview

## What is Foundation?

Foundation is a protocol that wraps tokenized real-world credit assets (RWAs) into permissionless, composable DeFi vault tokens. It bridges the $139T global fund management industry with onchain capital.

## Core Problems Solved

| Problem | Traditional | Foundation |
|---|---|---|
| **Access** | $1M+ minimums, accredited only | $1 minimum, permissionless |
| **Liquidity** | 14–90 day redemptions | Instant (T+0) via liquidity buffer |
| **Composability** | None — siloed tokens | Full ERC-4626, integrates with DeFi natively |

## How It Works

```
User deposits USDC on any chain
  → FdnRouter allocates across vaults per strategy weights
  → Each vault mints ERC-4626 shares to user
  → Shares represent pro-rata claim on underlying + accrued yield
  → Share price increases as yield accrues (no claiming needed)
  → User redeems shares for USDC at any time
```

## Target Yield

8–18% USD APY depending on vault and leverage configuration.

## Vault Tokens

fdnUSD is the collective brand for Foundation vault share tokens:

| Token | Full Name | Underlying |
|---|---|---|
| `fdnBUILD` | Foundation BUIDL Vault Share | BlackRock BUIDL |
| `fdnAPOLLO` | Foundation Apollo Vault Share | Apollo ACRED |
| `fdnGAIB` | Foundation GAIB Vault Share | GAIB GPU Notes |

All vault shares are standard ERC-20, ERC-4626 compliant, yield-bearing, and cross-chain via LayerZero OFT.

## Tech Stack

- **Contracts**: Solidity 0.8.24, Foundry, OpenZeppelin v4.9.6, UUPS upgradeable
- **App**: Vue 3, TypeScript, wagmi, viem, Tailwind CSS
- **Infrastructure**: Vercel, Supabase, Chainlink/Pyth oracles, LayerZero, OpenZeppelin Defender
