---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-09 11:34 AM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,314** |
| Cash | $7,120 (33.4%) |
| Invested | $14,194 (66.6%) |
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
    labels: ["Mar 7","Mar 10","Mar 11","Mar 12","Mar 13","Mar 14","Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9"],
    datasets: [{
      label: 'Before Agents',
      data: [23803.58,24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20959,20992,21549,21314],
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
| 1 Month | $24,891 | $21,314 | **-14.4%** |
| Since Agents (Mar 28) | $20,489 | $21,314 | **+4.0%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $183.26 | +$71.73 | **+3.4%** | 10.3% | $160 |
| MU | 5 | $375.00 | $407.00 | +$160.00 | **+8.5%** | 9.5% | $340 |
| PANW | 12 | $160.15 | $167.66 | +$90.09 | **+4.7%** | 9.4% | **$165 (1.6% away)** |
| CEG | 7 | $280.00 | $292.67 | +$88.66 | **+4.5%** | 9.6% | $255 |
| CCI | 20 | $84.31 | $87.05 | +$54.80 | **+3.3%** | 8.2% | $76.50 |
| DDOG | 16 | $119.00 | $112.05 | -$111.20 | **-5.8%** | 8.4% | $105 |
| NKE | 44 | $45.29 | $43.39 | -$83.46 | -4.2% | 9.0% | $40 |
| BTC | 0.003 | $70,867 | $71,398 | +$1.83 | +0.7% | 1.2% | — |
| UNH | 0.69 | $290.00 | $306.32 | +$11.26 | **+5.6%** | 1.0% | — |

**Open P&L: +$284** | Win rate: 6/7 (86%) | CPI report tomorrow — CCI directly exposed, PANW stop in danger zone.

**Recently Closed:**

| Ticker | Entry | Exit | Return | Hold |
|--------|-------|------|--------|------|
| MRVL | $91.72 | ~$101.34 | **+$173 (+10.5%)** | 3 days |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, PANW, DDOG, MU) | $8,039 | 37.7% |
| Consumer (NKE) | $1,909 | 9.0% |
| Energy/Nuclear (CEG) | $2,049 | 9.6% |
| Real Estate (CCI) | $1,741 | 8.2% |
| Healthcare (UNH) | $211 | 1.0% |
| Crypto (BTC) | $246 | 1.2% |
| **Cash** | **$7,120** | **33.4%** |

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
