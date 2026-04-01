---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-01 1:46 PM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,142** |
| Cash | $8,857 (41.9%) |
| Invested | $12,286 (58.1%) |
| Positions | 8 |

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
    labels: ["Mar 3","Mar 4","Mar 5","Mar 6","Mar 7","Mar 10","Mar 11","Mar 12","Mar 13","Mar 14","Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1"],
    datasets: [{
      label: 'Before Agents',
      data: [24890.95,24230.91,24671.71,24750.11,23803.58,24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27],
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
| 1 Month | $24,891 | $21,142 | **-15.1%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $176.44 | -$10.11 | -0.5% | 10.0% | — |
| NKE | 44 | $45.29 | $45.34 | +$2.12 | +0.1% | 9.4% | $40 (pending) |
| CEG | 7 | $280.00 | $283.32 | +$23.24 | +1.2% | 9.4% | $255 (PDT blocked) |
| MRVL | 18 | $91.72 | $106.93 | **+$273.66** | **+16.6%** | 9.1% | $101.37 (trail 6%) |
| PANW | 12 | $160.15 | $160.81 | +$7.86 | +0.4% | 9.1% | $148 |
| DDOG | 16 | $119.00 | $119.43 | +$6.88 | +0.4% | 9.0% | $105 |
| BTC | 0.003 | $70,867 | $68,418 | -$8.45 | -3.5% | 1.1% | — |
| UNH | 0.69 | $290.00 | $274.77 | -$10.50 | -5.3% | 0.9% | — |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, DDOG, MRVL, PANW) | $7,883 | 37.3% |
| **Consumer (NKE)** | **$1,995** | **9.4%** |
| Energy (CEG) | $1,983 | 9.4% |
| Healthcare (UNH) | $189 | 0.9% |
| Crypto (BTC) | $236 | 1.1% |
| Cash | $8,857 | 41.9% |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Trailing Stop | MRVL | 18 | $101.37 (6% trail, HWM $107.84) | GTC |
| Stop | DDOG | 16 | $105.00 | GTC |
| Stop | PANW | 12 | $148.00 | GTC |
| Stop | NKE | 44 | $40.00 (PENDING after fill) | — |
| Stop | CEG | 7 | $255.00 (PENDING — PDT blocked) | — |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken, dead money |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis, dead money |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
