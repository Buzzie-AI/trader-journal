# Trade: NFLX Sell — Autopilot Reaper 2026-04-21

**Strategy:** reaper-exit (thesis-break confirmed)
**Source:** autopilot manual run (09:52 ET), Phase 0 Reaper

## Thesis Break Sequence

Two-day confirmed thesis break:
1. **2026-04-20 14:18 ET (Mercury stream):** Reed Hastings exit announced + soft Q1 guidance preview — first RED signal
2. **2026-04-21 07:29 ET (poll follow-on):** Netflix Drops on Weak Guidance Despite Strong Q1 Results — thesis break fully confirmed

## Reaper Decision

- Position: 22 shares @ avg $97.00 entry, cost basis $2,134
- Current price: $93.97 (intraday -0.79%, vs entry -3.1%)
- Existing stop: $93.50 GTC (cushion $0.47 = 0.5%)
- Thesis now formally broken. Don't let cushion get chewed up during intraday noise.

## Execution

1. **Cancelled:** existing $93.50 stop order (id `f8eeab05-616c-414d-9320-420d39f4db35`)
2. **Placed:** limit sell 22 sh @ $93.50 day-TIF (order id `c9a10633-28e2-4ec3-b005-c92dedc13c5d`)
3. Limit at $93.50 with current bid $93.96 = fills immediately at bid (~$93.96)

## Safety Gates

| Gate | Value | Status |
|------|-------|--------|
| Daily trade cap (2) | 1 used (this sell) | ✓ |
| Circuit breaker (-8%) | portfolio +0.11% | ✓ |
| PDT same-day | NFLX bought days ago, not same-day | ✓ |
| Limit order | Yes ($93.50) | ✓ |

## P&L (at fill ~$93.96)

- Proceeds: ~$2,067
- Cost basis: $2,134
- Realized loss: ~**-$67** (-3.1%)
- vs. Stop-at-$93.50: saved $0.46/share × 22 = **+$10 vs letting the stop catch naturally**

## Post-Sale Portfolio Impact

- Cash moves: $4,520 → ~$6,583
- Open positions reduced from 11 → 10 (stocks: 9, crypto: 1, + 737CVR019 corporate-action)
- NFLX thesis chapter closed. No re-entry plan unless catalyst reverses (unlikely given management-succession + guidance-cut combo).
