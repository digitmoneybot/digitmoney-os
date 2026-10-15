# Yield Engine

Goal: Maximize **risk-adjusted real yield** while protecting capital.

## Opportunity Scoring Framework

Score every yield opportunity on these dimensions (0-10):

1. **Real Yield Quality** — Is the yield sustainable or mostly incentives?
2. **Smart Contract Risk** — Audit quality, time in production, complexity
3. **Liquidity Risk** — Can we exit quickly without major slippage?
4. **Opportunity Cost** — Compared to simply holding stables or ETH
5. **Impermanent Loss / Directional Risk**
6. **Gas & Operational Efficiency**

Only recommend opportunities that score well on the combination of the above.

## Preferred Yield Hierarchy (general)

1. High-quality lending / money markets (Aave, Morpho, etc. on major chains)
2. Sustainable real yield from trading fees or funding rates
3. Restaking / liquid restaking (with careful risk assessment)
4. Incentive-driven farming (only if risk is well understood and sized small)
5. Complex structured products (rare, high scrutiny)

## Auto-Compound Logic

- Compound when the expected value of compounding exceeds gas + opportunity cost
- Prefer less frequent compounding on smaller positions
- On larger positions, more active compounding is acceptable
- Always consider whether compounding increases smart contract exposure unnecessarily

## Output Format When Recommending Yield

Always present:
- Current best opportunity
- Estimated net APY (after fees/gas)
- Key risks (1-3 bullet points)
- Suggested allocation size
- Exit plan / monitoring triggers
