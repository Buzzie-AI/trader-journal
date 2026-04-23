---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-23 4:30 PM ET (Thursday EOD)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,789** |
| Cash | $2,212 (10.2%) |
| Invested | $19,577 (89.8%) |
| Positions | 11 stocks + BTC + UNH fractional |
| Today's activity | **🎯 First sleeve-routed trades**: BUY LRCX 4 sh @ $267.37 + INTC 19 sh @ $66.94 (semi_ai sleeve) · AEM stopped at $199.96 (-$152 realized) · BA stop $205 placed (PDT-deferred) |
| Stop coverage | ✅ All 9 equity positions stopped except LRCX/INTC (PDT-deferred to Apr 24) |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,21788.86],
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
| 1 Month | $23,448 | $21,789 | **-7.1%** |
| Since Agents (Mar 28) | $20,489 | $21,789 | **+6.3%** |
| Last 3 days | $21,664 (Apr 20) | $21,789 | **+0.6%** |
| Low | $20,408 (Mar 31) | | |
| High | $23,448 (Mar 17) | | |

Orange dashed line = agents took control (Mar 28). Blue dashed line = sector-sleeve infrastructure deployed (Apr 23).

---

## Current Positions (EOD)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **INTC 🆕** | **19** | **$66.94** | **$76.19** | **+$185** | **+13.82%** 🎯 | **6.7%** | **$61.60 (PDT pending)** |
| NVDA | 12 | $177.28 | $199.07 | +$261 | **+12.29%** | 11.0% | $185 ✅ |
| BA 🆕 | 9 | $222.99 | $233.95 | +$99 | **+4.91%** | 9.7% | $205 ✅ |
| **LRCX 🆕** | 4 | $267.37 | $259.00 | -$33 | -3.13% | 4.8% | $246 (PDT pending) |
| MRK 🆕 | 18 | $112.47 | $114.62 | +$39 | +1.91% | 9.5% | $103.50 ✅ |
| BLK | 2 | $1,057.92 | $1,052.55 | -$11 | -0.5% | 9.7% | $990 ✅ |
| CCI | 20 | $84.31 | $87.52 | +$64 | **+3.81%** | 8.0% | $80 ✅ |
| CEG | 7 | $280.00 | $292.40 | +$87 | **+4.43%** | 9.4% | $255 ✅ |
| CVS | 27 | $75.83 | $78.67 | +$77 | **+3.75%** | 9.8% | $72.08 ✅ |
| NKE | 44 | $45.29 | $45.15 | -$6 | -0.3% | 9.1% | $42.50 ✅ |
| BTC | 0.0034 | $70,867 | $78,028 | +$25 | **+10.10%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $353.50 | +$44 | **+21.90%** | 1.1% | — |

**Total Open P&L: +$832** (vs +$484 on Apr 20). INTC delivered +$185 unrealized on Day 1 of sleeve infrastructure after Q1 +29× EPS beat + Q2 guide raise.

---

## ⭐ NEW: Sector Sleeve Status (deployed Apr 23)

The portfolio now uses a **sector-sleeve** mechanism that reserves a portion of equity for tickers in a defined regime (currently AI/semiconductors).

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $5,447 (25%) | $4,883 (89.6%) | AT TARGET | NVDA, LRCX, INTC |

**How it works:** When the regime detector classifies semi_ai as HOT (≥5 qualifying alerts ≥70 in rolling 7-day window), semi candidates skip ahead in Phase A pipeline ranking. Without this priority routing, we would have selected TECK/TMO/ELV over INTC this morning — and missed the +13.82% INTC win on the same day.

[Full design rationale](https://github.com/Buzzie-AI/trader/blob/main/.claude/plans/fancy-mapping-scott.md) (private repo).

---

## Allocation (post-sleeve deployment)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (NVDA, INTC, LRCX) | $4,883 | 22.4% |
| Aerospace (BA) | $2,106 | 9.7% |
| Healthcare (MRK, CVS, UNH) | $4,431 | 20.3% |
| Financials (BLK) | $2,105 | 9.7% |
| Consumer (NKE) | $1,987 | 9.1% |
| Utility/Nuclear (CEG) | $2,047 | 9.4% |
| Real Estate (CCI) | $1,750 | 8.0% |
| Crypto (BTC) | $269 | 1.2% |
| **Cash** | **$2,212** | **10.2%** |

Eight sectors. Highest concentration: semi_ai sleeve at 22.4% (target 25%, max 35% with forced Harvest trim above).

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | NVDA | 12 | $185.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $255.00 | GTC | |
| Stop | CVS | 27 | $72.08 | GTC | (trailed up from $72.75) |
| Stop | NKE | 44 | $42.50 | GTC | |
| Stop | CCI | 20 | $80.00 | GTC | |
| Stop | MRK | 18 | $103.50 | GTC | (placed Apr 22 after PDT-deferred) |
| Stop | BA | 9 | $205.00 | GTC | (placed Apr 23 after PDT-deferred) |
| (pending) | **LRCX** | **4** | **$246** | **GTC** | To place Apr 24 morning (PDT same-day block) |
| (pending) | **INTC** | **19** | **$61.60** | **GTC** | To place Apr 24 morning (could trail to ~$70 to lock gains) |

---

## Recently Closed (last 7 days)

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| **AEM** | $215.20 | **$199.96** | **-$152 (-7.1%)** | Stop trigger Apr 23 open (gold-mining contagion + Iran/oil macro) |
| NFLX | $97.00 | $93.89 | -$68 (-3.2%) | Reaper sell Apr 21 (Hastings exit + soft Q1 guide) |
| MU | $375.00 | ~$438 | +$315 (+16.8%) | Stop trigger after Samsung-strike Mercury alert |
| PANW | $160.15 | $164.97 | +$58 (+3.0%) | Stop discipline WIN |
| DDOG | $119.00 | $104.95 | -$225 (-11.8%) | Stop discipline LOSS CUT |
| MRVL | $91.72 | $101.34 | +$173 (+10.5%) | Trailing stop WIN |

---

## This Week's Highlights

- **Apr 21:** Reaper-sell NFLX on thesis-break (Hastings exit) → realized -$68. MRK catalyst-buy 18 sh @ $112.47 (dual catalyst: Phase 3 + HIV approval).
- **Apr 22:** BA catalyst-buy 9 sh @ $222.99 on 5-catalyst stack (regulatory clearance + FCF guide pivot + record $695B backlog).
- **Apr 23:** **🎯 Sector-sleeve infrastructure DEPLOYED.** First-day validation: LRCX + INTC sleeve buys; INTC closed +13.82% on Q1 +29× EPS beat. AEM stopped out at open (-$152 realized).

## Tomorrow (Apr 24) priority stack

1. Place LRCX stop $246 GTC (T+1 PDT)
2. Place INTC stop ($61.60 standard or trail to $70 to lock $60 of $185 gain)
3. Trail BA stop $205 → $215-220 (Harvest breakeven-lock at +1R)
4. Evaluate INTC trim partial vs let it ride after-bell catalyst stack
5. General candidates carry-over: TECK, TMO, ELV, REGN (now caveated with MFN), NEM, DLR, EW
