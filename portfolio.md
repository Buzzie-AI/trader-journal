---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-14 10:30 AM ET*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,452** |
| Cash | $10,779 (50.2%) → ~$8,655 after BLK fill |
| Invested | $10,673 (49.8%) → ~$12,797 after BLK fill |
| Positions | 6 stocks + BTC + UNH (BLK pending fill) |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21452],
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
| 1 Month | $24,891 | $21,452 | **-13.8%** |
| Since Agents (Mar 28) | $20,489 | $21,452 | **+4.7%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Current | P&L | P&L % | Weight | Stop |
|--------|--------|-------|---------|-----|-------|--------|------|
| MU | 5 | $375.00 | $440.38 | +$326.90 | **+17.4%** | 10.3% | **$420** (Harvest tightened) |
| NVDA | 12 | $177.28 | $192.65 | +$184.41 | **+8.7%** | 10.8% | **$178** (Harvest breakeven) |
| CEG | 7 | $280.00 | $294.75 | +$103.25 | **+5.3%** | 9.6% | $255 |
| BLK | 2 | $1062.00 | $1060.02 | PENDING | PENDING | 9.9% | $990 (pending) |
| CCI | 20 | $84.31 | $85.70 | +$27.80 | **+1.6%** | 8.0% | $76.50 |
| NKE | 44 | $45.29 | $43.32 | -$86.76 | -4.4% | 8.9% | $40 |
| BTC | 0.003 | $70,867 | $75,725 | +$16.76 | **+6.9%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $318.03 | +$19.33 | **+9.7%** | 1.0% | — |

**Open P&L: +$591** | New trade: BUY 2 BLK on Q1 earnings beat. Harvest tightened MU and NVDA stops.

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
| Tech (NVDA, MU) | $4,514 | 21.0% |
| Financials (BLK) | $2,124 | 9.9% (pending) |
| Energy/Nuclear (CEG) | $2,063 | 9.6% |
| Consumer (NKE) | $1,906 | 8.9% |
| Real Estate (CCI) | $1,714 | 8.0% |
| Healthcare (UNH) | $219 | 1.0% |
| Crypto (BTC) | $261 | 1.2% |
| **Cash** | **~$8,655** | **~40.3%** (post-fill) |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Stop | MU | 5 | **$420** (Harvest tightened from $400) | GTC |
| Stop | NVDA | 12 | **$178** (Harvest breakeven lock from $160) | GTC |
| Stop | NKE | 44 | $40.00 | GTC |
| Stop | CEG | 7 | $255.00 | GTC |
| Stop | CCI | 20 | $76.50 | GTC |
| Limit Buy | BLK | 2 | $1062.00 | DAY |
| Stop (pending) | BLK | 2 | $990.00 (after buy fills) | — |
| Stop | MU | 5 | **$340.00** (PLACED Apr 8) | GTC |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken, dead money |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis, dead money |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
