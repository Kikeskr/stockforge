# StockForge Portfolio Creation Logic

## 1. Purpose

This document defines how a user creates a StockForge portfolio from beginning to end.

## 2. Creation Flow

Connect Wallet
      |
      v
Create Portfolio
      |
      v
Enter Name
      |
      v
Add Supported Assets
      |
      v
Set Target Allocations
      |
      v
Validate Portfolio
      |
      v
Save Portfolio
      |
      v
Portfolio Status = DRAFT

## 3. Required Information

A portfolio requires:

- Portfolio name
- Portfolio description (optional)
- At least one supported asset
- Target allocation for every selected asset

## 4. Validation

The portfolio is validated before being saved for execution.

Validation includes:

- Name is present.
- At least one asset is selected.
- All selected assets are supported.
- No duplicate assets exist.
- All allocation weights are valid.
- Total allocation equals 100%.

## 5. Draft State

A newly created portfolio begins in:

DRAFT

The user can modify a draft before execution.

## 6. Execution

A valid draft can be submitted for execution.

The execution process will later interact with the Solana program and supported tokenized-stock infrastructure.

After successful execution:

DRAFT -> ACTIVE

## 7. Creation Principle

Portfolio creation should be simple enough that a user can create a complete investment strategy without needing to understand the underlying Solana transactions.
