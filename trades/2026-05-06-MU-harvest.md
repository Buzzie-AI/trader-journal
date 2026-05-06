# Harvest Action: MU

**Date:** 2026-05-06
**Action:** TRIM_AT_3R + PROGRESSIVE_STOP_ADVANCE
**Triggered by:** 3R milestone hit per skills/harvest-plan.md Rule 3 (deferred from 2026-05-05 16:23 ET autopilot_close run because market had closed)

## Trade Details

| Field | Value |
|-------|-------|
| Entry | $541.11 |
| Original shares | 4 |
| Shares before trim | 4 |
| Shares trimmed | 1 |
| Shares remaining | 3 |
| Trim limit price | $648.00 |
| Trim fill price | $653.3162 (better than limit by $5.32) |
| Realized P&L | +$112.21 ((653.32 - 541.11) × 1) |
| Old stop | $510 (entry-stop level, locked -5.7%) |
| New stop | $603 (entry+2R, locks +$185.67/sh = +34.3% on 3 remaining sh) |

## Pre-trade math
- 1R = $541.11 - $510 = $31.11
- Current price $649.345 (snapshot at decision time) = +$108.235 = **3.48R** (above 3R milestone)
- Trim 25% per harvest config trim_at_3r_pct=25 (1 of 4 sh)
- Advance stop to entry+2R = $541.11 + $62.22 = **$603.33** → rounded down to $603

## Order IDs

| Order | ID | Status |
|-------|-----|--------|
| Cancel old stop ($510, 4 sh) | 958fcc6f-0baa-4d7e-9c34-49df1a8adc9b | Canceled |
| Sell limit (1 sh @ $648) | 3708aa1a-679c-4b76-bd72-8d1b39ad9491 | FILLED @ $653.32 |
| New Stop ($603, 3 sh) | 3527eb76-e9c6-4519-b679-6c7758f37c3d | Accepted |

## Rationale
MU at +20% unrealized on Q1 print + memflation cycle + Trump memory-chip-bloc thematic + AMD AI-CPU readthrough. 3R milestone hit cleanly. 25% trim banks +$112 realized; remaining 3 sh ride with stop locked at $603 (+11.4% above cost). Per progressive stops, next advance triggers at 4R = $665.55.
