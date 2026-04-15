---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-15 4:30 PM ET (EOD close)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,644** |
| Cash | $6,616 (30.5%) |
| Invested | $15,028 (69.5%) |
| Positions | 7 stocks + BTC + UNH fractional |
| Today's trade | **CVS BUY** 27 sh @ $75.83 (AM); no action this EOD run |
| CVS stop status | ⚠️ $72.75 PENDING — PDT same-day block, retry post-8 PM ET |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45],
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
| 1 Month | $23,448 | $21,679 | **-7.5%** |
| Since Agents (Mar 28) | $20,489 | $21,679 | **+5.8%** |
| Low | $20,408 (Mar 31) | | |
| High | $23,448 (Mar 17) | | |

---

## Current Positions (EOD close)

| Ticker | Shares | Entry | Close | P&L | P&L % | Weight | Stop |
|--------|--------|-------|-------|-----|-------|--------|------|
| MU | 5 | $375.00 | $453.43 | +$392.15 | **+20.9%** | 10.5% | **$438** (Harvest 2x) |
| NVDA | 12 | $177.28 | $198.34 | +$252.69 | **+11.9%** | 11.0% | **$185** (Harvest 2x) |
| BLK | 2 | $1057.92 | $1049.00 | -$17.84 | -0.8% | 9.7% | **$990** ✅ |
| CEG | 7 | $280.00 | $294.99 | +$104.93 | **+5.4%** | 9.5% | $255 |
| **CVS** | **27** | **$75.83** | **$74.99** | **-$16.43** | **-1.1%** | **9.4%** | **$72.75** ⚠️ pending |
| NKE | 44 | $45.29 | $45.48 | +$8.50 | +0.4% | 9.2% | $40 |
| CCI | 20 | $84.31 | $85.63 | +$26.40 | +1.6% | 7.9% | $76.50 |
| BTC | 0.003 | $70,867 | $74,667 | +$13.11 | **+5.4%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $314.09 | +$16.28 | **+8.3%** | 1.0% | — |

**Open P&L: +$779** | Day P&L: -$35 (flat). Tech-led rally offset by healthcare/industrial weakness. MU -2.6%, CVS -3.1%, NKE +2.9%.

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, MU) | $4,647 | 21.5% |
| **Healthcare (CVS + UNH)** | **$2,247** | **10.4%** |
| Financials (BLK) | $2,098 | 9.7% |
| Utility/Nuclear (CEG) | $2,065 | 9.5% |
| Consumer (NKE) | $2,001 | 9.2% |
| Real Estate (CCI) | $1,713 | 7.9% |
| Crypto (BTC) | $258 | 1.2% |
| **Cash** | **$6,616** | **30.5%** |

Seven sectors represented. No concentration over 22%. Healthcare added today via CVS.

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | MU | 5 | $438.00 | GTC | Harvest 2x advance |
| Stop | NVDA | 12 | $185.00 | GTC | Harvest 2x advance |
| Stop | BLK | 2 | $990.00 | GTC | Placed EOD Apr 14 |
| Stop | CEG | 7 | $255.00 | GTC | |
| Stop | NKE | 44 | $40.00 | GTC | |
| Stop | CCI | 20 | $76.50 | GTC | |
| **Stop** | **CVS** | **27** | **$72.75** | **GTC** | **PENDING — PDT same-day block, next run** |

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
