---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-10 10:20 AM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,227** |
| Cash | $10,779 (50.8%) |
| Invested | $10,448 (49.2%) |
| Positions | 5 stocks + BTC + UNH (PANW & DDOG stopped out) |

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
    labels: ["Mar 10","Mar 11","Mar 12","Mar 13","Mar 14","Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10"],
    datasets: [{
      label: 'Before Agents',
      data: [24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20959,20992,21342,21248,21227],
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
| 1 Month | $24,891 | $21,227 | **-14.7%** |
| Since Agents (Mar 28) | $20,489 | $21,227 | **+3.6%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| MU | 5 | $375.00 | $420.33 | +$226.66 | **+12.1%** | 9.9% | **$375 (breakeven)** |
| NVDA | 12 | $177.28 | $187.20 | +$119.02 | **+5.6%** | 10.6% | $160 |
| CEG | 7 | $280.00 | $287.28 | +$50.96 | **+2.6%** | 9.5% | $255 |
| CCI | 20 | $84.31 | $86.80 | +$49.80 | **+2.9%** | 8.2% | $76.50 |
| NKE | 44 | $45.29 | $43.02 | -$99.96 | -5.0% | 8.9% | $40 |
| BTC | 0.003 | $70,867 | $72,650 | +$6.15 | +2.5% | 1.2% | — |
| UNH | 0.69 | $290.00 | $309.43 | +$13.40 | **+6.7%** | 1.0% | — |

**Open P&L: +$366** | PANW & DDOG stopped out. Harvest locked MU at breakeven.

**Recently Closed:**

| Ticker | Entry | Exit | Return | Hold |
|--------|-------|------|--------|------|
| PANW | $160.15 | $164.97 | **+$57.84 (+3.0%)** | 11 days |
| DDOG | $119.00 | $104.95 | **-$224.80 (-11.8%)** | 11 days |
| MRVL | $91.72 | ~$101.34 | **+$173 (+10.5%)** | 3 days |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, MU) | $4,348 | 20.5% |
| Consumer (NKE) | $1,893 | 8.9% |
| Energy/Nuclear (CEG) | $2,011 | 9.5% |
| Real Estate (CCI) | $1,736 | 8.2% |
| Healthcare (UNH) | $213 | 1.0% |
| Crypto (BTC) | $251 | 1.2% |
| **Cash** | **$10,779** | **50.8%** |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Stop | NVDA | 12 | $160.00 | GTC |
| Stop | NKE | 44 | $40.00 | GTC |
| Stop | CEG | 7 | $255.00 | GTC |
| Stop | PANW | 12 | **$165.00** (TIGHTENED Apr 8) | GTC |
| Stop | DDOG | 16 | $105.00 | GTC |
| Stop | CCI | 20 | $76.50 | GTC |
| Stop | MU | 5 | **$340.00** (PLACED Apr 8) | GTC |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken, dead money |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis, dead money |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
