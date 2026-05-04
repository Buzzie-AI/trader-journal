---
title: "NVDA Stop Trigger — 2026-05-04"
date: 2026-05-04
ticker: NVDA
---

# NVDA Stop Trigger — 2026-05-04

## Exit summary

| Field | Value |
|-------|-------|
| Action | SELL (stop-loss triggered) |
| Symbol | NVDA |
| Shares | 10 |
| Fill price | $194.885 |
| Fill time | 2026-05-04 11:21 ET |
| Stop price | $195.00 (GTC) |
| Order ID | `96e50d4c-6f6b-4f64-8574-f1ebc0500719` |
| Client order ID | `autopilot_20260427_NVDA_stop_post_trim` |
| Stop submitted | 2026-04-27 14:01 UTC (post-harvest trim) |
| Proceeds | $1,948.85 |

## Realized P&L

The triggered lot maps to the 2026-03-09 buy of 10 sh @ $176.93 (last remaining lot under FIFO after the 3/30 market sell of 48 sh and 4/27 harvest trim of 2 sh).

- Cost basis: 10 × $176.93 = $1,769.30
- Proceeds: 10 × $194.885 = $1,948.85
- Realized: **+$179.55 / +10.1%**
- Hold period: ~57 days (3/9 → 5/4)

## Position state after fill

- **NVDA position closed** (was last 10 sh after 4/27 harvest trim of 2 sh @ $210.52)
- Cash freed: $1,948.85 (account cash now $3,281.71)
- Portfolio: 13 equity positions + BTC + UNH frac (was 14 + BTC + UNH)
- Semi/AI sleeve fill drops: NVDA was a contributing member; sleeve_held_value decreases by ~$1.95K

## Why the stop fired

- Stop was set at $195 GTC on 2026-04-27 immediately after the 2-share harvest trim at $210.52 (breakeven-locked above the 3/9 entry of $176.93, +10.2% above entry).
- Premarket pullback from Friday's close ($202.xx area) accelerated through the open; stop tagged at 11:21 ET.
- Catalyst overhang: NVDA was scored ~71 in this morning's autopilot (Mercury delta) — China=$0 / $380 PT (neutralized) + Cerebras IPO competitive threat. Mixed read flagged in the 09:18 ET debrief; the stop did its job before any operator decision.

## Discipline notes

- Stop was a **breakeven-protector**, not a thesis exit. The harvest trim on 4/27 was the conviction-management action; this stop just locked the floor on the residual lot.
- Cash freed reverses the binding constraint flagged in the 5:58 ET and 9:18 ET debriefs ($1,333 → $3,281, now above $2K min_reserve).
- High-conviction adds (QCOM ~85, INTC ~80, LMT/BA defense, AMZN multi-axis) are now executable through the full 5-agent fast-track pipeline at next autopilot run.

## Next steps

1. Watchlist update — remove NVDA from held cohort, surface to "recently closed (+10.1%)" row
2. Sleeve recalculation — semi_ai sleeve fill recomputes on next /autopilot Phase 0.5
3. No new BUY this run — pipeline discipline requires fresh autopilot fire (Iris→Grace→Atlas→Victor→Diana) on any candidate using the freed cash
