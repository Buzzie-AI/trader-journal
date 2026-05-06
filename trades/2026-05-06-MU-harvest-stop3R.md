# Harvest Action: MU (stop advance only)

**Date:** 2026-05-06
**Action:** PROGRESSIVE_STOP_ADVANCE (no trim — already at min_remaining 25%)
**Triggered by:** 4R milestone breached per morning debrief commitment ("next progressive advance trigger at 4R = $665.55")

## Trade Details

| Field | Value |
|-------|-------|
| Entry | $541.11 |
| 1R | $31.11 |
| 4R milestone | $665.55 |
| Current price | $670.69 (~4.18R) |
| Shares | 3 (post-morning trim, at min_remaining floor) |
| Old stop | $603 (entry+2R, set this morning) |
| New stop | $634 (entry+3R) |
| Locks | $634 - $541.11 = +$92.89/sh = +17.17% above cost on 3 sh |

## Order IDs

| Order | ID | Status |
|-------|-----|--------|
| Cancel old stop ($603) | 3527eb76-e9c6-4519-b679-6c7758f37c3d | Canceled |
| New Stop ($634, 3 sh) | 9ea7e080-33ad-4ecd-8134-e775f50f6b1a | Accepted |

## Rationale
MU continues 4R+ on AI memory thesis. No additional trim per min_remaining floor (already at 25% of original 4 sh). Stop advance to entry+3R locks meaningful gain while preserving room for normal volatility (-5.5% trail from current $670.69).
