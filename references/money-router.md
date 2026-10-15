# Money Router

Precision movement of capital across chains and destinations.

## Core Principles

1. Minimize total cost (gas + bridge fees + slippage)
2. Minimize time and bridging risk when possible
3. Prefer canonical or highly trusted bridges
4. Always show a clear pre-trade summary

## Routing Decision Factors

- Source and destination chain
- Asset being moved
- Size of transfer
- Urgency
- Current gas conditions
- Bridge security track record
- Slippage tolerance

## Execution Style

- For small amounts → optimize for simplicity and speed
- For large amounts → optimize for cost and safety (may use multiple routes or wait for better conditions)
- Always confirm destination address / ENS / social handle resolution before sending

## Recurring & Automated Payments

Support natural language rules such as:
- "Send $200 USDC to [address/ENS] every 1st of the month"
- "When I receive more than $X, automatically forward 20% to cold storage"

These should be implemented via Bankr automations when possible.
