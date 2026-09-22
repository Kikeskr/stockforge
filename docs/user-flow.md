# StockForge End-to-End User Flow

## 1. Product Flow

Connect Wallet
      |
      v
Create Portfolio
      |
      v
Name Portfolio
      |
      v
Select Supported Stocks
      |
      v
Set Allocations
      |
      v
Validate Portfolio
      |
      v
Save Draft
      |
      v
Fund Portfolio
      |
      v
Execute on Solana
      |
      v
Portfolio Becomes Active
      |
      v
Track Portfolio Value
      |
      v
Monitor Allocation
      |
      v
Rebalance When Needed
      |
      v
Continue Managing Portfolio

## 2. Detailed Flow

### Step 1 — Connect Wallet

The user connects a compatible Solana wallet.

The wallet becomes the user's StockForge identity.

### Step 2 — Create Portfolio

The user chooses:

- Portfolio name
- Description
- Stocks
- Target allocations

### Step 3 — Validate

StockForge checks:

- Supported assets
- Duplicate assets
- Allocation values
- Total allocation
- Portfolio completeness

### Step 4 — Save

The portfolio is stored as a draft.

Status: DRAFT

### Step 5 — Fund

The user supplies the required funds for execution.

The MVP uses USDC as the intended funding asset.

### Step 6 — Execute

The user reviews the portfolio and confirms the transaction.

The wallet signs the required Solana transaction(s).

### Step 7 — Active Portfolio

After successful execution:

DRAFT -> ACTIVE

The portfolio now represents the user's active investment strategy.

### Step 8 — Monitor

StockForge displays:

- Portfolio value
- Asset values
- Target allocations
- Current allocations
- Allocation differences
- Transaction history

### Step 9 — Rebalance

When allocations drift from their targets, the user can request a rebalance.

StockForge generates a proposed rebalance plan.

The user reviews and confirms it.

### Step 10 — Transaction Confirmation

The wallet signs the rebalance transaction(s).

StockForge updates the portfolio state after successful confirmation.

## 3. MVP User Journey

Connect
  ↓
Forge
  ↓
Fund
  ↓
Execute
  ↓
Own
  ↓
Monitor
  ↓
Rebalance

## 4. Product Principle

Every major action should have a clear user-visible state and, where applicable, an associated Solana transaction.

The user should always understand:

1. What they are doing.
2. What assets are involved.
3. What allocation they are creating.
4. What transaction they are signing.
5. What the resulting portfolio state is.
