# Vault Specifications

## BUILDVAULT

| Property | Value |
|---|---|
| Underlying | BlackRock BUIDL (US Treasury Money Market Fund) |
| Target APY | 4.5% |
| Risk Profile | Low |
| Redemption | Instant (T+0) |
| Leverage | 1.0x (no leverage) |
| Collateral | BUIDL tokens |
| Use Case | Stable yield parking, treasury management, collateral backing |

BlackRock's BUIDL is a tokenized US Treasury money market fund. BUILDVAULT wraps it into a permissionless vault token that can be used as pristine collateral across DeFi while earning base Treasury rates.

## APOLLOUSD

| Property | Value |
|---|---|
| Underlying | Apollo ACRED (Diversified Private Credit) |
| Target APY | 9.0% |
| Risk Profile | Medium |
| Redemption | Quarterly (underlying), Instant via liquidity buffer |
| Leverage | Up to 3.33x |
| Collateral | ACRED tokens |
| Use Case | Core yield allocation, institutional credit exposure |

Apollo's ACRED provides exposure to senior secured corporate lending, asset-backed finance, and structured products. APOLLOUSD amplifies the base ~3% ACRED yield through leverage on Morpho, targeting 9% net APY.

## GAIBVAULT

| Property | Value |
|---|---|
| Underlying | GAIB GPU Financing Notes |
| Target APY | 16.0% |
| Risk Profile | High |
| Redemption | 35-day (underlying), Instant via liquidity buffer |
| Leverage | Up to 2.5x |
| Collateral | GPU financing notes |
| Use Case | High-yield allocation, AI infrastructure exposure |

GAIB provides GPU financing notes backed by contracted compute revenue. GAIBVAULT offers the highest yield in the protocol but carries GPU utilization and counterparty risk.

## Yield Sources

| Source | Base Yield | After Leverage | Mechanism |
|---|---|---|---|
| US Treasuries (BUIDL) | 4.5% | 4.5% (no leverage) | Fed funds rate pass-through |
| Private Credit (ACRED) | ~3% | ~9% (3.33x) | Senior secured lending yield |
| GPU Financing (GAIB) | ~6.5% | ~16% (2.5x) | Contracted compute revenue |

## Fee Structure

| Fee | Amount | Recipient |
|---|---|---|
| Management fee | 0.5% AUM/year | Protocol treasury |
| Performance fee | 10% of yield | Protocol treasury |
| Entry/exit fee | 0% | — |
| Leverage spread | Variable | Morpho LPs |
