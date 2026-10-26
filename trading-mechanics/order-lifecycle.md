---
description: >-
  Replace your auto-generated subdomain with your own domain, with automatic
  SSL.
---

# Order Lifecycle

The lifecycle of a trade on RWAPerp follows a transparent, on-chain verifiable path:



1. Place: The client submits an order via REST API or SDK. The system verifies the account identity and trading permissions using the account-authorized trading key and Ed25519 request signature.
2. Validate: The trading and risk engine connected to RWAPerp validates available collateral, initial margin, minimum notional, price and quantity precision, order size limits, and price protection ranges. Orders that fail validation are rejected.
3. Enter Order Book: Validated orders enter the shared order book connected to RWAPerp. Limit orders wait in the book for matching; Market, IOC, and FOK orders proceed to matching immediately per their execution rules.
4. Match: The underlying matching engine matches orders according to order book rules. Fill records are generated upon matching between Maker and Taker.
5. Fill Confirmation: The system pushes order and fill updates via WebSocket, including fill price, quantity, fees, order status, and remaining quantity.
6. Settlement: The system updates account position, average entry price, realized and unrealized PnL, fees, and margin information. Trade results are settled through the underlying settlement network connected to RWAPerp; deposits and withdrawals are processed through the relevant asset contracts on supported chains.



Signing Method: Standard trading requests use Ed25519 signatures. EIP-712 is primarily used for account registration, adding trading keys, withdrawals, and initiating PnL Settlement.

<br>
