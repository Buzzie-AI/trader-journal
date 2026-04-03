---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-03 10:13 AM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$20,970** |
| Cash | $10,681 (51.0%) → ~$8,981 after CCI fill |
| Invested | $10,288 (49.0%) → ~$11,988 after CCI fill |
| Positions | 6 stocks + BTC + UNH (CCI pending fill) |

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
    labels: ["Mar 3","Mar 4","Mar 5","Mar 6","Mar 7","Mar 10","Mar 11","Mar 12","Mar 13","Mar 14","Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2"],
    datasets: [{
      label: 'Before Agents',
      data: [24890.95,24230.91,24671.71,24750.11,23803.58,24457.18,24512.53,24386.63,23710.33,23106.55,23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12],
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
| 1 Month | $24,891 | $20,970 | **-15.7%** |
| Since Agents (Mar 28) | $20,489 | $20,970 | **+2.3%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| NVDA | 12 | $177.28 | $177.31 | +$0.29 | **+0.0%** | 10.1% | $160 |
| PANW | 12 | $160.15 | $163.27 | +$37.44 | **+1.9%** | 9.3% | $148 |
| NKE | 44 | $45.29 | $44.19 | -$48.26 | -2.4% | 9.3% | $40 |
| DDOG | 16 | $119.00 | $120.36 | +$21.76 | **+1.1%** | 9.2% | $105 |
| CEG | 7 | $280.00 | $272.64 | -$51.52 | -2.6% | 9.1% | $255 |
| CCI | 20 | $84.94 | $84.77 | PENDING | PENDING | ~8.1% | $76.50 (pending) |
| BTC | 0.003 | $70,867 | $66,697 | -$14.39 | -5.9% | 1.1% | — |
| UNH | 0.69 | $290.00 | $277.23 | -$8.79 | -4.4% | 0.9% | — |

**New trade (Apr 3):** BUY 20 CCI @ $84.94 limit — activist-backed tower REIT restructuring. [Thesis](/theses/2026-04-03-CCI-momentum-buy)

**Recently Closed:**

| Ticker | Entry | Exit | Return | Hold |
|--------|-------|------|--------|------|
| MRVL | $91.72 | ~$101.34 | **+$173 (+10.5%)** | 3 days |

---

## Allocation

| Category | Value | Weight |
|----------|-------|--------|
| Tech (NVDA, DDOG, PANW) | $6,013 | 28.7% |
| Consumer (NKE) | $1,944 | 9.3% |
| Energy (CEG) | $1,910 | 9.1% |
| Real Estate (CCI) | ~$1,700 | ~8.1% (pending) |
| Healthcare (UNH) | $191 | 0.9% |
| Crypto (BTC) | $230 | 1.1% |
| **Cash** | **~$8,981** | **~42.8%** |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Stop | NVDA | 12 | $160.00 | GTC |
| Stop | NKE | 44 | $40.00 | GTC |
| Stop | CEG | 7 | $255.00 | GTC |
| Stop | PANW | 12 | $148.00 | GTC |
| Stop | DDOG | 16 | $105.00 | GTC |
| Limit Buy | CCI | 20 | $84.94 | Day |
| Stop (pending) | CCI | 20 | $76.50 (after buy fills) | — |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken, dead money |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis, dead money |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
