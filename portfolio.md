---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-20 4:30 PM ET (Monday EOD)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,664** |
| Cash | $4,520 (20.9%) |
| Invested | $17,144 (79.1%) |
| Positions | 9 stocks + BTC + UNH fractional |
| Today's activity | BUY AEM 10 sh @ $215.20 (autopilot midday, gold M&A acquirer-dip) · MU stopped-out at $438 (+16.8% locked) |
| Stop coverage | ⚠️ **9 of 9 equity positions stopped EXCEPT new AEM** (stop pending tomorrow per PDT same-day-block) |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63],
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
| 1 Month | $23,448 | $21,664 | **-7.6%** |
| Since Agents (Mar 28) | $20,489 | $21,664 | **+5.7%** |
| Low | $20,408 (Mar 31) | | |
| High | $23,448 (Mar 17) | | |

---

## Current Positions (EOD)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $202.00 | +$296.61 | **+13.9%** | 11.2% | **$185** (Harvest 2x) |
| AEM 🆕 | 10 | $215.20 | $216.39 | +$11.87 | +0.6% | 10.0% | pending tomorrow |
| NFLX | 22 | $97.00 | $94.64 | -$51.92 | **-2.4%** | 9.6% | **$93.50 (⚠️ 1.2% above)** |
| BLK | 2 | $1,057.92 | $1,050 | -$15.84 | -0.7% | 9.7% | **$990** ✅ |
| NKE | 44 | $45.29 | $46.50 | +$53.32 | **+2.7%** | 9.4% | $42.50 |
| CVS | 27 | $75.83 | $76.58 | +$20.29 | **+1.0%** | 9.5% | $72.75 ✅ |
| CEG | 7 | $280.00 | $288.92 | +$62.46 | **+3.2%** | 9.3% | $255 |
| CCI | 20 | $84.31 | $87.56 | +$65.00 | **+3.9%** | 8.1% | $80 |
| BTC | 0.003 | $70,867 | $76,240 | +$18.54 | **+7.6%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $324.59 | +$23.86 | **+11.9%** | 1.0% | — |

**Open P&L: +$484** | Today: MU closed at +20.7% (stopped out at $438), AEM bought as catalyst-buy. NFLX is the watchpoint — Reed Hastings exit + soft guidance, $1.14 above stop.

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA) | $2,424 | 11.2% |
| **Materials (AEM)** 🆕 | **$2,164** | **10.0%** |
| Communication (NFLX) | $2,082 | 9.6% |
| Financials (BLK) | $2,100 | 9.7% |
| Consumer (NKE) | $2,046 | 9.4% |
| Healthcare (CVS + UNH) | $2,291 | 10.6% |
| Utility/Nuclear (CEG) | $2,022 | 9.3% |
| Real Estate (CCI) | $1,751 | 8.1% |
| Crypto (BTC) | $263 | 1.2% |
| **Cash** | **$4,520** | **20.9%** |

Nine sectors represented. No concentration over 12%. **Materials added today via AEM** (gold M&A catalyst-buy).

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | NVDA | 12 | $185.00 | GTC | Harvest 2x advance |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $255.00 | GTC | |
| Stop | CVS | 27 | $72.75 | GTC | |
| Stop | NKE | 44 | $42.50 | GTC | |
| Stop | CCI | 20 | $80.00 | GTC | |
| Stop | NFLX | 22 | $93.50 | GTC | **⚠️ 1.2% above current $94.64** |
| (pending) | **AEM** | **10** | **$200** | **GTC** | **To be placed tomorrow morning (PDT same-day block)** |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| MU | $375.00 | ~$438 | **+$315 (+16.8%)** | Stop trigger after Samsung-strike Mercury alert (14d) |
| PANW | $160.15 | $164.97 | **+$57.84 (+3.0%)** | Stop discipline WIN (11d) |
| DDOG | $119.00 | $104.95 | **-$224.80 (-11.8%)** | Stop discipline LOSS CUT (11d) |
| MRVL | $91.72 | $101.34 | **+$173 (+10.5%)** | Trailing stop WIN (3d) |
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |

---

## This Week's Catalysts (from Oracle)

| Date | Event | Relevance |
|------|-------|-----------|
| **Apr 21 (AMC)** | ISRG Q1 earnings | Watchlist candidate post-earnings |
| **Apr 21-22** | 🚨 Iran ceasefire EXPIRES — binary | No energy exposure. XLE hedge considered |
| **Apr 22 (AMC)** | TSLA + GEV earnings | No position |
| **Apr 28** | FOMC + MSFT earnings start | CCI rate-sensitive; CEG pre-earn trim fires |
| **~Apr 30** | CVS earnings (date unverified) | Pre-earn trim would fire Apr 23 if confirmed |
| **May 5** | CEG earnings | Pre-earn trim fires Apr 28 |

*Oracle calendar last rebuilt Apr 16; refresh due.*
