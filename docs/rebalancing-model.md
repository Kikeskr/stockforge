# StockForge Rebalancing Model

## 1. Purpose

Rebalancing adjusts a portfolio when its current asset weights differ from the user's target allocations.

## 2. Target vs Current Weight

Example target:

NVDA   35%
MSFT   25%
GOOGL  20%
AMD    20%

After market movement, the current allocation might become:

NVDA   42%
MSFT   23%
GOOGL  19%
AMD    16%

The portfolio is now different from its target structure.

## 3. Rebalance Condition

A rebalance can be requested when the current allocation differs from the target allocation.

Allocation Difference = Current Weight - Target Weight

Example:

NVDA
Current: 42%
Target: 35%
Difference: +7%

## 4. Rebalancing Process

Read Current Portfolio
        |
        v
Fetch Current Asset Prices
        |
        v
Calculate Current Weights
        |
        v
Compare With Target Weights
        |
        v
Calculate Required Changes
        |
        v
Generate Rebalance Plan
        |
        v
User Confirms
        |
        v
Execute Transactions
        |
        v
Update Portfolio State

## 5. Rebalance Plan

Before execution, StockForge should display the proposed changes.

Example:

Rebalance Plan

NVDA
Current: 42%
Target: 35%
Action: Reduce

MSFT
Current: 23%
Target: 25%
Action: Increase

GOOGL
Current: 19%
Target: 20%
Action: Increase

AMD
Current: 16%
Target: 20%
Action: Increase

## 6. User Confirmation

A rebalance should require user confirmation before transactions are submitted.

## 7. MVP Scope

The MVP should support manual user-triggered rebalancing.

Automatic scheduled rebalancing is outside the initial MVP unless implementation time permits.

## 8. Rebalancing Principle

Rebalancing should preserve the user's target portfolio structure while minimizing unnecessary transactions.
