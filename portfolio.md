---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-07 9:36 AM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$20,864** |
| Cash | $7,120 (34.1%) |
| Invested | $13,744 (65.9%) |
| Positions | 7 stocks + BTC + UNH |

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
    labels: ["Mar 3","Mar 4","Mar 5","Mar 6","Mar 7","Mar 10","Mar 11","Mar 12","Mar 13","Mar 14","Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7"],
    datasets: [{
      label: 'Before Agents',
      data: [24890.95,24230.91,24671.71,24750.11,23803.58,24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20959,20864],
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
| 1 Month | $24,891 | $20,864 | **-16.2%** |
| Since Agents (Mar 28) | $20,489 | $20,864 | **+1.8%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $176.02 | -$15.21 | -0.7% | 10.1% | $160 |
| MU | 5 | $375.00 | $376.99 | +$9.95 | **+0.5%** | 9.0% | $340 (pending) |
| PANW | 12 | $160.15 | $161.54 | +$16.68 | **+0.9%** | 9.3% | $148 |
| NKE | 44 | $45.29 | $43.40 | -$83.24 | -4.2% | 9.2% | $40 |
| CEG | 7 | $280.00 | $272.56 | -$52.08 | -2.7% | 9.1% | $255 |
| DDOG | 16 | $119.00 | $115.00 | -$64.00 | -3.4% | 8.8% | $105 |
| CCI | 20 | $84.31 | $85.60 | +$25.80 | **+1.5%** | 8.2% | $76.50 |
| BTC | 0.003 | $70,867 | $68,418 | -$8.45 | -3.5% | 1.1% | — |
| UNH | 0.69 | $290.00 | $306.12 | +$11.11 | **+5.6%** | 1.0% | — |

**MU filled Apr 7** at $375.00 (better than $378.47 limit). [Thesis](/theses/2026-04-06-MU-dip-buy)

**Recently Closed:**

| Ticker | Entry | Exit | Return | Hold |
|--------|-------|------|--------|------|
| MRVL | $91.72 | ~$101.34 | **+$173 (+10.5%)** | 3 days |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, PANW, DDOG, MU) | $7,775 | 37.3% |
| Consumer (NKE) | $1,909 | 9.2% |
| Energy (CEG) | $1,908 | 9.1% |
| Real Estate (CCI) | $1,712 | 8.2% |
| Healthcare (UNH) | $211 | 1.0% |
| Crypto (BTC) | $236 | 1.1% |
| **Cash** | **$7,120** | **34.1%** |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Stop | NVDA | 12 | $160.00 | GTC |
| Stop | NKE | 44 | $40.00 | GTC |
| Stop | CEG | 7 | $255.00 | GTC |
| Stop | PANW | 12 | $148.00 | GTC |
| Stop | DDOG | 16 | $105.00 | GTC |
| Stop | CCI | 20 | $76.50 | GTC |
| Stop (pending) | MU | 5 | $340 (PDT — place tomorrow) | — |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken, dead money |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis, dead money |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
