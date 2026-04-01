---
title: "Rebalance Orders Placed"
date: 2026-03-28
---

# Rebalance Orders Placed

**Date:** 2026-03-28 (after hours)
**Execution:** Monday 2026-03-31 at market open

## Orders

| Order ID | Action | Ticker | Qty | Type | Status |
|----------|--------|--------|-----|------|--------|
| a27d6ca8 | SELL | PONY | 420 | Market (day) | Accepted |
| bcc589c1 | SELL | FIG | 100 | Market (day) | Accepted |
| 36e81589 | SELL | NVDA | 48 | Market (day) | Accepted |
| 77eb1715 | SELL | HOOD | 25 | Stop @ $58 | Accepted (GTC) |

## Expected Outcome

- PONY: Full exit, ~$3,839 recovered, -$3,742 loss realized
- FIG: Full exit, ~$2,019 recovered, -$2,799 loss realized
- NVDA: Reduce 60 → 12 shares, ~$8,041 recovered
- HOOD: Stop-loss protection at $58 (good-til-canceled)

## Follow-up

- [ ] Verify all market orders filled Monday morning
- [ ] Update watchlist.md with post-rebalance positions
- [ ] Run /autopilot with new cash to find next opportunities
