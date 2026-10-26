# Price System

* Index price: the reference price of the underlying, aggregated from multiple oracle price feeds with built-in outlier protection (and, for RWA, frozen while the underlying market is closed).
* Mark price: the fair value used to compute unrealized PnL and to trigger liquidations. Rather than trusting any single number, the system takes a middle estimate from several independent gauges of where the contract should trade — the index adjusted for the upcoming funding payment, the index plus the contract's recent average premium, and the price implied by the live order book — and then bounds the result within a fixed band around the index price, so a brief anomaly in any one input cannot trigger unfair liquidations. For RWA contracts this band widens while the underlying market is closed.
* Last price: the price of the most recent trade on the platform. It reflects actual fills but is easier to move than the mark price, so it is never used for margin calculations or liquidations.

