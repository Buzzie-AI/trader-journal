---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-20 09:53 AM ET (Monday open, intraday)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$21,755** |
| Cash | $4,482 (20.6%) |
| Invested | $17,273 (79.4%) |
| Positions | 8 stocks + BTC + UNH fractional |
| Today's Day P&L | **-$118 (-0.54%)** |
| Stop coverage | ✅ **All 8 whole-share equity positions stop-protected** |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21754.74],
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
| 1 Month | $23,448 | $21,755 | **-7.2%** |
| Since Agents (Mar 28) | $20,489 | $21,755 | **+6.2%** |
| Low | $20,408 (Mar 31) | | |
| High | $23,448 (Mar 17) | | |

---

## Current Positions (Intraday)

| Ticker | Shares | Entry | Last | P&L | P&L % | Today | Weight | Stop |
|--------|--------|-------|------|-----|-------|-------|--------|------|
| MU | 5 | $375.00 | $451.93 | +$384.63 | **+20.5%** | -0.69% | 10.4% | **$438** (Harvest 2x) |
| NVDA | 12 | $177.28 | $199.46 | +$266.07 | **+12.5%** | -1.10% | 11.0% | **$185** (Harvest 2x) |
| NFLX | 22 | $97.00 | $95.88 | -$24.71 | **-1.2%** | -1.47% | 9.7% | $93.50 ⚠️ tight (-2.5%) |
| BLK | 2 | $1057.92 | $1,056.16 | -$3.52 | -0.17% | +0.38% | 9.7% | $990 ✅ |
| CEG | 7 | $280.00 | $293.19 | +$92.33 | **+4.7%** | -1.02% | 9.4% | $255 (pre-earn Apr 28 trim) |
| CVS | 27 | $75.83 | $76.86 | +$27.85 | **+1.4%** | -0.57% | 9.5% | $72.75 ⚠️ earnings date TBD |
| NKE | 44 | $45.29 | $45.81 | +$22.80 | **+1.1%** | -0.49% | 9.3% | $42.50 ✅ |
| CCI | 20 | $84.31 | $88.68 | +$87.40 | **+5.2%** | -0.03% | 8.2% | $80 (tightened from $76.50) |
| BTC | 0.003 | $70,867 | $75,208 | +$14.98 | **+6.1%** | +0.72% | 1.2% | — |
| UNH | 0.69 | $290.00 | $323.22 | +$22.91 | **+11.5%** | -0.43% | 1.0% | — |

**Open P&L: +$891** | Morning session, broader market slightly red (SPY -0.2%, QQQ -0.3%). Energy (XLE +1%) leads on Iran ceasefire expiry tomorrow.

---

## Allocation

| Category | Value | Weight | Note |
|----------|-------|--------|------|
| Tech (NVDA, MU) | $4,653 | 21.4% | |
| **Communication (NFLX)** | **$2,109** | **9.7%** | Stop tight; watching |
| Healthcare (CVS + UNH) | $2,298 | 10.6% | CVS earnings date unverified |
| Financials (BLK) | $2,112 | 9.7% | |
| Utility/Nuclear (CEG) | $2,052 | 9.4% | Pre-earnings Apr 28 trim fires |
| Consumer (NKE) | $2,015 | 9.3% | |
| Real Estate (CCI) | $1,774 | 8.2% | FOMC Apr 28 rate-sensitive |
| Crypto (BTC) | $259 | 1.2% | |
| **Cash** | **$4,482** | **20.6%** | Room to deploy; Sage prefers non-tech |

Eight sectors. Tech concentration (incl. comm) at 31.1% — Sage flag.

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | MU | 5 | $438.00 | GTC | Harvest 2x advance |
| Stop | NVDA | 12 | $185.00 | GTC | Harvest 2x advance |
| Stop | BLK | 2 | $990.00 | GTC | Placed Apr 14 |
| Stop | CEG | 7 | $255.00 | GTC | |
| Stop | CVS | 27 | $72.75 | GTC | Placed Apr 16 |
| Stop | NKE | 44 | $42.50 | GTC | Tightened |
| Stop | CCI | 20 | $80.00 | GTC | Tightened from $76.50 |
| Stop | NFLX | 22 | $93.50 | GTC | Placed Apr 18 |

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

---

## This Week's Catalysts (from Oracle)

| Date | Event | Relevance |
|------|-------|-----------|
| **Apr 21 (AMC)** | ISRG Q1 earnings | Watchlist candidate post-earnings |
| **Apr 21-22** | 🚨 Iran ceasefire EXPIRES — binary | No energy exposure. XLE hedge considered |
| **Apr 22 (AMC)** | TSLA + GEV earnings | No position |
| **Apr 28** | FOMC + MSFT earnings start | CCI rate-sensitive; CEG pre-earn trim fires |
| **~Apr 30** | CVS earnings (date unverified) | Pre-earn trim would fire Apr 23 if confirmed |
| **May 5** | CEG earnings | Pre-earn trim fires Apr 28 |

*Oracle calendar last rebuilt Apr 16; refresh due.*
