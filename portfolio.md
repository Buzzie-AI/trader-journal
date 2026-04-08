---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-08 9:35 AM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,549** |
| Cash | $7,120 (33.0%) |
| Invested | $14,429 (67.0%) |
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
    labels: ["Mar 6","Mar 7","Mar 10","Mar 11","Mar 12","Mar 13","Mar 14","Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8"],
    datasets: [{
      label: 'Before Agents',
      data: [24750.11,23803.58,24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20959,20992,21549],
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
| 1 Month | $24,891 | $21,549 | **-13.4%** |
| Since Agents (Mar 28) | $20,489 | $21,549 | **+5.2%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $183.60 | +$75.81 | **+3.6%** | 10.2% | $160 |
| PANW | 12 | $160.15 | $176.03 | +$190.56 | **+9.9%** | 9.8% | **$165 (TIGHTENED)** |
| MU | 5 | $375.00 | $409.94 | +$174.70 | **+9.3%** | 9.5% | **$340 (PLACED)** |
| CEG | 7 | $280.00 | $286.14 | +$42.98 | **+2.2%** | 9.3% | $255 |
| DDOG | 16 | $119.00 | $121.53 | +$40.48 | **+2.1%** | 9.0% | $105 |
| NKE | 44 | $45.29 | $43.64 | -$72.46 | -3.6% | 8.9% | $40 |
| CCI | 20 | $84.31 | $85.16 | +$17.00 | **+1.0%** | 7.9% | $76.50 |
| BTC | 0.003 | $70,867 | $72,272 | +$4.85 | **+2.0%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $312.09 | +$15.23 | **+7.6%** | 1.0% | — |

**Open P&L: +$489** | **Win rate: 6/7 (86%)** | All stops in place. PANW target hit. Massive rally day.

**Recently Closed:**

| Ticker | Entry | Exit | Return | Hold |
|--------|-------|------|--------|------|
| MRVL | $91.72 | ~$101.34 | **+$173 (+10.5%)** | 3 days |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, PANW, DDOG, MU) | $8,310 | 38.6% |
| Consumer (NKE) | $1,920 | 8.9% |
| Energy/Nuclear (CEG) | $2,003 | 9.3% |
| Real Estate (CCI) | $1,703 | 7.9% |
| Healthcare (UNH) | $215 | 1.0% |
| Crypto (BTC) | $249 | 1.2% |
| **Cash** | **$7,120** | **33.0%** |

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
