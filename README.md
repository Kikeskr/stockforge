# StockForge

**Forge your portfolio. Own it on-chain.**

StockForge is a Solana-based platform for creating programmable investment portfolios from tokenized stocks.

## Core Idea

Users can create custom stock baskets, define allocations, fund them with USDC, and manage the portfolio on-chain.

## Core Wedge

Custom programmable portfolios built from tokenized stocks on Solana.

## Planned Stack

- Frontend: Next.js + TypeScript
- Backend: Python + FastAPI
- Database: Supabase / PostgreSQL
- Blockchain: Solana
- Smart Contract: Rust + Anchor
- Price Feeds: Pyth
- Wallet: Solana Wallet Standard
- Deployment: Vercel

## Development

StockForge is currently being built for the Solana Stocklana hackathon.

**Network:** Solana Devnet

## Project Structure

```text
stockforge/
├── apps/
│   ├── web/
│   └── api/
├── packages/
│   ├── solana/
│   ├── pyth/
│   └── markets/
├── programs/
│   └── stockforge/
├── docs/
└── README.md