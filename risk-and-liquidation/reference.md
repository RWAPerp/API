# Reference

### Liquidation

#### Trigger Condition

A liquidation is triggered when the Account Margin Ratio (AMR) falls below the Maintenance Margin Ratio (MMR):

account\_margin\_ratio < maintenance\_margin\_ratio

RWAPerp uses the Mark Price to determine whether liquidation is triggered. The Maintenance Margin Ratio changes dynamically based on market parameters and position size.

#### Liquidation Price

The liquidation price is calculated by the RWAPerp risk engine based on total account collateral, all positions, the Mark Price, dynamic margin requirements, and unsettled PnL. Refer to the estimated liquidation price displayed on the RWAPerp trading interface.

#### Liquidation Process

1\. Trigger: The system detects that the account margin ratio has fallen below the maintenance margin ratio.

2\. Cancel & Freeze: The system cancels all open orders for the account and freezes withdrawals, transfers, and other operations.

3\. Partial Liquidation: The system calculates the position size that needs to be liquidated to restore the account margin ratio to the Initial Margin Ratio (IMR).

4\. Liquidator Takeover: Qualified liquidators with sufficient collateral may take over the liquidated position at a discount per system rules. RWAPerp typically does not sell the entire position directly into the order book.

5\. Insurance Fund Backstop: If the account is insolvent, or the remaining collateral is insufficient to cover liquidation costs, unprocessed positions and debt may be transferred to the insurance fund.

<br>
