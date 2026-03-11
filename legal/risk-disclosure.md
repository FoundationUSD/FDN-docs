# Risk Disclosure Statement

> **DRAFT — Requires legal review before publication.**

## Important Notice

Using Foundation Protocol involves significant risks. You should not deposit funds you cannot afford to lose. This document outlines — but does not exhaustively cover — the risks associated with using the Protocol.

## Smart Contract Risk

Foundation Protocol relies on smart contracts deployed on public blockchains. Despite testing and planned audits, smart contracts may contain bugs or vulnerabilities that could result in partial or total loss of deposited funds. Smart contracts are immutable once deployed (upgradeable via proxy, but subject to governance constraints).

## Oracle Risk

Vault share prices are determined by oracle price feeds. Oracle manipulation, staleness, or failure could result in incorrect share pricing, enabling arbitrage at the expense of other depositors, or preventing withdrawals at fair value.

## Credit Risk

Underlying assets carry counterparty and credit risk:
- **BUIDL (BlackRock)**: US Treasury exposure — considered low risk but not risk-free
- **ACRED (Apollo)**: Private credit — subject to corporate default risk
- **GAIB GPU Notes**: GPU financing — subject to technology and counterparty risk

## Liquidity Risk

Instant redemptions depend on the availability of USDC in each vault's liquidity buffer. When the buffer is depleted, withdrawals are queued and settled when underlying assets redeem. Settlement times vary: 1–7 days (BUILDVAULT), quarterly (APOLLOUSD), up to 35 days (GAIBVAULT).

## Leverage Risk

Leveraged vault positions (APOLLOUSD, GAIBVAULT) are subject to liquidation if the health factor drops below the threshold. Rapid price movements or oracle delays can result in liquidation losses.

## Regulatory Risk

The regulatory environment for DeFi and tokenized securities is evolving. Changes in law or enforcement could restrict access to the Protocol, require KYC for all users, or mandate cessation of operations in certain jurisdictions.

## Bridge Risk

Cross-chain transactions via LayerZero or other bridges introduce additional risk including bridge contract vulnerabilities, message relay failures, and delayed finality.

## No Guarantee of Returns

Target APY figures are estimates based on current underlying asset yields and market conditions. Actual returns may be higher or lower. Past performance is not indicative of future results.

## Protocol Governance

The Protocol is currently managed by a multi-sig controlled by the core team. Governance decentralization is planned but not guaranteed.

## Acknowledgment

By using Foundation Protocol, you acknowledge that you have read and understood these risks and accept full responsibility for your financial decisions.

---

*This document is a template and must be reviewed by qualified legal counsel before publication.*
