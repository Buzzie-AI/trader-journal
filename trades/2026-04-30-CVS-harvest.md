# Trade — 2026-04-30 CVS harvest (breakeven-lock)

## Order details
- **Symbol:** CVS
- **Action:** STOP REPLACEMENT (breakeven-lock)
- **Old stop:** $72.08 GTC
- **New stop:** $75.83 GTC (= entry $75.8286 rounded)
- **Replaced order ID:** bbf3316e-0e1b-42ae-a336-9d2b6da5eb1d
- **New order ID:** 6e28cfdf-1583-4386-ae24-b61a3c2e7dbb
- **Client order ID:** harvest_20260430_CVS_breakeven_lock
- **Strategy tag:** harvest-breakeven-lock

## Trigger condition (skills/harvest-plan.md breakeven-lock rule)
- Entry: $75.8286
- Original stop: $72.08
- 1R = entry − stop = $3.75
- Current price: $83.24 (intraday -0.79%, cumulative +9.77%)
- Price ≥ entry + 1R = $79.58 ✓
- Stop below entry ($72.08 < $75.83) ✓
- → Move stop to entry (locks in zero-loss)

## Position context
- 27 sh @ $75.83 = $2,047 cost basis
- Current value: $2,247 (+$200, +9.77%)
- Thesis target: $90 (still ~$6.76 / 8.1% away — no trim trigger yet)
- Cohort: managed-care triple-bull (UNH/CNC/ELV all Q1 bull)
- Buffer: $83.24 - $75.83 = $7.41 below current price (8.9% drop triggers stop)

## Notes
- No PDT issue — this is a stop modification on existing GTC order, not a new opening trade
- Daily 2-trade cap (CVX + NUE morning) does not apply to stop adjustments
- Reaper green-tagged; this is the Harvest follow-up for capital preservation
