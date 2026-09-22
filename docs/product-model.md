# StockForge Product Model

## 1. Product

StockForge allows users to create programmable investment portfolios from tokenized stocks on Solana.

Core idea:

> Forge your portfolio. Own it on-chain.

---

## 2. Core Entities

StockForge MVP is built around five core entities:

- User
- Portfolio
- Portfolio Asset
- Stock Asset
- Transaction

---

## 3. User

Represents a wallet user interacting with StockForge.

### Fields

- `wallet_address`
- `created_at`

The wallet address is the primary identity for the MVP.

---

## 4. Portfolio

Represents a user-created investment strategy.

### Fields

- `id`
- `owner`
- `name`
- `description`
- `total_value`
- `status`
- `created_at`
- `updated_at`

### Example

```text
Portfolio
Name: AI Infrastructure
Owner: <wallet>
Status: ACTIVE