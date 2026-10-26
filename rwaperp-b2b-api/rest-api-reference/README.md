# REST API reference



Base URL: `https://api-trade.rwaperp.xyz` (default). Dedicated VIP REST: `https://api-vip.rwaperp.xyz` (same paths and `RWA-*` signing). This reference contains **147** endpoints grouped by domain. Open an endpoint from the tables below to view its parameters, request body, response fields, authentication requirement, and rate limit.

Schemas are adapted from the published API specification supplied for this integration. RWA Perp's base URL, `RWA-*` authentication headers, X Layer restriction, and RWA-specific signing flows are authoritative for this document.

Three RWA-specific operations—`POST /v1/public/query`, `POST /v1/register_dex_account`, and `POST /v1/dex_api_key`—are documented in the local integration guides.

General request and response conventions are documented in the REST API overview.

* **Auth = None**: call directly
* **Auth = RWA**: see request signing
* **Auth = Wallet**: `register_dex_account` / `dex_api_key`
* **Auth = Wallet + RWA**: `withdraw_request` (Withdrawals)

| Section                           | Count |
| --------------------------------- | ----- |
| Public market data                | 33    |
| Candles and TradingView           | 5     |
| Trading and orders                | 28    |
| Positions and leverage            | 14    |
| Account                           | 15    |
| Funds and settlement              | 18    |
| Account registration and API keys | 2     |
| Strategy Vault                    | 6     |
| Staking and Valor                 | 11    |
| Volume statistics                 | 3     |
| Notifications                     | 4     |
| Liquidator                        | 1     |
| Other endpoints                   | 7     |
| Out of scope                      | —     |

For public GET endpoints, replace `{symbol}` with a value such as `PERP_ETH_USDC`.
