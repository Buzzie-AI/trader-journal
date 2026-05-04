---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-04 12:47 PM ET (Monday mid-session — eod_summary refresh, market still open 3h13m)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$25,251.27** |
| Cash | $2,119.51 (8.4%) ✅ above $2K min-reserve |
| Invested | $23,131.76 (91.6%) |
| Positions | 13 equity + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **3 actions**: (1) MU stop $510 GTC placed AM (T+3 catch-up); (2) **NVDA stop fired 11:21 ET** — 10 sh @ $194.885 = +$179.55 realized / +10.1%, freed $1,949 cash; (3) **INTC sleeve catalyst-buy 12:27 ET** — 12 sh @ $96.8499 = $1,162 (sleeve specialty tier, full pipeline pass, score 78). |
| Stop coverage | ✅ 11 active stops (BLK/CCI/CEG/CVS/CVX/MRK/MRVL/MU/NKE/NUE/TXN). **INTC stop $89.50 deferred to T+1** (tomorrow morning autopilot). Exempt: UNH (fractional), 737CVR019 (CVR), BTC. |
| 🎯 Best held | **CEG +14.0%** 🎯 (AI-power, +3.74% intraday) · **BTC +13.2%** ($80,237) · **CVS +8.8%** · **MU +7.0%** (HBM4, +6.78% intraday) · **CCI +6.4%** · **UNH +27.2%** (fractional) |
| Day P&L | **+$157.84 / +0.63%** vs Friday close $25,093.43 |
| **Realized today** | **+$179.55** (NVDA stop) |

---

## Equity Curve (1 Month)

<div style="width:100%;overflow-x:auto">
<canvas id="equityChart" width="800" height="300"></canvas>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-annotation"></script>
<script>
const ctx = document.getElementById('equityChart').getContext('2d');
new Chart(ctx, {
  type: 'line',
  data: {
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25251.27],
      borderColor: '#16a34a',
      backgroundColor: 'rgba(22,163,74,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 4,
      pointBackgroundColor: '#16a34a',
      borderWidth: 3
    }]
  },
  options: {
    responsive: true,
    plugins: {
      legend: { display: true, position: 'top' },
      tooltip: {
        callbacks: {
          label: function(ctx) { return ctx.dataset.label + ': $' + ctx.parsed.y.toLocaleString(); }
        }
      },
      annotation: {
        annotations: {
          sleeveLine: {
            type: 'line',
            xMin: 'Apr 23',
            xMax: 'Apr 23',
            borderColor: '#3b82f6',
            borderWidth: 2,
            borderDash: [4, 4]
          },
          depositMarker: {
            type: 'point',
            xValue: 'Apr 23',
            yValue: 24602.55,
            backgroundColor: '#a855f7',
            radius: 7,
            borderColor: '#fff',
            borderWidth: 2
          },
          depositLabel: {
            type: 'label',
            xValue: 'Apr 23',
            yValue: 24602.55,
            yAdjust: -20,
            content: ['+$3K deposit'],
            color: '#a855f7',
            font: { size: 11, weight: 'bold' },
            backgroundColor: 'rgba(255,255,255,0.85)',
            padding: 3
          }
        }
      }
    },
    scales: {
      y: {
        ticks: { callback: function(v) { return '$' + (v/1000).toFixed(1) + 'k'; } },
        min: 19000, max: 26000
      }
    }
  }
});
</script>

| Period | Start | End | Change | Notes |
|--------|-------|-----|--------|-------|
| **Today (May 4 intraday)** | $25,093 (Fri close) | $25,251 | **+0.63% (+$158)** | NVDA stop fired (+$180 realized); INTC sleeve buy filled; MU +6.8%; CEG +3.7% |
| 1 Week | $24,880 (Apr 30) | $25,251 | +1.5% | CVX/NUE stops + MU sleeve add (5/1); NVDA stopout + INTC buy (5/4) |
| **Since Agents (Mar 28)** | $20,489 | $25,251 | **+$4,762 (+23.2%)** | Excludes $3,000 Apr 23 deposit; agent P&L only ~+$1,762 (+8.6%) |
| Total equity (incl deposit) | $20,489 | $25,251 | +23.2% | |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$1,762 (+8.6% in 37 days)**. The total-equity chart includes a $3,000 deposit on Apr 23 (purple dot).

Blue dashed line = sector-sleeve infrastructure deployed (Apr 23). Purple dot = $3K capital injection (Apr 23).

---

## Current Positions (intraday — 13 equity)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **CEG** | 7 | $280.00 | $319.32 | **+$275** | **+14.0%** 🎯 | 8.9% | $290 ✅ (above entry) |
| **CVS** 🎯 | 27 | $75.83 | $82.51 | +$180 | **+8.8%** | 8.8% | $75.83 ✅ (breakeven-lock) |
| **MU** 🆕 | 4 | $541.11 | $579.00 | +$152 | **+7.0%** | 9.2% | **$510 ✅ (placed today T+3)** |
| **CCI** | 20 | $84.31 | $89.72 | +$108 | +6.4% | 7.1% | $84.31 ✅ (breakeven-lock) |
| UNH | 0.69 | $290.00 | $368.75 | +$54 | **+27.2%** | 1.0% | — fractional exempt |
| **TXN** | 5 | $272.83 | $280.79 | +$40 | +2.9% | 5.6% | $254 ✅ |
| **MRVL** | 9 | $159.54 | $163.50 | +$36 | +2.5% | 5.8% | $145 ✅ |
| **BTC** | 0.0034 | $70,867 | $80,237 | +$32 | **+13.2%** | 1.1% | — crypto exempt |
| **MRK** | 18 | $112.47 | $113.41 | +$17 | +0.8% | 8.1% | $103.50 ✅ |
| **NUE** | 9 | $223.00 | $224.23 | +$11 | +0.6% | 8.0% | $210 ✅ |
| **INTC** 🆕🆕 | 12 | $96.85 | $96.89 | +$0 | flat | 4.6% | **$89.50 PLANNED T+1** |
| CVX | 10 | $191.92 | $191.88 | -$0 | flat | 7.6% | $182 ✅ |
| BLK | 2 | $1,057.92 | $1,052.48 | -$11 | -0.5% | 8.3% | $990 ✅ |
| NKE | 44 | $45.29 | $43.32 | -$86 | -4.3% | 7.5% | $42.50 ✅ TIGHT |

**Total Open P&L: +$806 unrealized.** Today's intraday drivers: CEG +$81, MU +$147, CCI +$9, MRK +$23, INTC +$0; offset by NKE -$47, MRVL -$13, NUE -$16, BLK -$18.

**🚪 Closed today (realized):** NVDA 10 sh @ $194.885 = **+$179.55 / +10.1%** (stop fired 11:21 ET; entry 2026-03-09 @ $176.93).

---

## ⭐ Sector Sleeve Status (semi_ai)

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $6,313 (25%) | $6,354 (101%) | **AT TARGET** | MRVL, TXN, MU, **INTC 🆕** |

**Sleeve concentration:** 25.2% of equity (target 25%, ceiling 35%). INTC sleeve catalyst-buy filled the 82%→101% gap exactly. Sleeve members: MRVL $1,472 / TXN $1,404 / MU $2,316 / INTC $1,163. Priority queue can return to standby until next regime check.

---

## Allocation (intraday)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MRVL, TXN, MU, INTC) | $6,354 | 25.2% (at target) |
| Healthcare (MRK, CVS, UNH) | $4,523 | 17.9% |
| Utility/Nuclear (CEG) | $2,235 | 8.9% |
| Financials (BLK) | $2,105 | 8.3% |
| Materials (NUE) | $2,018 | 8.0% |
| Energy (CVX) | $1,919 | 7.6% |
| Consumer (NKE) | $1,906 | 7.5% |
| Real Estate (CCI) | $1,794 | 7.1% |
| Crypto (BTC) | $277 | 1.1% |
| **Cash** | **$2,120** | **8.4%** ✅ above $2K reserve |

Cash buffer thinned to ~$120 above reserve after INTC fill — disciplined deployment, no further BUYs this run. Semi sleeve at target cleanly.

---

## Open Orders (11 active stops + 1 deferred T+1)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 4 | $510 | GTC | Placed today AM (T+3 catch-up) |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CVS | 27 | $75.83 | GTC | Breakeven-lock |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | TIGHT buffer ~$0.82 |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $254.00 | GTC | |
| Stop | CVX | 10 | $182.00 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |
| **PENDING** | **INTC 🆕** | 12 | $89.50 | GTC | **T+1 placement tomorrow morning autopilot** |

🚪 **Filled today:** NVDA 10 sh stop @ $195 → fill $194.885 (order `96e50d4c`). Position closed.
🆕 **Filled today:** INTC 12 sh BUY @ limit $97 → fill $96.8499 (order `f981471e`).

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-04** | **NVDA** | Stop fired @ $194.885 (10 sh) | **+$179.55 / +10.1%** | Entry 3/9 @ $176.93. Stop 4/27 post-harvest-trim. ~57d hold. |
| 2026-04-28 | INTC | Stop fired @ $81.50 (gap-down) | +$204 | Q1 blowout +29× then sleeve compression |
| 2026-04-28 | LRCX | Stop fired @ $245.94 | -$86 | US Commerce Hua Hong tool-ban |
| 2026-04-28 | BA | Stop fired @ $227.87 | +$44 | Airbus Q1 mixed peer-cohort |
| 2026-04-23 | AEM | Stop fired @ $199.96 (open) | -$152 | Reversal of Apr 20 catalyst-buy |
| 2026-04-21 | NFLX | Reaper SELL | -$68 | Reed Hastings exit + weak guide |

---

## Mon catalyst cluster — autopilot_close digest (12:27 ET)

**Tier-1 in pipeline (executed):**
- ✅ **INTC** (score 78) — multi-axis bull (SambaNova antitrust + perm CTO + Physical AI Group + Sat upgrades), under-reacted -2.85%, sleeve specialty tier. **FILLED 12 sh @ $96.8499.**

**Tier-1 watchlist (cash-bound this run):**
- AMZN (score 75) — 6-deep multi-axis (Anthropic + OpenAI + JPM + supply chain + HUMAIN + DoW CMMC); +0.88% partial reaction
- ORCL (score 72) — classified Dept of War + $1.1T tailwind framing; +3% intraday
- LMT (score 70) — defense $119B Israel; +1.72% confirming reaction
- JNJ (score 60) — pharma cohort defensive; -1.13%

**Tier-1 rejected:**
- ❌ **QCOM** — premarket +20% rally on mystery chip deal headlines fully unwound to **-5.13%** by 12:24 ET. Over-reacted/round-trip pattern. Revisit only on confirming bullish catalyst.

**Bear-qualifiers:** AZN (FDA panel reject), NCLH (FY26 guidance cut), META (China Manus block + capex digest), BA (-1.55% despite defense tailwind)

---

## Recent autopilot debriefs

- [2026-05-04 12:27 ET (close — INTC sleeve catalyst-buy)](debriefs/2026-05-04-1227.html) — 1 BUY filled, sleeve at target, full pipeline pass
- [2026-05-04 09:18 ET (midday — streamlined)](debriefs/2026-05-04-0918.html)
- [2026-05-04 05:58 ET (morning)](debriefs/2026-05-04-0558.html) — MU stop placed, 22 Mercury alerts scored
- [2026-05-01 16:23 ET (close)](debriefs/2026-05-01-1623.html)
- [2026-05-01 13:17 ET (midday)](debriefs/2026-05-01-1317.html)
- [2026-05-01 09:50 ET (morning)](debriefs/2026-05-01-0950.html)

---

## Architecture / Cron note

**Cron timezone bug active:** all configured ET cron expressions firing in UTC interpretation (4h early). Today's pattern:
- `27 9 * * 1-5` autopilot_morning → fired 5:58 ET premarket
- `47 12 * * 1-5` autopilot_midday → fired 9:18 ET (12 min before open)
- `53 15 * * 1-5` autopilot_close → fired 12:27 ET (3.5h before close)

**Net impact today:** despite the timing skew, the close run was the **first actionable autopilot since cash binding cleared** — caught the INTC entry window with full pipeline discipline. Bug fix still pending; doesn't block execution but wastes the morning analytical pass.
