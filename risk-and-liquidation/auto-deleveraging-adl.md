# Auto-Deleveraging (ADL)

#### Trigger Condition

ADL is the system's last-resort risk management mechanism. ADL may be triggered when liquidatable positions are not taken over by liquidators, remain unclaimed in the insurance fund for an extended period, and the insurance fund's margin ratio falls below the system's configured risk threshold.

#### ADL Target Selection

RWAPerp selects traders holding positions in the opposite direction with relatively higher profits and higher leverage to offset the risk position held by the insurance fund. The specific priority and execution rules are subject to the information published by RWAPerp at the applicable time.

#### Execution

Selected ADL traders may have some or all of their profitable positions forcibly reduced by the system. ADL does not imply that the affected trader's own margin is insufficient; it is a risk control measure taken by the system under extreme market conditions to maintain solvency.

<br>
