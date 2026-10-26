# Margin Modes

* Cross margin (default): Your USDC collateral is shared across all cross positions. Profit in one position can offset loss in another, and margin is measured at the account level.
* Isolated margin: Each position receives its own dedicated margin. Loss is capped at that position's margin and does not affect the rest of your account. You can add margin to or remove margin from an isolated position at any time.
* Per-order choice: You choose the margin mode when placing each order. The two modes are independent — you can hold a cross position and an isolated position on the same contract simultaneously, each with its own margin and liquidation price.

