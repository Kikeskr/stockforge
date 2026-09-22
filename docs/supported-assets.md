# StockForge Supported Assets

## 1. Purpose

StockForge portfolios are composed of supported tokenized stock assets.

An asset must be registered and active before it can be added to a portfolio.

## 2. Asset Information

Each supported asset contains:

- `id`
- `symbol`
- `name`
- `token_address`
- `price_feed`
- `decimals`
- `is_active`

## 3. MVP Asset Requirements

Each asset must have:

1. A unique identifier.
2. A stock symbol.
3. A token representation on Solana.
4. A configured price feed.
5. Known token decimals.
6. An active/inactive status.

## 4. Asset Validation

Before adding an asset to a portfolio, StockForge checks:

- Asset exists.
- Asset is active.
- Token address is valid.
- Price feed is configured.
- Asset is not already present in the portfolio.

## 5. Initial Asset Set

The MVP should begin with a small curated set of tokenized stocks rather than attempting to support every available asset.

Example:

```text
NVDA
MSFT
GOOGL
AMD