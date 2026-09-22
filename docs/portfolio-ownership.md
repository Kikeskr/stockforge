# StockForge Portfolio Ownership Model

## 1. Ownership Identity

The connected Solana wallet is the primary identity of a StockForge user.

Wallet Address = User Identity

## 2. Portfolio Ownership

Every portfolio belongs to exactly one owner.

Portfolio
    |
    └── owner
          |
          └── Wallet Address

## 3. Ownership Rules

The owner can:

- Create portfolios.
- Modify draft portfolios.
- Execute eligible portfolios.
- View portfolio information.
- Request supported portfolio actions.
- Close their portfolio.

## 4. Wallet Verification

Actions that change portfolio state must be authorized by the portfolio owner's wallet.

The application must not rely only on a frontend-provided wallet address.

## 5. On-Chain Ownership

The Solana program will enforce ownership for on-chain portfolio state.

The connected wallet must sign transactions requiring authorization.

## 6. Ownership Transfer

Portfolio ownership transfer is outside the MVP scope.

The MVP assumes:

One portfolio -> One owner

## 7. Privacy

The wallet address is publicly visible on Solana.

StockForge should avoid storing unnecessary personal information when a wallet address is sufficient for the product.
