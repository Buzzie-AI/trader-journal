# Watchlist — End of Day 2026-04-23

Updated by eod_summary cron. **Day 1 of sleeve infrastructure successfully validated.**

## Current positions (post-close, 13 positions)

| Ticker | Qty | Avg Entry | Current | P&L $ | P&L % | Stop | Sleeve | Notes |
|--------|----:|----------:|--------:|------:|------:|-----:|--------|-------|
| **BA** | 9 | $222.99 | $233.95 | **+$99** | **+4.91%** | $205 ✓ | — | 9-catalyst stack continuing to absorb; near +1R for breakeven-stop trail |
| BLK | 2 | $1057.92 | $1052.55 | -$11 | -0.5% | $990 | — | Modest pullback |
| BTC | 0.0034 | $70,867 | $78,028 | +$25 | +10.1% | — | — | Stable |
| CCI | 20 | $84.31 | $87.52 | +$64 | +3.8% | $80 | — | Q1 FFO beat continuation |
| CEG | 7 | $280 | $292.40 | +$87 | +4.4% | $255 | — | AI-power thesis +1.83% intraday |
| CVS | 27 | $75.83 | $78.67 | +$77 | +3.8% | $72.08 | — | +2.94% intraday — strongest day for healthcare |
| **INTC (NEW)** | **19** | **$66.94** | **$76.70** | **+$185** | **+14.58%** | **$61.60 (PDT pending)** | **semi_ai** | **🎯 Q1 +29× EPS beat + Q2 guide raise = first sleeve win** |
| **LRCX (NEW)** | 4 | $267.37 | $259.00 | -$33 | -3.13% | $246 (PDT pending) | semi_ai | RBC PT $310 raise validates thesis; semi-equip lagged INTC today |
| MRK | 18 | $112.47 | $114.62 | +$39 | +1.91% | $103.50 ✓ | — | REGN MFN precedent overhang to monitor |
| NKE | 44 | $45.29 | $45.15 | -$6 | -0.3% | $42.50 | — | LULU pressure plateaued |
| NVDA | 12 | $177.28 | $199.07 | +$261 | +12.29% | $185 | semi_ai | -1.69% intraday; Google chip caveat continues |
| UNH | 0.69 | $290 | $353.50 | +$44 | +21.9% | — | — | Stable |
| 737CVR019 | 4.06 | $0 | — | — | — | — | — | Corporate action shares |

**Aggregate: portfolio $21,789 | cash $2,212 | day P&L +0.96% (+$208) | total unrealized +$832**

### ⚠ AEM CLOSED at 09:30 ET
- Stop $200 triggered at open at $199.96 (10 sh × $199.96 = $1,999.60 cash inflow)
- Realized loss: **-$152.40** (-7.1% from $215.20 entry)
- **Ironic context**: NEM (gold-mining peer) reported Q1 +31% EPS beat + $6B buyback expansion AH today. Gold sector reframed bull AFTER our exit. Lesson: stop triggered on sentiment overshoot, not fundamentals — but stop did its job preserving capital.

## ⭐ SLEEVE INFRASTRUCTURE — DAY 1 VALIDATION

**This is a 🎯 milestone day.** First live run with sector-sleeve mechanics deployed in the morning captured **exactly the kind of catalyst the old monolithic system was systematically missing.**

### After-Hours INTC Catalyst Stack (post-EOD update)

Eleven INTC catalysts compounded throughout the day — the bull thesis hardened materially after the 4:00 PM close:

1. **Q1 EPS $0.29 vs $0.01 est (29× beat)** + Sales $13.577B vs $12.424B (+9.3%)
2. **Q2 guide $0.20 EPS vs $0.09 est (+more than DOUBLE)** + Sales $13.8-14.8B vs $13.07B
3. CFO: TSLA chip fab deal details "still being worked between Lip-Bu and Elon" (minor caveat)
4. CFO: INTC raising chip prices to reflect costs — pricing power signal
5. CFO: less than $200M external foundry revenue Q1 (foundry pivot still early — important caveat)
6. CEO Lip-Bu Tan: **demand continued to run AHEAD OF SUPPLY for ALL businesses in Q1**
7. CEO: top priority = maximize factory output to meet demand
8. CEO: **CPUs REGAINING POSITION as foundation of AI** (strategic positioning shift)
9. Executive: **custom ASIC business has run rate of OVER $1 BILLION** (first concrete external-revenue datapoint)
10. AMD + ARM rallying AH in sympathy with INTC (sector-wide validation)
11. Trump administration's Intel stake **up 290% in less than a year** (government-aligned interests)

Net post-AH: INTC closed regular session at **$76.19 (+13.82% from $66.94 entry, +$185 unrealized)**. After-bell catalysts position the stock for potential extension at Friday open. Sleeve infrastructure validated end-to-end on Day 1.

```
SLEEVE STATE — END OF DAY
==========================
semi_ai: regime=HOT (auto, 6+ qualifying alerts ≥70 in 7d window)
  target=$5,447 (25% of $21,789)
  current_fill=$4,883 (89.6%) — AT TARGET
  members held: NVDA ($2,389, +12.3%), LRCX ($1,036, -3.1%), INTC ($1,457, +14.6%)
  dry_powder=$564
  priority_queue=ON (capacity constrained until Harvest trim)
  cash_flex_available=YES (not invoked today)
```

**Sleeve P&L today:**
- INTC: **+$185 unrealized in <8 hours** (Q1 +29× EPS beat + Q2 guide raise after-bell)
- LRCX: -$33 (semi-equipment didn't follow INTC up despite RBC PT $310 raise)
- NVDA (held pre-sleeve): +$261 cumulative, intraday -$41
- **Net new sleeve value vs. entry cost: +$152** (LRCX + INTC combined)

**Counterfactual check:** Without sleeve priority queue, this morning's autopilot would have selected TECK/TMO/ELV (general candidates scoring 70-85) over INTC. Today's tape (broad beat-punished cohort, software/tech weakness, pharma MFN bear) would have left those flat-to-slightly-down. The sleeve priority lane captured the +14.6% INTC win that pure score-based monolithic ranking would have missed.

## Today's trades

1. **BA STOP $205 GTC PLACED** — `172ca746` (yesterday's PDT-deferred resolved)
2. **AEM STOP $200 TRIGGERED** at open at $199.96 (realized -$152) — closed position
3. **LRCX BUY** 4 sh @ $267.37 — `bcd0abbf` — **first sleeve-routed trade in project history**
4. **INTC BUY** 19 sh @ $66.94 — `c2c26223` — second sleeve trade

**Daily cap: 2/2 trades used.** LRCX/INTC stops PDT-deferred to tomorrow.

## Tomorrow (Apr 24) morning autopilot priority stack

### URGENT — first action
1. **Place LRCX stop $246 GTC** (T+1)
2. **Place INTC stop $61.60 GTC** (T+1) — **OR consider trailing to $70 to lock in ~$60 of the +$185 gain** (BA is the precedent)
3. **Trail BA stop $205 → $215-220** (Harvest breakeven-lock rule, +1R achieved)
4. Verify MRK stop $103.50 still active

### Top buy candidates from after-bell catalysts
5. **INTC** add-on consideration (currently 6.7% sleeve weight; NVDA-cap exception allows up to 12% for proven thesis names — could add 7 more shares at $76 = $532)
6. **DLR** Q1 beat + guide raise (data center REIT, AI infrastructure)
7. **EW** Q1 beat + guide raise (medtech)
8. **NEM** Q1 +31% beat + $6B buyback expansion (gold reframe)
9. **TECK / TMO / ELV / REGN** general candidates carry-over (REGN now caveated with MFN overhang)

### Bearish watch
10. **MRK (HELD)** — REGN MFN precedent risk; monitor for pricing-deal pressure on big pharma
11. **HON / MOH / LMT / FCX** — guide-cut cohort continuation
12. **CRM / NOW / IBM / META** — tech restructuring + AI anxiety theme
13. **TXN** — gap-up was steep at +16% earlier; if it pulls back materially, becomes interesting

### Sleeve adjustment for tomorrow
- Sleeve fill at 89.6% **AT TARGET**
- INTC up +14.6% may push absolute weight; calculate at open
- May Harvest trim INTC partial (lock ~25% of gain) → free up sleeve capacity for next semi catalyst
- LRCX -3.1% may justify add at lower entry

## Today's Mercury alert summary

**~80 alerts processed today.** Dominant themes:

### Bull cluster
- **🎯 INTC blockbuster** — Q1 +29× EPS beat + Q2 guide raise (sleeve win)
- **Semi/AI**: TXN beat+raise+two upgrades, LRCX RBC PT $310 raise, AMAT Advantest, MU HBM bottleneck, INTC chip fab + 14A node + pricing power, AMD/ARM AH sympathy with INTC
- **Healthcare bull**: UNH 5+ positives, ELV reframe to bull (FY guide raise), MCO triple positive (Q1 + guide + $2.5B buyback), TMO reframe, EW beat+raise, REGN FDA Dupixent
- **AI infrastructure**: ORCL $550B backlog, DLR Q1 beat+guide raise, GOOG Cloud Next 10+ partnerships, MSFT $18B Australia commitment, GPT-5.5 release
- **Aerospace**: BA 9 positives in 48h (but China-orders caveated)
- **Mining**: NEM Q1 +31% + $6B buyback, TECK +75% + Anglo merger Canada approval

### Bear cluster
- **REGN MFN pricing precedent** — Trump deal, sector overhang for LLY/NVO/MRK-held/PFE/BMY/ABBV
- **ABBV FDA CRL** — drug rejection
- **Industrial guide-cuts**: HON triple cut, MOH dramatic -46% Adj EPS, LMT cash flow turns negative, FCX Grasberg delay guide cut
- **Tech restructuring**: META 10% layoffs, MSFT first-ever voluntary buyout, NOW -14% AH on Middle East
- **Beat-punished cohort**: ~12 names (NOC/GE/RTX/CME/IBM/VRT-partial/BSX/TMO-partial/FCX/LVS/AXP/DOW)
- **GOOG EU pressure** + Google Cloud chip push (NVDA bear read-through)

### Macro context
- **Iran peace talks stalled** → oil $100/bbl morning, partial reversal to $95 afternoon
- **Hormuz disruption** persistent
- **Nasdaq 100 eased from records** — broad tech soft despite earnings beats
- **Sentiment-driven environment** confirmed by ~12-name beat-punished cohort
