# Portfolio Engine

This module is responsible for intelligent capital allocation and rebalancing.

## Risk Regimes

| Regime        | Description                          | Typical Allocation Style                  | Max Single Position |
|---------------|--------------------------------------|-------------------------------------------|---------------------|
| Conservative  | Capital preservation first           | High stables + bluechips                  | 15-20%             |
| Balanced      | Growth with strong downside control  | Core + moderate satellite                 | 20-25%             |
| Growth        | Higher expected return               | Higher beta + selective yield             | 25-30%             |
| Opportunistic | Asymmetric bets allowed              | Core + high-conviction satellites         | 30-35%             |
| Custom        | User-defined                         | Fully flexible                            | User-defined       |

## Portfolio Sleeves

Always think in sleeves:

- **Core** (40-70%): Highest conviction, lowest risk assets (ETH, BTC, major stables, high-quality LSTs)
- **Satellite** (15-40%): Higher expected return strategies (selective yield, mid-cap, thematic)
- **Opportunistic** (0-20%): High asymmetry, smaller size
- **Cash / Dry Powder** (5-25%): Stablecoins ready for deployment

## Rebalancing Logic

Do **not** rebalance mechanically on schedule.

Rebalance when:
1. Allocation drift exceeds threshold (default 5-7% absolute)
2. Market regime has clearly changed
3. A better risk-adjusted opportunity appears
4. User explicitly requests it
5. Risk limits are approached

When rebalancing:
- Prefer selling into strength and buying into relative weakness
- Minimize unnecessary transactions
- Always show before/after allocation and expected impact

## Position Sizing Principles

- Size is a function of conviction × liquidity × risk
- Never size a position so large that a 30-40% drawdown in that asset threatens the whole portfolio
- Prefer scaling in over all-in entries on new ideas
