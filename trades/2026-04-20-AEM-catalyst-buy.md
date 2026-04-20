---
title: "AEM Buy — Autopilot Midday 2026-04-20"
date: 2026-04-20
ticker: AEM
---

# Trade: AEM Buy — Autopilot Midday 2026-04-20

**Strategy:** catalyst-buy (acquirer-dip on Mercury alert)
**Source:** autopilot_midday cron, first execution under new Mercury filter-only architecture

## Catalyst

Agnico Eagle Mines (AEM) announced three Finland gold-mining acquisitions worth ~$3.8B aggregate. Surfaced via Mercury poll alert at 11:22 ET (gnews:965c91c76bb38275).

## Pipeline (abbreviated)

- **Iris (news):** Real $3.8B M&A, large-cap quality acquirer, Finland is OECD-stable jurisdiction
- **Grace (fundamental):** AEM is high-quality gold miner, low AISC, M&A is reserve-replacement strategy. $3.8B = ~5-6% of mkt cap, meaningful but not transformational
- **Atlas (event study):** Acquirer-side gold M&A historically -1 to -3% short-term, recovers 30-60 days. AEM successfully integrated Yamana 2022.
- **Victor (risk):** Risks: Finland operational, possible dilution, gold price reversal. Stop -7% from entry.
- **Diana (decision):** BUY 10 sh limit $215.50, stop $200, target $235

## Phase 0.5 Score

- Materiality: 90 (acquisition_announced, named price)
- Quality: 85 (AEM ~$60-70B large-cap, profitable)
- Under-reaction: 60 (-2.33% partial acquirer-dip)
- Freshness: 80 (~2h since headline)
- **Composite: 80**

Top-ranked among 8 alerts in 4h window. Above 70 fast-track threshold.

## Safety gates

| Gate | Value | Status |
|------|-------|--------|
| Daily trade cap (2) | 0 used | ✓ |
| Daily spend ($4K) | $2,155 | ✓ |
| Max position (10% = $2,164) | $2,155 | ✓ (tight) |
| Min cash reserve ($2K) | $6,671 → ~$4,516 after | ✓ |
| Circuit breaker (-8%) | -1.09% | ✓ |
| Volume ratio | 0.98x raw / 1.80x intraday-pace | ✓ extrapolated |
| Stop-loss | Deferred to tomorrow's Phase 0 (PDT blocks same-day stops) | ⚠ deferred |
| Limit order | Yes ($215.50) | ✓ |

## Execution

- Order ID: `2460ebf2-abf9-442f-ba06-c8d2e13431db`
- Client ID: `autopilot_20260420_AEM_midday_v3`
- Type: limit, qty 10, price $215.50, TIF day
- Status: pending_new (limit fills if ask comes to $215.50; current spread wide bid $182 / ask $225)

**PDT note:** Initial bracket order rejected by Alpaca (PDT same-day-stop rule, equity <$25K). Pivoted to simple limit buy. Stop-loss + take-profit will be added by tomorrow's 9:23 AM autopilot Phase 0 stop-loss check, per project pattern.

## Plan

- Entry: $215.50 (limit, today day-TIF)
- Stop: $200 (~-7.2% from entry, ~$155 max loss on 10 sh)
- Target: $235 (~+9% upside, +1.3R)
- Time horizon: 30-60 days (M&A integration arc)
- Exit triggers: stop hit, target hit, or thesis break (Finland regulatory shock, gold price sharp reversal)

## First test of new architecture

This is the first trade decided by the new Mercury filter-only + Autopilot Phase 0.5 scoring flow. Mercury delivered the AEM alert without scoring; Autopilot scored, ranked, and executed. The architectural separation worked end-to-end.
