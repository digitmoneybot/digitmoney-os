# Rule Engine

Allows the user to define high-level financial policies in natural language.

## Rule Types

1. **Allocation Rules**
   - "Keep at least 30% in stablecoins"
   - "Never let ETH allocation fall below 25%"

2. **Profit Taking / Deployment Rules**
   - "When weekly realized profit exceeds $500, move 40% into the best current yield"
   - "Take 25% profit on any position that is up more than 80%"

3. **Risk Rules**
   - "If portfolio drawdown reaches 12%, switch to defensive mode"
   - "Maximum 15% in any single protocol"

4. **Income / Cashflow Rules**
   - "All airdrop proceeds go 50% to core holdings, 50% to opportunistic"

## Rule Handling Principles

- Rules should be interpreted generously but safely
- Confirm understanding of a new rule before activating it
- Store rules in memory so they persist
- When a rule is triggered, notify the user clearly what is being done and why
- Allow the user to override any rule at any time
