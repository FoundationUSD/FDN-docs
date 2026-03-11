# Audit Status

## Current Status: Not Audited

Foundation Protocol smart contracts have **not yet been audited**. The protocol is currently deployed on **Sepolia testnet only** and has not launched on mainnet.

An audit will be conducted before any mainnet deployment.

## Contracts in Scope

| Contract | Description |
|---|---|
| `FdnVault.sol` | ERC-4626 vault — deposits, share minting, NAV-based yield |
| `FdnRouter.sol` | Multi-vault deposit routing |
| `FdnOracle.sol` | NAV price oracle with deviation bounds |
| `FdnLiquidity.sol` | Instant-redemption buffer with queue fallback |
| `FdnRegistry.sol` | Vault registry, fee config, admin roles |
| `FdnKYC.sol` | KYC whitelist (scaffold) |
| `FdnLeverage.sol` | Morpho leverage module (scaffold, not implemented) |

## Test Coverage

- 41 unit tests passing (Foundry)
- Solidity 0.8.24, OpenZeppelin v4.9.6, UUPS upgradeable

## Audit Reports

*None yet. This section will be updated when audits are completed.*

<!--
When adding a report, use this format:

### [Auditor Name] — [Month Year]
- **Scope**: [contracts audited]
- **Findings**: [X critical, X high, X medium, X low]
- **Report**: [link to PDF]
- **Status**: [all resolved / X outstanding]
-->
