# Funding Fee (Mechanics)

The funding rate mechanism keeps the perpetual contract price near the underlying Index Price. Funding fees are periodically calculated and exchanged between long and short position holders.

The funding period may be 1 hour, 4 hours, or 8 hours. The specific period, rate caps, and rate floors are subject to adjustment based on market conditions.

| Parameter           | Description                                                                                      |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| Settlement Interval | May be 1 hour, 4 hours, or 8 hours, configured per market conditions                             |
| Payment Direction   | Longs pay Shorts when rate > 0; Shorts pay Longs when rate < 0                                   |
| Rate Cap / Floor    | Adjusted per market conditions; refer to real-time data on the trading interface                 |
| Fee Settlement      | Funding fees are credited to the account's unsettled PnL and settled upon PnL Settlement trigger |

<br>

Traders can view the current funding rate, next settlement time, and estimated funding fee on the RWAPerp trading interface.

<br>
