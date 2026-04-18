---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-17 10:00 PM ET (Friday EOD)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,855** |
| Cash | $4,482 (20.5%) |
| Invested | $17,373 (79.5%) |
| Positions | 8 stocks + BTC + UNH fractional |
| Today's trade | BUY NFLX 22 sh @ $97 (post-earnings dip-buy) |
| Stop coverage | ✅ **All 8 equity positions stop-protected** (NFLX $93.50 placed 9:59 PM) |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21855],
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
| 1 Month | $23,448 | $21,855 | **-6.8%** |
| Since Agents (Mar 28) | $20,489 | $21,855 | **+6.7%** |
| Low | $20,408 (Mar 31) | | |
| High | $23,448 (Mar 17) | | |

---

## Current Positions (Intraday)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| MU | 5 | $375.00 | $452.70 | +$388.50 | **+20.7%** | 10.4% | **$438** (Harvest 2x) |
| NVDA | 12 | $177.28 | $200.98 | +$284.40 | **+13.4%** | 11.0% | **$185** (Harvest 2x) |
| NFLX | 22 | $97.00 | $97.29 | +$6.38 | **+0.3%** | 9.8% | $93.50 ✅ |
| BLK | 2 | $1057.92 | $1,052 | -$11.84 | -0.6% | 9.6% | **$990** ✅ |
| CEG | 7 | $280.00 | $296.10 | +$112.70 | **+5.7%** | 9.6% | $255 (⚠️ 1R at $305) |
| CVS | 27 | $75.83 | $77.30 | +$39.69 | **+1.9%** | 9.5% | $72.75 ✅ |
| NKE | 44 | $45.29 | $46.13 | +$36.96 | **+1.9%** | 9.3% | $40 |
| CCI | 20 | $84.31 | $88.71 | +$88.00 | **+5.2%** | 8.0% | $76.50 |
| BTC | 0.003 | $70,867 | $77,229 | +$19.09 | **+9.0%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $324.00 | +$23.46 | **+11.7%** | 1.0% | — |

**Open P&L: +$987** | Friday EOD: NFLX stop placed at 9:59 PM. All 8 positions protected for the weekend. Broad rally: SPY +0.9%.

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, MU) | $4,721 | 21.6% |
| **Communication (NFLX)** | **$2,134** | **9.8%** |
| Healthcare (CVS + UNH) | $2,288 | 10.5% |
| Financials (BLK) | $2,085 | 9.6% |
| Utility/Nuclear (CEG) | $2,086 | 9.6% |
| Consumer (NKE) | $2,019 | 9.3% |
| Real Estate (CCI) | $1,742 | 8.0% |
| Crypto (BTC) | $230 | 1.2% |
| **Cash** | **$4,482** | **20.5%** |

Eight sectors represented. No concentration over 22%. Communication Services added today via NFLX.

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | MU | 5 | $438.00 | GTC | Harvest 2x advance |
| Stop | NVDA | 12 | $185.00 | GTC | Harvest 2x advance |
| Stop | BLK | 2 | $990.00 | GTC | Placed EOD Apr 14 |
| Stop | CEG | 7 | $255.00 | GTC | |
| Stop | CVS | 27 | $72.75 | GTC | |
| Stop | NKE | 44 | $40.00 | GTC | |
| Stop | CCI | 20 | $76.50 | GTC | |
| Stop | NFLX | 22 | $93.50 | GTC | Placed 9:59 PM ET ✅ |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| PANW | $160.15 | $164.97 | **+$57.84 (+3.0%)** | Stop discipline WIN (11d) |
| DDOG | $119.00 | $104.95 | **-$224.80 (-11.8%)** | Stop discipline LOSS CUT (11d) |
| MRVL | $91.72 | $101.34 | **+$173 (+10.5%)** | Trailing stop WIN (3d) |
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
