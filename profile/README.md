# Joinn

A web3 wealth management platform combining tokenized real-world asset investing with everyday spending through a VISA card.

[![Live App](https://img.shields.io/badge/app-joinn.io-blue)](https://app.joinn.io)
[![React](https://img.shields.io/badge/react-18-61DAFB?logo=react)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/typescript-5-3178C6?logo=typescript)](https://www.typescriptlang.org)
[![Vite](https://img.shields.io/badge/vite-646CFF?logo=vite)](https://vitejs.dev)

## Overview

Joinn is an RWA aggregation platform that unifies a fragmented tokenized asset market into a single, accessible hub. Users create non-custodial smart accounts through social login and gain access to institutional-quality RWA products across multiple EVM chains -- without needing blockchain expertise.

The platform pairs DeFi investing with real-world spending and a seamless web2 UX: invest in tokenized gold, corporate credit, treasury bills, and private credit vaults, then spend stablecoin balances directly with a Joinn Pay VISA card. Gasless transactions, cross-chain bridging, and an AI trading assistant make the experience seamless.

Joinn is non-custodial and non-discretionary -- users retain full ownership and control of their assets at all times. The platform is a Progressive Web App installable on both mobile and desktop.

## Features

### Multi-Chain Smart Accounts

Deploy and manage smart contract wallets across 6 EVM chains: Ethereum, Polygon, Base, Gnosis, Plume, and Injective. Account abstraction (ERC-4337) enables gasless, sponsored transactions with social login onboarding -- no seed phrases, no gas tokens, no complexity.

### RWA Investment Products

Access tokenized real-world assets through a unified interface:

| Asset | Type | Chain |
|-------|------|-------|
| PAXG | Physical Gold | Ethereum, Polygon |
| deJAAA | Corporate Credit CLO | Base |
| syrupUSDC | Maple Finance Yield | Base |
| cUSDO | OpenEden Staking | Ethereum |

**Nest Protocol Institutional Vaults** on Plume Network provide access to 8 additional RWA strategies:

| Vault | Strategy |
|-------|----------|
| nTBILL | US Treasury Bills |
| nALPHA | Diversified RWA Portfolio |
| nBASIS | Money Market Instruments |
| nINSTO | Institutional Fixed Income |
| nWISDOM | Private Credit |
| nOPAL | Credit Card Receivables |
| nMNRL | Oil & Gas Royalties |
| inALPHA | Alpha Vault LP |

### Joinn Pay VISA Card

Virtual and physical VISA cards funded from any supported chain. Spend in EUR, GBP, or USD stablecoins with full card management:

- Freeze/unfreeze cards
- Configurable daily and monthly spending limits
- Card replacement
- IBAN/BIC banking details via Monerium for inbound transfers
- Transaction history and spending analytics

### AI Trading Agent

Conversational trading interface which a execute trades, fund your card, and explore investment products using natural language:

- *"Buy 100 PAXG"*
- *"Deposit 500 USDC to my card"*
- *"Tell me about nTBILL"*

The agent handles cross-chain bridging, DEX routing, and execution autonomously with a confirmation step before every trade.

## Current Supported Chains

| Chain | ID | Smart Accounts | Swapping | Bridging |
|-------|----|:-:|:-:|:-:|
| Ethereum | 1 | ✓ | ✓ | ✓ |
| Polygon | 137 | ✓ | ✓ | ✓ |
| Base | 8453 | ✓ | ✓ | ✓ |
| Gnosis | 100 | ✓ | -- | ✓ |
| Plume | 98866 | ✓ | -- | ✓ |
| Injective | 1776 | ✓ | ✓ | ✓ |

## Security

- **Non-custodial** -- All wallets are ERC-4337 smart contract accounts owned solely by the user
- **SIWE Authentication** -- Sign-In With Ethereum with EIP-712 typed data signing
- **KYC/AML Compliance** -- Identity verification gating for VISA product access
- **Geo-blocking** -- IP geolocation enforcement for sanctioned regions
- **Session Management** -- Cross-tab synchronization with automatic token refresh

## Roadmap

- **Stock Token Vault** -- Automated vault maintaining target ratios of RWAs to stablecoin reserves with automated rebalancing strategies
- **Property-Backed Digital Credit** -- Unlock property equity through integration with banking partners

See the [Yield-Fi organization profile](https://github.com/Yield-Fi) for the broader platform vision.

## License

Proprietary. All rights reserved.

