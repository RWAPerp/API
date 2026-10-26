---
description: >-
  React to deploys, comments, and external events with workflows that run on the
  platform.
---

# Account & Margin Metrics

RWAPerp uses Cross Margin mode by default. For markets that support Isolated Margin, traders may also select Isolated Margin mode when placing orders.

The Maintenance Margin Rate is dynamically calculated based on market base parameters and position notional value:

```
MMR_i = max(
  Base MMR_i,
  (Base MMR_i / Base IMR_i)
    × IMR Factor_i
    × |Position Notional_i|^(4/5)
)
```

As position notional value increases, the effective Maintenance Margin Rate may increase, reducing the effective maximum leverage for large positions.

Base IMR, Base MMR, IMR Factor, maximum leverage, and maximum position notional for each market are subject to adjustment. Refer to the real-time parameters displayed on the RWAPerp trading interface.

\
<br>
