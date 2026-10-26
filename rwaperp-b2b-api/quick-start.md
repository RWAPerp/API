---
description: Install dependencies and run the end-to-end example.
---

# Quick start

Complete account onboarding before running the trading example. The onboarding process creates the trading account and returns the API credentials required below.

> **Production environment:** Default REST is `https://api-trade.rwaperp.xyz`. If your integration is provisioned for VIP, use `https://api-vip.rwaperp.xyz` (same paths and `RWA-*` signing). The default command performs read-only queries. The `--with-order` option submits and cancels a real order using real account funds.

```bash
pip install eth-account base58 cryptography pynacl websocket-client
export RWA_ACCOUNT_ID="0x..."
export RWA_API_KEY="ed25519:..."
export RWA_SECRET_B58="..."
# Optional VIP host:
# export B2B_API_BASE="https://api-vip.rwaperp.xyz"
# After saving the trading example as trading-mainline.py:
python3 trading-mainline.py
python3 trading-mainline.py --with-order   # submits and cancels a real order; requires sufficient USDC
```

**Chain restriction: X Layer only (`chainId = 196`). No other chain is supported.** Do not use Avalanche, Arbitrum, Base or any other `CHAIN_ID` when opening an account or binding a key.

| What you need                      | Section            |
| ---------------------------------- | ------------------ |
| Trading workflow and sample script | Trading workflow   |
| RWA request signing                | Request signing    |
| Response format                    | REST API overview  |
| Complete endpoint documentation    | REST API reference |
| Withdrawals                        | Withdrawals        |

Trading pairs: `PERP_{BASE}_{QUOTE}` (e.g. `PERP_ETH_USDC`).
