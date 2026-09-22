cat > docs/portfolio-structure.md <<'EOF'
# StockForge Portfolio Structure

## 1. Portfolio Definition

A StockForge portfolio is a user-defined basket of tokenized stocks with target allocation weights.

Each portfolio has:

- An owner
- A unique portfolio ID
- A name
- A description
- A collection of stock allocations
- A target allocation for each stock
- A current portfolio value
- A lifecycle status
- Creation and update timestamps

---

## 2. Portfolio Example

```text
AI Infrastructure

Owner: <wallet>

Assets:
    NVDA   35%
    MSFT   25%
    GOOGL  20%
    AMD    20%

Total Allocation: 100%
Status: ACTIVE