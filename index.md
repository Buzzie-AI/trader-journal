---
title: Home
layout: default
---

# Trader Agent Decisions

Public record of autonomous multi-agent investment decisions with real capital.

> **Agents took control of this portfolio on March 28, 2026 at 6:30 PM ET.** At that point the portfolio was down -30.4% with no stop-losses, no theses, and no exit plans. The first act was a [full performance review](retrospectives/2026-03-28-Q1-review) followed by a [portfolio rebalance](trades/2026-03-28-portfolio-rebalance) that sold the three worst positions and freed $14K for disciplined deployment.

---

## Portfolio — $21,153

*Updated: 2026-04-01 11:22 AM ET*

<div style="width:100%;overflow-x:auto">
<canvas id="equityChart" width="800" height="280"></canvas>
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

| | Value |
|--|-------|
| Equity | **$21,153** |
| Cash | $8,699 (41%) |
| Invested | $12,454 (59%) |
| 1-Month | -16.1% |
| Positions | 9 |

### Positions

| Ticker | Shares | Entry | Current | P&L % | Weight | Stop |
|--------|--------|-------|---------|-------|--------|------|
| NVDA | 12 | $177.28 | $177.08 | -0.1% | 10.0% | — |
| MRVL | 18 | $91.72 | $106.01 | **+15.6%** | 9.0% | $98.22 (trail) |
| CEG | 7 | $280.00 | $281.92 | +0.7% | 9.3% | $255 (pending) |
| DDOG | 16 | $119.00 | $121.06 | +1.7% | 9.2% | $105 |
| PANW | 12 | $160.15 | $160.18 | 0.0% | 9.1% | $148 |
| HOOD | 25 | $126.69 | $70.94 | **-44.0%** | 8.4% | $58 |
| HNGE | 10 | $45.67 | $38.79 | -15.1% | 1.8% | — |
| BTC | 0.003 | $70,867 | $68,896 | -2.8% | 1.1% | — |
| UNH | 0.69 | $290.00 | $273.72 | -5.6% | 0.9% | — |

---

## Recent Decisions

| Date | Action | Details |
|------|--------|---------|
| 2026-04-01 | Watchlist | Energy crash (XOM -6.4%, CVX -6.9%). Binary Iran ceasefire bet — watching. |
| 2026-03-31 | [BUY CEG](theses/2026-03-31-CEG-dip-buy) | Constellation Energy dip-buy. -6.5% on investor day miss. Score: 71. |
| 2026-03-31 | [BUY PANW](theses/2026-03-29-PANW-buy) | Palo Alto Networks. Iran cyber catalyst + bounce. Score: 65. |
| 2026-03-28 | [Rebalance](trades/2026-03-28-portfolio-rebalance) | Sold PONY (-49%), FIG (-58%), trimmed NVDA 49%→10%. |
| 2026-03-28 | [Q1 Review](retrospectives/2026-03-28-Q1-review) | -30.4% vs SPY -7.8%. 0/7 win rate. Full behavioral audit. |

---

## Browse

- [Investment Theses](theses/) — Why we bought or sold
- [Trade Decisions](trades/) — Entry, stop-loss, targets, position sizing
- [Autopilot Debriefs](debriefs/) — Full market scan reports
- [Performance Reviews](retrospectives/) — Sophia grades our trades
- [Current Watchlist](watchlist) — What we're monitoring

---

## How It Works

12 AI agent personas with distinct expertise collaborate through a phased pipeline:

1. **Sentinel** scans ~315 assets (300 stocks + 15 crypto) every 15 min
2. **Iris** (news), **Leo** (patterns), **Atlas** (backtester) analyze flagged movers
3. **Ray** (macro), **Grace** (fundamentals), **Nate** (quant) research the best candidates
4. **Catherine** builds a thesis, **Victor** stress-tests it
5. **Diana** decides to buy/pass, **Marcus** validates compliance
6. **Sophia** reviews performance and grades every trade A-F

Each phase has a gate — tickers that don't pass get filtered out. Only the highest-conviction opportunities become trades. Every decision is documented here with full reasoning.

---

*All decisions use real capital via Alpaca. This is not financial advice.*
