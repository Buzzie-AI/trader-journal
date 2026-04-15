---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-14 8:57 PM ET (End of Day)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,583** |
| Cash | $8,663 (40.1%) |
| Invested | $12,920 (59.9%) |
| Positions | 6 stocks + BTC + UNH (all stops active ✅) |

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
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21583],
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
| 1 Month | $24,891 | $21,583 | **-13.3%** |
| Since Agents (Mar 28) | $20,489 | $21,583 | **+5.3%** |
| Low | $20,408 (Mar 31) | | |
| High | $24,891 (Mar 3) | | |

---

## Current Positions

| Ticker | Shares | Entry | Close | P&L | P&L % | Weight | Stop |
|--------|--------|-------|-------|-----|-------|--------|------|
| MU | 5 | $375.00 | $460.48 | +$427.40 | **+22.8%** | 10.7% | **$438** (Harvest 2x) |
| NVDA | 12 | $177.28 | $195.83 | +$222.57 | **+10.5%** | 10.9% | **$185** (Harvest 2x) |
| CEG | 7 | $280.00 | $297.19 | +$120.33 | **+6.1%** | 9.6% | $255 |
| BLK | 2 | $1057.92 | $1049.21 | -$17.42 | -0.8% | 9.7% | **$990 ✅ (placed EOD)** |
| NKE | 44 | $45.29 | $45.20 | -$3.82 | -0.2% | 9.2% | $40 |
| CCI | 20 | $84.31 | $81.28 | -$60.60 | **-3.6%** ⚠️ | 7.5% | $76.50 |
| BTC | 0.003 | $70,867 | $74,508 | +$12.56 | **+5.1%** | 1.2% | — |
| UNH | 0.69 | $290.00 | $314.70 | +$17.03 | **+8.5%** | 1.0% | — |

**Open P&L: +$718** | Day: +$255 (MU +$170, NKE +$101 recovery, CCI -$116 drop). First time this quarter all positions have active stops.

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
| Tech (NVDA, MU) | $4,652 | 21.6% |
| Financials (BLK) | $2,098 | 9.7% |
| Energy/Nuclear (CEG) | $2,080 | 9.6% |
| Consumer (NKE) | $1,989 | 9.2% |
| Real Estate (CCI) | $1,626 | 7.5% ⚠️ |
| Crypto (BTC) | $257 | 1.2% |
| Healthcare (UNH) | $217 | 1.0% |
| **Cash** | **$8,663** | **40.1%** |

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF |
|------|--------|-----|---------|-----|
| Stop | MU | 5 | **$438** (Harvest 2x: $400→$420→$438) | GTC |
| Stop | NVDA | 12 | **$185** (Harvest 2x: $160→$178→$185) | GTC |
| Stop | NKE | 44 | $40.00 | GTC |
| Stop | CEG | 7 | $255.00 | GTC |
| Stop | CCI | 20 | $76.50 | GTC |
| **Stop** | **BLK** | **2** | **$990.00 (placed EOD ✅)** | GTC |
| Stop | MU | 5 | **$340.00** (PLACED Apr 8) | GTC |

---

## Recently Closed

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| HOOD | $126.69 | ~$70.44 | -44.4% | Reaper: thesis broken, dead money |
| HNGE | $45.67 | ~$38.83 | -15.0% | Reaper: no thesis, dead money |
| PONY | $18.05 | $9.15 | -49.4% | Q1 rebalance |
| FIG | $48.18 | $20.21 | -58.1% | Q1 rebalance |
