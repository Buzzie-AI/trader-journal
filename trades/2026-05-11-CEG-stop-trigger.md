---
title: "Trade: CEG STOP TRIGGER — 2026-05-11"
date: 2026-05-11
ticker: CEG
---

# Trade: CEG STOP TRIGGER — 2026-05-11 11:09 ET

**Strategy:** stop-loss exit
**Source:** GTC stop placed 2026-04-27 (subsequently ratcheted to $290)
**Detected:** 2026-05-11 13:14 ET midday autopilot run (the stop had fired at 11:09 ET but wasn't surfaced in real-time)

## Order

- **Stop trigger:** $290.00
- **Filled:** 7 sh @ **$289.52** (slight slippage; day low touched $288.83)
- **Realized P&L:** ($289.52 − $280.00) × 7 = **+$66.64 / +3.4%**
- Side: SELL (sell_to_close)
- Order class: stop (GTC)
- Original entry: 7 sh @ $280.00 on 2026-04-01
- Hold: 40 days
- Alpaca order ID: 61cdab59-e3e8-4216-924d-06018025b9fb
- Client order ID: `autopilot_20260427_CEG_stop_replaced`

## What happened

CEG reported Q1 today (alerted at 07:02 ET by Mercury stream — score 81.75):
- Q1 Adj EPS $2.74 BEAT $2.57 (+6.6%)
- Q1 Sales $11.122B vs $8.721B est (MASSIVE 28% sales beat)
- Catalyst type: earnings_beat with structural AI-power thesis tailwind

Despite the mega-beat, the tape SOLD THE NEWS:
- Pre-open implied: positive
- Open: $313.53 (positive reaction)
- Intraday high: $317.39 (+4% from prev close $303.50)
- Then **selloff began** — tape sold the news
- 11:09 ET: stop triggered at $290 fill price $289.52
- Day low (after stop): $288.83

This is the canonical "sold the news on Q1 beat" pattern.

## What we got right

- ✅ Stop discipline. The $290 stop was placed 4/27 (initial $255) and ratcheted to $290 on 4/27 per Harvest progressive_stops rule (at_2r → entry + 1R = $290 lock).
- ✅ Reaper flagged CEG as YELLOW at 09:53 manual run with 3.7% cushion. The recommendation was "hold for midday reassessment, don't tighten given Q1 vol". The stop was in the right place.
- ✅ Locked small profit (+3.4%) rather than letting position decay further (low touched $288.83 ~30c below stop, suggesting we got a reasonable fill).

## What we got wrong (or could improve)

- ⚠️ The stop fired at 11:09 ET but wasn't surfaced in real-time. None of the Mercury cron fires between 11:00-12:00 checked positions, only the queue. The 11:09 fill went undetected until the 13:14 midday autopilot ran get_all_positions and noticed CEG missing.
- 🤔 Mercury "Constellation Energy Wins Big" at 11:57 ET was alerted on same theme but I filtered as content-dedup — I missed that I had ALREADY been stopped out at that point. A position-state check on each Mercury fire could have surfaced the exit faster.
- 💡 Improvement: add position-fill check to harvest cron, or add a "stop trigger alert" to the news listener to push fill events through the same Mercury alert path.

## Strategy notes

- CEG was the AI-power thesis play — combined Q1 mega-beat + Sat 18:37 Calpine deal close + energy bull setup from Trump-Iran-rejection. Three reinforcing tailwinds.
- Despite the strong fundamentals, the tape didn't care today. Sell-the-news dominated.
- **AI-power exposure now removed from portfolio.** NEE/OKLO remained on watchlist but not entered (daily cap binds).
- Cash freed: $2,026.64 (7 × $289.52)
- Could be a re-entry candidate if CEG stabilizes and the Q1 beat is recognized later in the week. Watch for:
  - Bounce off support around $285
  - Multi-day stability above $290
  - Reaffirmation from analysts
- Re-entry would be a fresh decision through the full pipeline.
