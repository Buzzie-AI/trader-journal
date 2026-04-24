---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-24 10:05 AM ET (Friday intraday)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$24,921** |
| Cash | $3,776 (15.2%) |
| Invested | $21,145 (84.8%) |
| Positions | 13 equity + BTC + UNH fractional |
| Today's activity | **🎯 Biggest sleeve-validation day yet**: INTC +22% on Q1 beat · MRVL sleeve BUY 9sh @ $159.54 (the score-96 catalyst) · stops placed for LRCX $246 + INTC $70 breakeven-lock · BA stop trailed $205 → $223 (+1R breakeven-lock) |
| Stop coverage | ✅ All 10 equity positions stopped except MRVL (PDT-deferred to Apr 25) |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,24920.78],
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

| Period | Start | End | Change |
|--------|-------|-----|--------|
| 1 Month | $23,448 | $24,921 | **+6.3%** |
| Since Agents (Mar 28) | $20,489 | $24,921 | **+21.6%** |
| Last 2 days | $21,581 (Apr 22) | $24,921 | **+15.5%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,921 (Apr 24 intraday) | | |

Orange dashed line = agents took control (Mar 28). Blue dashed line = sector-sleeve infrastructure deployed (Apr 23). Apr 23→24 jump reflects INTC +22% on Q1 blowout + corporate-action realization on 737CVR019.

---

## Current Positions (intraday)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **INTC** | 19 | $66.94 | **$81.64** | **+$279** | **+22.0%** 🎯 | 6.2% | **$70 ✅ (breakeven-lock placed today)** |
| **MRVL 🆕** | 9 | $159.54 | $161.37 | +$17 | +1.2% | 5.8% | $145 (PDT pending, T+1 Apr 25) |
| NVDA | 12 | $177.28 | $202.16 | +$299 | **+14.0%** | 9.7% | $185 ✅ |
| BA | 9 | $222.99 | $233.03 | +$90 | **+4.5%** | 8.4% | **$223 ✅ (trailed today from $205)** |
| LRCX | 4 | $267.37 | $270.61 | +$13 | +1.2% | 4.3% | **$246 ✅ (placed today)** |
| MRK | 18 | $112.47 | $112.67 | +$4 | +0.2% | 8.1% | $103.50 ✅ |
| BLK | 2 | $1,057.92 | $1,049.12 | -$18 | -0.8% | 8.4% | $990 ✅ |
| CCI | 20 | $84.31 | $86.23 | +$38 | **+2.3%** | 6.9% | $80 ✅ |
| CEG | 7 | $280.00 | $294.16 | +$99 | **+5.1%** | 8.3% | $255 ✅ |
| CVS | 27 | $75.83 | $78.16 | +$63 | **+3.1%** | 8.5% | $72.08 ✅ |
| NKE | 44 | $45.29 | $45.34 | +$2 | +0.1% | 8.0% | $42.50 ✅ |
| BTC | 0.0034 | $70,867 | $77,982 | +$25 | **+10.0%** | 1.1% | — |
| UNH | 0.69 | $290.00 | $352.77 | +$43 | **+21.6%** | 1.0% | — |

**Total Open P&L: +$954** (vs +$832 at yesterday EOD). INTC alone +$279 unrealized.

---

## ⭐ Sector Sleeve Status (Day 2 of deployment)

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $6,230 (25%) | $6,512 (104.5%) | AT TARGET | NVDA, LRCX, INTC, **MRVL 🆕** |

**Day 2 validation:** Sleeve picker prioritized MRVL over general candidates this morning on the post-Apr-20 fade entry window. MRVL was the score-96 Google AI-chip partnership catalyst the old monolithic system systematically missed — the sleeve captured it on the second go-round. Combined with yesterday's INTC +14% Day 1 and now +22% Day 2, sleeve unrealized P&L at **+$608 across 4 positions** in 2 days.

**Sleeve regime signals today:** AMD DA Davidson PT $220→$375 (+70%), MRVL triple analyst upgrade, MXL multi-firm upgrade, INTC 52-week highs. All consistent with HOT regime thesis.

---

## Allocation (post-MRVL buy)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (NVDA, INTC, LRCX, MRVL) | $6,512 | 26.1% |
| Aerospace (BA) | $2,097 | 8.4% |
| Healthcare (MRK, CVS, UNH) | $4,381 | 17.6% |
| Financials (BLK) | $2,098 | 8.4% |
| Consumer (NKE) | $1,995 | 8.0% |
| Utility/Nuclear (CEG) | $2,059 | 8.3% |
| Real Estate (CCI) | $1,725 | 6.9% |
| Crypto (BTC) | $269 | 1.1% |
| **Cash** | **$3,776** | **15.2%** |

Eight sectors. Highest concentration: semi_ai sleeve at 26.1% (target 25%, max 35% with forced Harvest trim above).

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | NVDA | 12 | $185.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $255.00 | GTC | |
| Stop | CVS | 27 | $72.08 | GTC | |
| Stop | NKE | 44 | $42.50 | GTC | |
| Stop | CCI | 20 | $80.00 | GTC | |
| Stop | MRK | 18 | $103.50 | GTC | |
| **Stop** | **BA** | **9** | **$223** | GTC | **trailed today from $205 — +1R breakeven-lock rule** |
| **Stop** | **LRCX** | **4** | **$246** | GTC | **placed today (PDT-deferred from Apr 23)** |
| **Stop** | **INTC** | **19** | **$70** | GTC | **placed today at breakeven-lock (locks $58+ of +$279 gain)** |
| (pending) | **MRVL** | **9** | **$145** | GTC | To place Apr 25 morning (PDT same-day block) |

---

## Recently Closed (last 7 days)

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| AEM | $215.20 | $199.96 | -$152 (-7.1%) | Stop trigger Apr 23 open (gold-mining contagion + Iran/oil macro) |
| NFLX | $97.00 | $93.89 | -$68 (-3.2%) | Reaper sell Apr 21 (Hastings exit + soft Q1 guide) |
| MU | $375.00 | ~$438 | +$315 (+16.8%) | Stop trigger after Samsung-strike Mercury alert |
| PANW | $160.15 | $164.97 | +$58 (+3.0%) | Stop discipline WIN |
| DDOG | $119.00 | $104.95 | -$225 (-11.8%) | Stop discipline LOSS CUT |
| MRVL | $91.72 | $101.34 | +$173 (+10.5%) | Trailing stop WIN (pre-sleeve-era; re-bought today at $159.54) |

---

## This Week's Highlights

- **Apr 21:** Reaper-sell NFLX on thesis-break (Hastings exit) → realized -$68. MRK catalyst-buy 18 sh @ $112.47 (dual catalyst: Phase 3 + HIV approval).
- **Apr 22:** BA catalyst-buy 9 sh @ $222.99 on 5-catalyst stack (regulatory clearance + FCF guide pivot + record $695B backlog).
- **Apr 23:** **🎯 Sector-sleeve infrastructure DEPLOYED.** First-day validation: LRCX + INTC sleeve buys; INTC closed +13.82% on Q1 +29× EPS beat. AEM stopped out at open (-$152 realized).
- **Apr 24:** **🎯 Day 2 sleeve validation.** INTC opens +28% premarket, holds +22% intraday. MRVL re-entry (score-96 catalyst) at $159.54 — the fade-to-flat window the sleeve's `over_reacted` threshold override was designed to capture. LRCX $246 + INTC $70 breakeven-lock stops placed. BA stop trailed $205→$223 at +1R. **Portfolio +15.5% in 2 days.**

## Monday (Apr 28) priority stack

1. Place MRVL stop $145 GTC (T+1 PDT clear)
2. INTC Harvest trim 25% decision (locks $430+ realized gain; sleeve freed)
3. NVDA thesis check — Graviton/TPU custom-silicon narrative accumulating
4. BA at $234 approaching take-profit target $245 (+10%)
5. Fresh Mercury alerts from Apr 25-27 weekend

---

## Architecture note (fix deployed Apr 24)

Cron schedule adjusted after autopilot_morning was starved by hour-9 mercury fire overlap:
- `mercury_stream_off` cron narrowed to `*/5 4-8,16-20` (hour 9 dropped; was double-covered with mercury_stream_market)
- `autopilot_morning` shifted from 9:23 AM → **9:27 AM** to land in a clean `*/8` idle window

Today's MRVL sleeve-buy was executed manually at 09:49 ET after the 09:23 cron fire failed to deliver. Fix goes live tomorrow Monday morning.
