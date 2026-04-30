---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-30 4:30 PM ET (Thursday EOD)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$25,124.38** |
| Cash | $3,497 (13.9%) |
| Invested | $21,627 (86.1%) |
| Positions | 11 equity + BTC + UNH fractional |
| Today's activity | **2 BUYs** (CVX 10sh @ $191.92 catalyst-buy 9-cat geopolitical + Hess $53B close · NUE 9sh @ $223 dual analyst PT cluster $244+$260) + **1 Harvest** (CVS stop $72.08 → $75.83 breakeven-lock at +9.84%). Daily cap met cleanly (2/2, $3,926 spend). 0 stops triggered. |
| Stop coverage | ✅ 9 active stops (BLK/CCI/CEG/CVS/MRK/MRVL/NKE/NVDA/TXN). ⚠️ CVX + NUE PDT-blocked, T+1 Friday morning |
| 🎯 Best held | NVDA +13.2% (semi cohort confirmed by today's TSM/MU/AVGO/INTC bull stack) · CEG +11.8% (AI-power utility thesis, +5.5% intraday best mover today) · CVS +9.8% (managed-care triple-bull, breakeven-locked today) |
| Day P&L | **+$244 / +0.98%** vs prior close $24,880.66 |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25124.38],
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
          handoverLine: {
            type: 'line',
            xMin: 'Mar 28',
            xMax: 'Mar 28',
            borderColor: '#f59e0b',
            borderWidth: 2,
            borderDash: [6, 4]
          },
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
| **Since Agents (Mar 28) — agent P&L only** | $20,489 | **~$22,124** | **+$1,635 (+8.0%)** | Excludes $3,000 Apr 23 deposit |
| 1 Month — agent P&L only | $23,448 | ~$22,124 | -5.6% | Excludes deposit; broader market context |
| Total equity (incl deposit) | $20,489 | $25,124 | +22.6% | Inflated by $3K Apr 23 deposit |
| **Today (Apr 30)** | $24,880 (Wed close) | $25,124 | **+0.98% (+$244)** | 2 BUYs (CVX + NUE), 1 Harvest stop-mod (CVS breakeven-lock) |
| Yesterday (Apr 29) | $24,910 (Tue close) | $24,880 | -0.12% (-$30) | FED day, 0 trades (cron-miss) |
| Low | $20,408 (Mar 31) | | | |
| High | $25,124 (Apr 30 close) | | | (incl deposit) — new high today |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$1,635 (+8.0% in 33 days)**, annualized ~88%. The total-equity chart includes a $3,000 deposit on Apr 23.

Orange dashed line = agents took control (Mar 28). Blue dashed line = sector-sleeve infrastructure deployed (Apr 23). Purple dot = $3K capital injection (Apr 23).

---

## Current Positions (post-close)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **NVDA** | 10 | $176.93 | $200.25 | +$233 | **+13.2%** 🎯 | 8.0% | $195 ✅ |
| **CEG** | 7 | $280.00 | $313.00 | +$231 | **+11.8%** 🎯 | 8.7% | $290 ✅ |
| **CVS** 🎯 | 27 | $75.83 | $83.29 | **+$201** | **+9.8%** 🎯 | 9.0% | **$75.83 ✅ (BREAKEVEN-LOCK Apr 30)** |
| **CCI** | 20 | $84.31 | $88.78 | +$89 | +5.3% | 7.1% | $80 ✅ |
| **TXN** | 5 | $272.83 | $280.71 | +$39 | +2.9% | 5.6% | $254 ✅ |
| **MRVL** | 9 | $159.54 | $163.30 | +$34 | +2.4% | 5.9% | $145 ✅ |
| **CVX 🆕** | 10 | $191.92 | $194.20 | +$23 | +1.2% | 7.7% | **$182 PENDING T+1 (PDT)** |
| **NUE 🆕** | 9 | $223.00 | $225.29 | +$21 | +1.0% | 8.1% | **$210 PENDING T+1 (PDT)** |
| BLK | 2 | $1,057.92 | $1,065.60 | +$15 | +0.7% | 8.5% | $990 ✅ |
| MRK | 18 | $112.47 | $109.18 | -$59 | -2.9% | 7.8% | $103.50 ✅ ⚠️ |
| NKE | 44 | $45.29 | $44.36 | -$41 | -2.0% | 7.8% | $42.50 ✅ TIGHT |
| BTC | 0.0034 | $70,867 | $76,309 | +$19 | **+7.7%** | 1.0% | — |
| UNH | 0.69 | $290.00 | $369.30 | +$55 | **+27.3%** | 1.0% | — |

**Total Open P&L: +$867 unrealized.** Today's day-change drivers: CEG +$112 intraday, MRVL +$61, CCI +$58, BLK +$52, TXN +$57; offset by NVDA -$90 intraday (semi rotation; structural thesis intact).

---

## ⭐ Sector Sleeve Status (post 04-28 INTC+LRCX stop-out)

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $6,281 (25%) | $4,876 (78%) | UNDER TARGET — dry powder available | NVDA, MRVL, TXN |

**Sleeve compression note:** INTC ($1,170) + LRCX ($1,036) stopped 04-28 = $2,206 capital returned to sleeve dry powder pool. Apr 30: no sleeve adds (CVX + NUE are general-bucket, not sleeve members). MU + INTC re-entry candidates for Friday queue.

**Cumulative sleeve P&L (history):**
- INTC: +$401 realized (Harvest 04-24) + closed at stop 04-28 = net **+$401**
- LRCX: closed at stop 04-28 = **-$86**
- MRVL: +$34 unrealized (held)
- TXN: +$39 unrealized (held)
- NVDA: +$66 realized (Harvest 04-27) + $233 unrealized = **+$299**
- **Total sleeve P&L all-time: ~+$687**

---

## Allocation (post-close)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (NVDA, MRVL, TXN) | $4,876 | 19.4% |
| Energy (CVX 🆕) | $1,942 | 7.7% |
| Materials (NUE 🆕) | $2,028 | 8.1% |
| Healthcare (MRK, CVS, UNH) | $4,469 | 17.8% |
| Financials (BLK) | $2,131 | 8.5% |
| Consumer (NKE) | $1,952 | 7.8% |
| Utility/Nuclear (CEG) | $2,191 | 8.7% |
| Real Estate (CCI) | $1,776 | 7.1% |
| Crypto (BTC) | $263 | 1.0% |
| **Cash** | **$3,497** | **13.9%** |

Nine sectors. Highest concentration: semi_ai sleeve at 19.4% (target 25%, room to add). New: Energy + Materials added today via CVX + NUE catalyst-buys.

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | NVDA | 10 | $195.00 | GTC | Trail-up post-trim 04-27 |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry; structural lock |
| **Stop** | **CVS** | **27** | **$75.83** | GTC | **🎯 BREAKEVEN-LOCK Apr 30** (was $72.08) |
| Stop | NKE | 44 | $42.50 | GTC | TIGHT buffer $1.86 |
| Stop | CCI | 20 | $80.00 | GTC | |
| Stop | MRK | 18 | $103.50 | GTC | ⚠️ Q1 LOSS Cidara qualifier 04-30 |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $254.00 | GTC | |
| **(pending)** | **CVX** | **10** | **$182** | GTC | **PDT-blocked, place Friday 9-10am ET** |
| **(pending)** | **NUE** | **9** | **$210** | GTC | **PDT-blocked, place Friday 9-10am ET** |

---

## Recently Closed (last 14 days)

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| **INTC** | $66.94 | $81.50 | **+$204 (+22.0%)** | Stop trigger Apr 28 (gap-down at open) |
| **LRCX** | $267.37 | $245.94 | **-$86 (-3.2%)** | Stop trigger Apr 28 (US Commerce Hua Hong tool-ban + cohort selloff) |
| **BA** | $222.99 | $227.87 | **+$44 (+2.2%)** | Stop trigger Apr 28 (Airbus Q1 mixed peer-cohort overwhelmed Copa 60-jet bull) |
| **NVDA (partial 04-27)** | $176.93 | $210.52 | **+$66 (+18.7%)** | Harvest trim 2 sh; remaining 10 sh +13.2% |
| **INTC (partial 04-24)** | $66.94 | $83.00 | **+$401 (+24.0%)** | Harvest trim 5 sh |
| **AEM** | $215.20 | $199.96 | -$152 (-7.1%) | Stop trigger Apr 23 |
| **NFLX** | $97.00 | $93.89 | -$68 (-3.2%) | Reaper sell Apr 21 (Hastings exit) |
| **MU** | $375.00 | ~$438 | +$315 (+16.8%) | Stop trigger Apr 20 (post Samsung-strike) |

---

## Today's Trades (2/2 daily cap used)

1. **CVX BUY** 10 sh @ limit $192.25 (filled $191.92) — catalyst-buy: 9-cat geopolitical bull stack culminating in $53B Hess acquisition CLOSE; Brent $115 + Trump-Iran-strike rhetoric + naval blockade; complementary geopolitical hedge to held NVDA AI thesis. Stop $182 PENDING T+1 (PDT-blocked).
2. **NUE BUY** 9 sh @ limit $223 (filled $223) — catalyst-buy: 5-cat bull stack (Q1 + 38% YTD + Wells Fargo PT $244 + Citigroup PT $260 + materials-cohort BHP/RIO/VALE iron-ore-China). Stop $210 PENDING T+1 (PDT-blocked).
3. **CVS HARVEST** stop replace $72.08 → $75.83 GTC — breakeven-lock triggered at +9.8% / 1.97R; locks in zero-loss; thesis target $90 still ~8% away (no qty trim).

---

## Friday (May 1) priority stack

1. **FIRST PRIORITY**: Place CVX stop $182 GTC + NUE stop $210 GTC at 9:00-10:00 ET (T+1 PDT cleared)
2. **TIER 1 BUY candidates** (after stop placement): MU (semi sleeve member, AI memory crunch direct beneficiary, sleeve cash-flex eligible if score ≥ 85) · GOOGL (biggest stock breakout since 2004 — resolves Thursday morning gap-defer logic) · TWLO (EXTREME Q2 EPS guide $2.50-2.60 vs $1.29 est, ~95% above consensus)
3. **TIER 2 backup**: INTC (HSBC PT $50→$95 sleeve specialty) · NFLX ($25B buyback re-entry candidate, was sold 04-21) · EQIX (Citi PT $1240 data-center REIT)
4. **Held position monitoring**:
   - NVDA HOLD AGGRESSIVE — semi cohort still STRONG (TSM/MU/AVGO bull alerts validate); 3R trim ~$203.48 if reached
   - CEG strong day +5.5% — monitor for 3R milestone Friday
   - CVS BREAKEVEN-LOCKED, target $90 still ~8% away
   - NKE buffer TIGHT $1.86; consumer cohort weak (stagflation discretionary headwind)
   - MRK Q1 LOSS Cidara qualifier; FY26 raise bull intact; HOLD with monitor

---

## Architecture / Cron note

**100% autopilot cron miss-or-late rate today** (morning +27 min, midday +30 min, close +30 min) — same pattern as 04-29 (FED day). Recommendation persists: reduce mercury_stream_market `*/8` → `*/12` OR move autopilot times to off-minute slots (:03/:33). Two consecutive trading days of structural cron failure to address before next trading session.
