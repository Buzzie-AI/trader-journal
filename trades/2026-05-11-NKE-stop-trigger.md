---
title: "Trade: NKE STOP TRIGGER — 2026-05-11"
date: 2026-05-11
ticker: NKE
---

# Trade: NKE STOP TRIGGER — 2026-05-11 14:54 ET

**Strategy:** stop-loss exit
**Source:** GTC stop placed 2026-04-17 ($40 initial → $42.50 advance)
**Detected:** 2026-05-11 16:25 ET autopilot_close run

## Order

- **Stop trigger:** $42.50
- **Filled:** 44 sh @ **$42.50** (clean fill at stop, no slippage)
- **Realized P&L:** ($42.50 − $45.2868) × 44 = **−$122.62 / −6.2%**
- Side: SELL (sell_to_close)
- Order class: stop (GTC)
- Original entry: 44 sh @ $45.2868 on 2026-04-01
- Hold: 40 days
- Alpaca order ID: c5864f03-7f0b-4e5b-8457-410b5d8c2cb7

## What happened

NKE was the day's bear leg. Reaper flagged it as YELLOW++ at 09:53 AM manual run (1.1% cushion to stop) and 13:14 midday (0.4% cushion at day low $42.635). Recommendation both times: **let stop work** — clean exit acceptable.

Two macro headwinds compounded:
1. **Trump rejects Iran "totally unacceptable" peace proposal** (pre-market Mon 05:47 alert) → energy premium back, inflation pressure on consumer discretionary
2. **68-ticker consumer discretionary sector sell-off** alert at 14:50 ET (Mercury filter dropped as aggregator but the underlying flow was real). NKE included in the sell-off list.

By 14:54 ET — 4 min after the consumer-disc sector aggregator alert — NKE punched through $42.50 and stop filled cleanly at the trigger price.

## What we got right

- ✅ Stop discipline. The $42.50 stop was at risk all day (Reaper marked YELLOW twice) but we didn't tighten (no point) and didn't proactively exit (clean stop was the right path).
- ✅ Clean fill at trigger ($42.50 exact). No slippage despite sector-pressure tape.
- ✅ Limited the loss to -6.2%. Reasonable for a 40-day hold on a name that was structurally weakening for weeks.

## What we got wrong (or could improve)

- ⚠️ Thesis weak for weeks. NKE was -2.5% intraday at midday and Reaper flagged it. We could have proactively trimmed at $44+ days earlier and avoided the full stop fill. But absent fresh bear catalyst, sticking with the stop discipline is defensible.
- 🤔 Real-time detection latency. Stop fired 14:54 ET; not surfaced until 16:25 autopilot_close (1h31m gap). Same latency issue as CEG stop earlier today. Position-fill monitoring should be added to mercury stream cron (or harvest cron) to surface fills inside 5 min.

## Realized today total

- CEG +$66.64 (11:09 ET stop)
- NKE -$122.62 (14:54 ET stop)
- **Net: -$55.98**

Despite the net realized loss, account equity is +$110.61 / +0.42% on the day vs Fri close (the AVGO/AMAT buys' near-flat P&L plus existing position appreciation more than offset the NKE realized loss).

## Strategy notes

- Consumer discretionary exposure now reduced to zero
- Cash freed: $1,870 (44 × $42.50)
- Could consider NKE re-entry at lower levels (sub-$40 with clear bottom signal + improving athletic-wear data), but no rush
- Pipeline-discipline: any re-entry would require fresh full pipeline run, not "buy the dip"
