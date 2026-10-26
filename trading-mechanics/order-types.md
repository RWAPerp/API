# Order Types

RWAPerp is a decentralized exchange (DEX) that supports Limit, Market, Immediate-or-Cancel (IOC), Fill-or-Kill (FOK), and Post-Only order types, along with Reduce-Only instructions.



Orders are submitted through the RWAPerp frontend to its shared order book, processed by the underlying off-chain matching engine, with real-time order and fill status updates via WebSocket.

<table data-header-hidden data-search="false"><thead><tr><th></th><th></th></tr></thead><tbody><tr><td>Order Type</td><td>Description</td></tr><tr><td>Limit</td><td>Executes at the specified or better price. Supports GTC (Good-till-Cancelled) and GTD (Good-till-Date).</td></tr><tr><td>Market</td><td>Executes immediately at the best available price. Speed is guaranteed, price is not.</td></tr><tr><td>IOC (Immediate-or-Cancel)</td><td>Fills the available portion immediately; the remainder is automatically cancelled and does not enter the order book.</td></tr><tr><td>FOK (Fill-or-Kill)</td><td>Must be filled entirely or cancelled entirely. No partial fills.</td></tr><tr><td>Post-Only</td><td>Guarantees maker status; cancelled if it would immediately take liquidity. Used to earn maker rebates.</td></tr><tr><td>Reduce-Only</td><td>Only reduces an existing position; cannot open a new position in the opposite direction. Typically used with take-profit and stop-loss orders.</td></tr></tbody></table>
