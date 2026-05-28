---
title: "MRVL Stop Fire — 2026-05-28 10:47 ET"
date: 2026-05-28
ticker: MRVL
---
# MRVL Stop Fire — 2026-05-28 10:47 ET (MISSED IN MORNING AUTOPILOT)

**Action:** STOP FIRED (sell-to-close)
**Order ID:** `f3520c7b-efb6-4d25-a7a8-12c8ebc1c55f`
**Qty:** 4 sh
**Stop price:** $195
**Filled price:** **$195 (clean, no slippage)** ✅
**Entry:** $189.11 (avg from 5 sh @ $189.11, after pre-ER trim 1 sh @ $200.18 on 5/27)
**Realized:** **+$23.56** (4 × ($195 - $189.11))

## Why missed in morning audit

Morning autopilot ran 09:57 ET. MRVL stop fired 10:47 ET = **50 minutes after autopilot Phase 0 completed**. Same pattern as yesterday's BSX miss (09:48 ET stop fired 3 min after 09:45 ET morning autopilot).

**Memory rule violated:** "Morning stop audit window — re-check stop status mid-morning if volatility flags" (per BSX-fire memory 5/27). The 4 AM stream alerts on Iran-strikes UNVERIFIED + the heavy MRVL analyst churn during 09:00-12:00 ET would have qualified as volatility flags but I didn't trigger a mid-morning audit.

**Net:** I spent the next 3 hours writing alerts labeled "MRVL HELD" with all the bull-stack analyst data — ALL after the position was already closed. The bull analyst stack (Stifel/Needham/Benchmark/BofA/Rosenblatt/KeyBanc/Wells Fargo/Rosenblatt $260 each + TD Cowen $200 Hold + MS $195 Neutral) does NOT benefit our (now-zero) position.

## Why MRVL dipped to $195

Intraday range: $194.79 low → $207.31 high. Stop fired at $195 then stock rallied back. Possibly:
- Sell-the-news pattern from yesterday's print (per "SNOW exploded, MRVL muted" alert)
- Initial post-print analyst Hold from Morgan Stanley + TD Cowen weighed early
- Bounced back as bull-stack accumulated (Stifel/Needham/Benchmark all post-print bull)

## Net outcome

| Item | Value |
|------|-------|
| Sold 4 sh | $780.00 |
| Cost basis | $756.44 |
| **Realized gain** | **+$23.56** |
| Lost opportunity | 4 × ($205.67 - $195) = $42.68 (at midday $205.67) |
| Net vs ideal | Realized = ~36% of bull-stack-suggested gain |

## What I should have done

1. **Mid-morning re-audit** after MRVL stream alerts flowed (~10:30 ET) per BSX memory rule
2. **Stop ratchet $195→$200 IMMEDIATELY at open** — but math: open $202.80 → stop $200 = $2.80 cushion = 1.4% safe, would have prevented the stop fire (intraday low $194.79 above $200 ratchet stop = stop $200 also would have fired!)

Actually rethinking: If stop had been $200, it would have fired at $200 instead of $195 = realized 4×($200-$189.11) = +$43.56 instead of +$23.56 = $20 better outcome.

**Lesson:** Either ratchet stops same-day as bullish analyst stack lights up, OR sit on hands. Sitting on hands with stale $195 stop while bull stack builds = worst of both worlds (got stopped at lower price than market consensus).

## Updated state

- MRVL position: ZERO
- Cash: +$780 (from sale)
- Realized today: +$23.56
- Tech sleeve fill drops slightly (semi_ai still has NVDA/MU/AVGO/TSM + TXN + CSCO)
