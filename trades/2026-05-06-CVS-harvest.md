# Harvest Action: CVS

**Date:** 2026-05-06
**Action:** PROGRESSIVE_STOP_ADVANCE (no trim)
**Triggered by:** Mercury triple-bull-stack pre-market — Q1 EPS BEAT (+16.8%) + Adj EPS guide RAISED + GAAP EPS guide RAISED. Tape +8.75% intraday at decision time. HELD POSITION (27 sh).

## Trade Details

| Field | Value |
|-------|-------|
| Entry (avg) | $75.8286 |
| Current shares | 27 |
| Shares trimmed | 0 (stop-advance only) |
| Shares remaining | 27 |
| Current price (decision time) | $87.75 (+15.7% on cost) |
| Old stop | $75.83 (breakeven from 2026-04-30 harvest) |
| New stop | $82.00 (locks +$166.59 = +8.1% above entry) |

## Pre-trade math
- Position locked at breakeven since 2026-04-30 harvest
- This morning Q1 cycle: print BEAT + Adj EPS guide $7.30-$7.50 (vs $7.16 est, midpoint +3.4%) + GAAP EPS guide $6.24-$6.44 (vs $5.84 est, midpoint +8.6%)
- Tape: $87.75 = +$11.92 from entry, +$11.92 / new $82 stop = -6.5% trail
- Conservative locking +8% above entry; preserves +50% of unrealized $11.92/sh while leaving room for normal volatility

## Order IDs

| Order | ID | Status |
|-------|-----|--------|
| Cancel old stop ($75.83) | 6e28cfdf-1583-4386-ae24-b61a3c2e7dbb | Canceled |
| New Stop ($82.00, 27 sh) | da7b717e-e162-4cb6-852e-e06df72806dc | Accepted |

## Rationale
Triple-positive Q1 cycle (print + 2 guide raises) on a held-position. Stop at breakeven was leaving all of the +8.75% intraday gain unprotected. Advancing to $82 locks meaningful gain while trail (-6.5%) is still wide enough to weather typical post-earnings volatility. Phase 0.5 / Reaper at next autopilot run can decide whether to advance further.
