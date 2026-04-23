# Trade: LRCX Buy — Autopilot Morning 2026-04-23 (FIRST SLEEVE-ROUTED TRADE)

**Strategy:** catalyst-buy (semi_ai sleeve)
**Source:** autopilot_morning cron, first run with new sector sleeve infrastructure live

## Catalyst Stack

1. **Apr 22 16:08 ET (after-bell):** Q3 record beat — Adj EPS $1.47 vs $1.36 (+8.1%), Sales $5.841B vs $5.779B
2. **Apr 22 16:09 ET:** Q4 guide ABOVE consensus — Adj EPS $1.50-1.80 vs $1.45 est (high end +24%); Sales $6.2-7.0B vs $6.09B
3. **Apr 23 04:37 ET:** Semi-equipment cycle hardening (stacks with TXN beat+raise overnight)
4. **General sector:** AI capex tailwind for semi-equipment (NVDA + TSLA Giga Texas + INTC foundry pivot all driving deposition/etch demand)

## Price Action — under-reaction

- Yesterday close: $265.48
- Today open: $264.89
- Current (10:04 ET): $267.32 → **+0.7% from prev close**
- Expected impact for beat+raise + semi cycle confirmation: +5-10%
- Reaction ratio: 0.7% / 7.5% midpoint = **0.09 → MASSIVE under-reaction**

The market is barely pricing the LRCX beat+raise — surprising given the cleanest signal in the semi cohort this week. Sleeve-aware classification (HOT regime override): Under-reacted (ratio < 0.5). Cleanest catalyst-buy setup of the day.

## Sleeve Routing (NEW infrastructure)

- **Sleeve:** semi_ai
- **Regime:** HOT (auto-detected, 6+ qualifying alerts ≥70 in last 7 days)
- **Sleeve target:** $5,400 (25% of $21,598 portfolio)
- **Sleeve held pre-trade:** $2,431 (NVDA only, 45% fill)
- **Sleeve dry powder:** $2,969
- **Per-name cap (sleeve):** 6% of portfolio = $1,296
- **Position size:** 4 sh × $267.50 = $1,070 (well within sleeve cap)

## Pipeline (abbreviated)

- **Iris:** beat + raise + sector-cycle confirmation; no negatives
- **Grace:** LRCX ~$140B, semi-equipment (deposition/etch); leveraged to AI capex cycle
- **Atlas:** beat+raise mega-cap typically +5-12% over 1-2 weeks; +0.7% = ~10× under-reaction gap
- **Victor:** Stop $246 = -8% from entry. Max loss on 4 sh ~$86. Position 5.0% of portfolio
- **Diana:** **BUY 4 sh @ $268.50 limit, target $295 (+10%), stop $246 (-8%)**

## Safety gates

| Gate | Value | Status |
|------|-------|--------|
| Daily trade cap (2) | 1 used (LRCX) | ✓ (1 remaining for INTC) |
| Daily spend ($4K) | $1,070 | ✓ |
| Max position (10% global) | 5.0% | ✓ |
| Sleeve per-name cap (6%) | 5.0% | ✓ |
| Sleeve total ceiling (35%) | $3,500 / 16% | ✓ |
| Min cash reserve ($2K) | $3,483 after | ✓ |
| Circuit breaker (-8%) | +0.08% day | ✓ |
| Limit order | Yes ($268.50) | ✓ |
| Stop-loss | **PDT blocked** same-day — deferred to tomorrow AM | ⚠ deferred |

## Execution

- Order ID: `bcd0abbf-6b99-4216-af1f-09341d3f009e`
- Client ID: `autopilot_20260423_LRCX_sleeve_buy`
- Type: limit buy 4 sh @ $268.50 day-TIF
- **FILLED at $267.3705** (total $1,069.48, better than limit)
- Stop rejected by Alpaca code 40310000 — defer to tomorrow's autopilot (mirror BA/MRK/AEM pattern)
- **Sleeve:** semi_ai
- **Sleeve Flex Used:** false (no cash-flex needed; reserve adequate)

## Plan

- Entry: $267.3705 (filled)
- Stop: **$246 (pending tomorrow)** — ~-8% from entry
- Target: $295 (+10%, +1.3R)
- Horizon: 10-30 days (semi-equipment cycle absorption)
- Exit triggers: stop hit, target hit, semi cycle thesis break, broader semi sector rotation

## Tomorrow's Autopilot Action

1. Place LRCX stop $246 GTC (T+1 should clear PDT)
2. Place INTC stop $61.60 GTC
3. Verify BA stop $205 still active (placed today)
4. Verify MRK stop $103.50 still active

## Post-Trade Sleeve State

- semi_ai sleeve held: NVDA $2,431 + LRCX $1,070 = $3,501 (65% of $5,400 target — HEALTHY)
- Sleeve dry powder remaining: $1,899 (will be reduced after INTC buy)
