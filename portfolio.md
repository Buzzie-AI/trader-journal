---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-01*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,153** |
| Cash | $8,699 |
| Invested | $12,454 |
| Positions | 9 |
| Day P&L | +$267 (+1.28%) |

---

## Equity Curve (1 Month)

<div style="width:100%;overflow-x:auto">
<canvas id="equityChart" width="800" height="300"></canvas>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
const ctx = document.getElementById('equityChart').getContext('2d');
new Chart(ctx, {
  type: 'line',
  data: {
    labels: ["03-03","03-04","03-05","03-06","03-07","03-10","03-11","03-12","03-13","03-14","03-17","03-18","03-19","03-20","03-21","03-24","03-25","03-26","03-27","03-28","03-31","04-01"],
    datasets: [{
      label: 'Portfolio Equity ($)',
      data: [24890.95,24230.91,24671.71,24750.11,23803.58,24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,20408.39,20886.27],
      borderColor: '#2563eb',
      backgroundColor: 'rgba(37,99,235,0.1)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#2563eb'
    }]
  },
  options: {
    responsive: true,
    plugins: {
      legend: { display: false },
      tooltip: {
        callbacks: {
          label: function(ctx) { return '$' + ctx.parsed.y.toLocaleString(); }
        }
      }
    },
    scales: {
      y: {
        ticks: { callback: function(v) { return '$' + (v/1000).toFixed(1) + 'k'; } },
        min: 19000,
        max: 26000
      }
    }
  }
});
</script>

| Period | Start | End | Change |
|--------|-------|-----|--------|
| 1 Month | $24,891 | $20,886 | **-16.1%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $177.08 | -$2.49 | -0.1% | 10.0% | — |
| MRVL | 18 | $91.72 | $106.01 | **+$257.19** | **+15.6%** | 9.0% | $98.22 (trail 6%) |
| CEG | 7 | $280.00 | $281.92 | +$13.44 | +0.7% | 9.3% | $255 (pending) |
| DDOG | 16 | $119.00 | $121.06 | +$32.96 | +1.7% | 9.2% | $105 |
| PANW | 12 | $160.15 | $160.18 | +$0.36 | 0.0% | 9.1% | $148 |
| HOOD | 25 | $126.69 | $70.94 | -$1,393.68 | **-44.0%** | 8.4% | $58 |
| HNGE | 10 | $45.67 | $38.79 | -$68.80 | -15.1% | 1.8% | — |
| BTCUSD | 0.003 | $70,867 | $68,896 | -$6.80 | -2.8% | 1.1% | — |
| UNH | 0.69 | $290.00 | $273.72 | -$11.23 | -5.6% | 0.9% | — |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, DDOG, MRVL, PANW) | $7,892 | 37.3% |
| Energy (CEG) | $1,973 | 9.3% |
| Fintech (HOOD) | $1,774 | 8.4% |
| Healthcare (UNH) | $189 | 0.9% |
| Crypto (BTC) | $238 | 1.1% |
| Cash | $8,699 | 41.1% |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Trailing Stop | MRVL | 18 | $98.22 (6% trail, HWM $104.49) | GTC |
| Stop | DDOG | 16 | $105.00 | GTC |
| Stop | PANW | 12 | $148.00 | GTC |
| Stop | HOOD | 25 | $58.00 | GTC |
| Stop | CEG | 7 | $255.00 (PENDING — PDT blocked) | — |
