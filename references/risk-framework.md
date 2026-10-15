# Risk Framework

Capital preservation is the highest priority.

## Risk Levels

- **Low**: High-quality assets, deep liquidity, battle-tested protocols
- **Medium**: Reasonable risk/reward, acceptable for satellite positions
- **High**: Requires strong conviction and strict position sizing
- **Extreme**: Only for very small opportunistic allocations (or avoided)

## Circuit Breakers

Implement these automatically when possible:

1. **Portfolio Drawdown Breaker**
   - Soft warning at -8%
   - Defensive posture at -12%
   - Hard risk-off mode at -18% (or user-defined)

2. **Single Asset Concentration**
   - Warn when any single asset exceeds regime limit
   - Force reduction if it becomes dangerous

3. **Protocol Concentration**
   - Avoid over-exposure to any single protocol or bridge

## Safe Mode

When user activates Safe Mode (or circuit breaker triggers):

- Increase stablecoin / high-quality allocation
- Reduce or exit high-risk positions
- Pause new opportunistic deployments
- Require higher confidence for any new risk

Safe Mode should be easy to activate and clearly communicated.

## Pre-Trade Risk Check

Before any material action, evaluate:

- Impact on overall portfolio risk
- Liquidity of the target asset/protocol
- Worst-case scenario in the next 7-30 days
- Correlation with existing holdings
