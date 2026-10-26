---
description: Roles, permissions, and how access flows from workspace to project.
---

# RWA Pricing & Trading Hours

Because real-world assets (such as equities) trade only during their native market hours, while perps run 24/7, off-hours pricing is handled explicitly:<br>

* Price source: the reference (index) price is aggregated from multiple oracle price feeds. Outlier protection is built in — a feed that strays too far from the consensus of the others is pulled back toward it, and a feed that stops updating is dropped from the calculation until it recovers.&#x20;
* Market open: the index price tracks live market data.
* Market closed (nights, weekends, holidays): the index price is frozen at the last close, and the system automatically widens the allowed deviation between mark price and index price to accommodate reduced liquidity and a wider basis.
* Gap risk: the underlying market can re-open far from where it closed. Positions held across a close may see sudden changes in unrealized PnL — and liquidation risk — at the next open, so size positions with this in mind.

<br>

This directly affects mark price, funding, and liquidation (see those sections).

<br>
