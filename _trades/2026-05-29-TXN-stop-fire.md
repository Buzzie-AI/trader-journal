---
title: "TXN Stop Fire — 2026-05-29"
date: 2026-05-29
ticker: TXN
---

# TXN Stop Fire — 2026-05-29

**Trigger:** Stop $310 fired at **10:43:20 ET** (15 min after autopilot_morning completed at 09:57)
**Fill:** 5 sh @ $309.87 (slippage -$0.13)
**Entry:** $272.83
**Realized:** **+$185.20** (5 × $37.04)

## Pattern recurrence — 3rd in a row (BSX → MRVL → TXN)

| Date | Ticker | AM autopilot | Stop fire | Lag |
|------|--------|--------------|-----------|-----|
| 5/27 | BSX | 09:57 | ~10:30 | ~33 min |
| 5/28 | MRVL | 09:57 | 10:47 | ~50 min |
| **5/29** | **TXN** | **09:57** | **10:43** | **~46 min** |

**The pattern is consistent.** Stops fire 30-50 minutes after morning autopilot during the first volatility wave of the day. This is exactly the window where the "BSX-pattern mid-morning re-audit" remediation would catch the fire and either let it run, ratchet to breakeven, or update watchlist data.

## TXN-specific notes

- Position carried with 1.9% cushion into Friday open (very tight)
- TXN was flagged in Thu close debrief as "fire likely if memory cycle pause"
- Fill at $309.87 vs $310 stop = 13¢ favorable (clean fill)
- Lifecycle gain at exit: +13.6% from $272.83 entry
- Position fully reaped its trend run (entry late April → mid-May at $325 high → drift down)

## Realized impact on day P&L

- Day equity change: +$132.48 ($31,204.52 → $31,337)
- TXN realized: +$185.20
- CBRS realized: -$28.33
- Net realized: **+$156.87**
- Unrealized changes account for the -$24 gap (CVS pullback, MDB sold-the-news drift)

## Lesson reinforced

The same-day-stop-ratchet-on-bull-stack-analyst-signal rule (documented Thu midday) does not apply here — TXN had no bullish catalyst overnight. This was a normal stop-out on a trend exhaustion + low cushion combination. The TIGHT 1.9% cushion was correctly flagged Thursday close as the elevated fire risk.

The remediation needed is structural: a **mid-morning autopilot run at 10:30 ET** to catch the 30-50 min volatility window. The current schedule (09:23 morning, 12:47 midday, 15:53 close) leaves a 3-hour gap during peak intraday volume that has now produced 3 missed stops in 3 sessions.

**Will propose to operator at close: add `autopilot_midmorning` cron at 10:30 ET weekdays.**
