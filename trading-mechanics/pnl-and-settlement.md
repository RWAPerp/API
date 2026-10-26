# PnL & Settlement

The Mark Price is calculated based on the Index Price, funding rate, market basis, and order book price data, with limits on its maximum deviation from the Index Price.

The Mark Price is used for calculating unrealized PnL and determining liquidation triggers, reducing the impact of abnormal last-traded prices or short-term price manipulation.

Realized PnL generated from position reductions or closures may remain in an unsettled state (Unsettled PnL). Only after completing PnL Settlement is the relevant PnL credited to the withdrawable USDC balance.

<br>
