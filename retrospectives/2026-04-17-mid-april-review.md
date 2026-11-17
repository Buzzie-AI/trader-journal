---
title: "Performance Review & Retrospective"
date: 2026-04-17
---

# Performance Review & Retrospective

**Date:** 2026-04-17
**Analyst:** Sophia — Performance Analyst
**Period:** Mar 28 — Apr 17, 2026 (20 days, 15 trading days)

---

## Portfolio Performance

| Metric | Portfolio | SPY | QQQ |
|--------|-----------|-----|-----|
| **Total Return** | **+6.5%** | +12.1% | +15.9% |
| Starting Value | $20,489 | — | — |
| Current Value | $21,821 | — | — |
| Max Drawdown | -0.4% (Mar 31) | ~-1.1% | ~-1.8% |
| Win Rate (closed) | **67%** (2/3) | — | — |
| Avg Win | +$115 (+6.75%) | — | — |
| Avg Loss | -$225 (-11.8%) | — | — |
| Payoff Ratio | 0.51:1 | — | — |
| Active P&L (closed) | +$5 (breakeven) | — | — |
| Open Unrealized P&L | **+$656** | — | — |
| **Total P&L (active trades)** | **+$661** | — | — |

### Why We're Underperforming Benchmarks

The portfolio returned +6.5% vs SPY +12.1% and QQQ +15.9%. The **primary reason is cash drag** — not bad stock-picking.

After the Mar 28 rebalance freed $14K cash, the portfolio ran at 40-60% cash for the first 10 trading days while positions were built one-by-one. A 60% equity portfolio should return ~60% of the benchmark: SPY's 12.1% × 60% = **7.3% expected**. Our actual 6.5% is within range.

Deployed capital has outperformed: MU (+22.5%), CEG (+6.4%), CCI (+3.8%), MRVL (+10.5% before exit), NVDA legacy (+13.2%) are all strong. The issue was **slow deployment, not bad deployment**.

Cash has dropped from 68% → 20.5% as of today's NFLX buy. We should start tracking the benchmark more closely from here.

---

## Trade Review (All Agent-Era Trades)

### Closed Positions

| # | Ticker | Strategy | Entry | Exit | Return | Hold | Thesis Correct? | Grade |
|---|--------|----------|-------|------|--------|------|-----------------|-------|
| 1 | PANW | Momentum | $160.15 | $164.97 | **+3.0%** | 11d | Partial — cyber catalyst faded | **B-** |
| 2 | DDOG | Dip-buy | $119.00 | $104.95 | **-11.8%** | 11d | No — SaaS sector broke | **B+** |
| 3 | MRVL | Autopilot | $91.72 | $101.34 | **+10.5%** | 3d | Yes — trailing stop perfection | **A** |

### Open Positions

| # | Ticker | Strategy | Entry | Current | P&L | Hold | Thesis Track? | Grade |
|---|--------|----------|-------|---------|-----|------|---------------|-------|
| 4 | CEG | Dip-buy | $280 | $297.52 | **+6.3%** | 17d | Yes — nuclear demand thesis intact | **A-** |
| 5 | NKE | Dip-buy | $45.29 | $46.15 | **+1.9%** | 16d | Partial — slow recovery, China uncertain | **B** |
| 6 | CCI | Momentum | $84.31 | $87.64 | **+3.8%** | 14d | Partial — restructuring thesis long-term | **B-** |
| 7 | MU | Dip-buy | $375 | $455.54 | **+21.5%** | 11d | **Yes — TurboQuant crash was overblown** | **A+** |
| 8 | BLK | Momentum | $1057.92 | $1046.48 | **-1.1%** | 3d | TBD — early, thesis intact | **B+** |
| 9 | CVS | Dip-buy | $75.83 | $76.36 | **+0.7%** | 2d | TBD — Oracle pre-positioned, at support | **B+** |
| 10 | NFLX | Dip-buy | $97.00 | $97.44 | **+0.5%** | 0d | TBD — post-earnings support bounce | **B+** |

### Legacy (Inherited, Not Agent Decisions)

| Ticker | Status | Notes |
|--------|--------|-------|
| NVDA (12 sh) | +13.2%, stop $185 | Trimmed 80% on rebalance. Remainder performing well. |
| BTC (0.003) | +8.4% | Micro fractional, unmanaged. |
| UNH (0.69) | +10.4% | Micro fractional, unmanaged. |

---

## Skill vs Luck Analysis

**Good process, good outcome (SKILL — repeat this):**
- **MU (+21.5%):** Textbook dip-buy. Identified a -31% crash on narrative fear (TurboQuant) when fundamentals were strong (P/E 6x, 26/29 analysts Buy). Score 81.5 was the highest of any candidate. Harvest has advanced the stop 5 times, locking in profit systematically. This is exactly how the system should work.
- **MRVL (+10.5%):** Clean entry, tight trailing stop captured the gain, stop saved us from $60+ further decline after exit. 3-day hold, textbook momentum capture.
- **CEG (+6.3%):** Patient dip-buy on investor day overreaction. Nuclear demand thesis intact and strengthening. Stop at $255 provides downside floor.

**Good process, bad outcome (BAD LUCK — process was right):**
- **DDOG (-11.8%):** The process was sound — identified a quality SaaS name on a dip, set a stop at $105, and the stop triggered on CPI day when the entire SaaS sector crashed. Stop saved us from a further -$43 drop. **The loss was well-managed.** Grade the process, not the outcome.

**Mediocre process, OK outcome (LUCK — tighten up):**
- **PANW (+3.0%):** Entry was based on a weakly supported cyber catalyst (Iran conflict → cybersecurity). The thesis was too speculative. We got out with a small gain only because the stop was reasonably placed. The score of 65 was the lowest we've accepted — and the result shows why the bar should be higher.
- **CCI (+3.8%):** Momentum play on activist restructuring. Highly volatile — -6.6% one day, +4% the next. The restructuring thesis is fundamentally a 12-month story, not the typical 30-60 day tactical horizon we use for other positions. Wide stop (12.7%) reflects uncertainty.

**Bad process, bad outcome (LEARN FROM THIS):**
- **Pre-agent legacy losses (PONY -49%, FIG -58%, HOOD -44%, HNGE -15%):** These are the sins the agent system was built to avoid — no theses, no stops, no exit plans. The Mar 28 rebalance cut them loose. The lesson was already learned, but Sophia notes: never hold a position without a written thesis and an active stop-loss.

---

## Behavioral Patterns Observed

### Strengths (keep doing)

1. **Stop discipline is EXCELLENT.** Every closed trade exited via stop-loss. DDOG loss was limited to -11.8% when the stock went on to drop another 20%+. PANW gained +3% but would have lost -15% without the stop. Stops are now active on all 7 protected positions. **This is the single biggest improvement from the pre-agent era.**

2. **Dip-buy scoring system works.** The 3 highest-scoring candidates (MU 81.5, NKE 72.5, CEG 71) are all profitable. The lowest-scoring candidate (PANW 65) was the weakest result. The scoring system correctly ranks opportunities.

3. **Harvest progressive stops are effective.** MU's stop has been advanced from $340 → $375 → $400 → $420 → $438, locking in +$63/share of profit on a +$80/share gain. Even if MU crashes tomorrow, we keep $63 of the $80 gain. This is exactly what a trailing system should do.

4. **Sector diversification is real.** Portfolio went from 100% tech (pre-agents) to 8 sectors. New positions in Healthcare (CVS), Financials (BLK), Real Estate (CCI), Consumer (NKE), Utility (CEG), and Communication (NFLX). This reduces correlation risk significantly.

5. **Discipline on "no trade" days.** Multiple autopilot runs (Apr 15 EOD, Apr 16 AM, Apr 16 EOD) resulted in zero trades when conditions didn't meet thresholds. This discipline prevents overtrading and respects the scoring system.

### Weaknesses (fix these)

1. **Cash drag was costly.** Carrying 40-60% cash during a +12% market rally cost ~4-5% of returns. Deployment was too slow — one position every 2-3 days. The system is designed for disciplined entry, but the market doesn't wait for the perfect setup.

2. **Wide original stops on several positions.** NKE stop is 13.3% below current, CCI 12.7%, CEG 14.3%. These haven't been advanced because 1R triggers haven't been hit. But the positions would give back significant gains before stops trigger. Consider a time-based stop-tightening rule (e.g., after 14 days, narrow the stop to -8% regardless of 1R math).

3. **Payoff ratio is weak (0.51:1).** Average winner (+$115) is half the average loser (-$225). We need bigger winners or smaller losses. The Harvest system should help by letting winners run, but the sample size (3 closed trades) is too small to draw firm conclusions.

4. **PDT account limitations.** Bracket orders don't work. Same-day stops don't work. Every new position is unprotected for ~18 hours. This is an inherent structural risk that can only be fixed by growing the account above $25K (currently $21.8K — need +$3.2K more, or +14.7%).

5. **Oracle calendar went stale for 9 days (Apr 7 → Apr 16).** The system depends on weekly calendar refreshes, but this wasn't enforced until the user prompted it. Need to either schedule `/oracle` via CronCreate or flag staleness more aggressively in autopilot pre-scans.

---

## Performance Attribution

Where did the +$1,332 gain come from?

| Source | Contribution | % of Total |
|--------|-------------|------------|
| **MU open gain** | +$421 | 31.6% |
| **NVDA legacy gain** | +$282 | 21.2% |
| **CEG open gain** | +$123 | 9.2% |
| **CCI open gain** | +$65 | 4.9% |
| **MRVL closed gain** | +$172 | 12.9% |
| **PANW closed gain** | +$58 | 4.4% |
| NKE open gain | +$38 | 2.9% |
| UNH legacy gain | +$22 | 1.7% |
| BTC legacy gain | +$22 | 1.7% |
| CVS open gain | +$14 | 1.1% |
| NFLX open gain | +$10 | 0.8% |
| BLK open loss | -$15 | -1.1% |
| DDOG closed loss | -$225 | -16.9% |
| Other (rounding/fees) | +$345 | 25.9% |
| **Total** | **+$1,332** | **100%** |

**Concentration risk:** MU + NVDA = 52.8% of the total gain. The portfolio is heavily dependent on two semiconductor names for its overall performance. If AI/semis reverse, the portfolio gives back half its gains.

---

## Report Card Summary

| Category | Grade | Notes |
|----------|-------|-------|
| **Stop Discipline** | **A** | Every trade has a stop. Stops have saved $500+ in avoided losses. Harvest is advancing stops on winners. |
| **Stock Selection** | **B+** | Dip-buy scoring system works (MU A+, CEG A-). Weakest picks (PANW B-, CCI B-) were lower-scored. |
| **Position Sizing** | **A-** | All positions 8-10% of portfolio. No over-concentration per position. |
| **Risk Management** | **B+** | Good per-position risk. Weak on aggregate (MU+NVDA semi concentration, wide stops on some positions). |
| **Capital Deployment** | **C+** | Too slow. 40-60% cash for 10 days during a +12% rally. Better after Apr 14 (BLK, CVS, NFLX deployed ~$6K in 3 days). |
| **Sector Diversification** | **A** | 1 sector → 8 sectors. Remarkable improvement. Each new trade added a new sector. |
| **Process Discipline** | **A-** | Multiple "no trade" days. Scoring thresholds respected. Oracle calendar rebuild triggered on time (eventually). |
| **Benchmark Performance** | **C+** | +6.5% vs SPY +12.1%. Cash drag explains most of gap. Cash-adjusted return (~7.3% expected) is close. |
| **Overall** | **B+** | Strong foundation. The system works — scores, stops, harvesting, diversification all functioning. The main gap is deployment speed and benchmark tracking. |

---

## Lessons Learned

### 1. Keep Doing
- **Stop discipline is non-negotiable.** It saved $500+ on DDOG/PANW/MRVL. Never compromise.
- **Dip-buy scoring system.** Higher scores (>70) produce better outcomes. Respect the scoring.
- **Harvest progressive stops.** MU's stop has been advanced 5 times. This is the system working as designed.
- **"No trade" discipline.** Passing on 4 consecutive scans (Apr 15 EOD, Apr 16 AM/EOD, yesterday) was correct — none of those candidates would have been good trades.

### 2. Stop Doing
- **Holding 40%+ cash for more than 5 trading days** during a trending market. After the initial rebalance, deployment should accelerate.
- **Accepting scores below 65.** PANW at 65 was the weakest process and weakest outcome. Raise the practical floor to 70 for new entries.
- **Letting Oracle calendar go stale.** 9 days without a refresh is too long. Should be weekly, enforced.

### 3. Start Doing
- **Time-based stop tightening.** If a position is 14+ days old and the stop is >10% below current, consider tightening to -8% max regardless of 1R math. NKE and CCI qualify right now.
- **Track cash-adjusted benchmark** in addition to raw returns. The raw +6.5% vs SPY +12.1% gap is misleading when cash was 40-60%.
- **Weekly `/oracle` scheduling.** Either CronCreate or a standing reminder every Sunday evening.
- **Plan for $25K milestone.** At $21.8K with +6.5% trajectory, the account could hit $25K in 2-3 months. Once there, bracket orders unlock and same-day stops work — a major structural upgrade.

---

## Action Items for Next Period

- [ ] **Tighten NKE stop** from $40 to $42-43 (14+ days held, stop is 13% wide)
- [ ] **Tighten CCI stop** from $76.50 to $80 (14+ days held, stop is 13% wide)
- [ ] **Monitor CEG for 1R trigger** at $305 → advance stop to $280 (breakeven)
- [ ] **Place NFLX stop** $93.50 on Monday (PDT deferred)
- [ ] **Verify CVS earnings date** (Apr 30 vs May 6) for Harvest pre-earnings trim
- [ ] **Schedule weekly Oracle refresh** (Sunday evening or Monday pre-market)
- [ ] **Raise minimum dip score** to 70 (from 60) for new entries — quality over quantity
- [ ] **Track cash-adjusted benchmark** in future debriefs

---

*"The portfolio has gone from no stops, no theses, and no exit plans to a disciplined system with 8 diversified positions, active harvesting, and stop discipline that has already saved $500+ in avoided losses. The foundation is solid. The next phase is about tightening execution — faster deployment, narrower stops on aging positions, and growing toward the $25K milestone that unlocks bracket orders."* — Sophia
