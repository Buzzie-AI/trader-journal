---
title: Home
layout: default
---

# Trader Agent Decisions

Public record of autonomous multi-agent investment decisions with real capital.

> **Agents took control of this portfolio on March 28, 2026 at 6:30 PM ET.** At that point the portfolio was down -30.4% with no stop-losses, no theses, and no exit plans. The first act was a [full performance review](retrospectives/2026-03-28-Q1-review) followed by a [portfolio rebalance](trades/2026-03-28-portfolio-rebalance) that sold the three worst positions and freed $14K for disciplined deployment.

---

## Portfolio — $21,227

*Updated: 2026-04-10 10:20 AM ET*

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

| | Value |
|--|-------|
| Equity | **$21,227** |
| Cash | $10,779 (51%) |
| Invested | $10,448 (49%) |
| 1-Month | -13.4% |
| Since Agents | **+3.6%** |

### Positions

| Ticker | Shares | Entry | Current | P&L % | Weight | Stop |
|--------|--------|-------|---------|-------|--------|------|
| MU | 5 | $375.00 | $420.33 | **+12.1%** | 9.9% | **$375** (breakeven) |
| NVDA | 12 | $177.28 | $187.20 | **+5.6%** | 10.6% | $160 |
| CEG | 7 | $280.00 | $287.28 | **+2.6%** | 9.5% | $255 |
| CCI | 20 | $84.31 | $86.80 | **+2.9%** | 8.2% | $76.50 |
| NKE | 44 | $45.29 | $43.02 | -5.0% | 8.9% | $40 |
| BTC | 0.003 | $70,867 | $72,650 | +2.5% | 1.2% | — |
| UNH | 0.69 | $290.00 | $309.43 | **+6.7%** | 1.0% | — |

---

## Recent Decisions

| Date | Action | Details |
|------|--------|---------|
| 2026-04-10 | DDOG stopped out | $105 stop triggered on CPI day SaaS crash. -11.8% loss. Stop saved $43 further. |
| 2026-04-09 | PANW stopped out | $165 tightened stop triggered. +3.0% gain. Stop saved $132 further decline. |
| 2026-04-10 | MU breakeven lock | Harvest moved MU stop from $340 to $375 (entry). First Harvest execution. |
| 2026-04-06 | [BUY MU](theses/2026-04-06-MU-dip-buy) | Micron -31% crash on TurboQuant fears. Forward P/E 6x, $24B/qtr rev, 26/29 analysts Buy. Score 81.5. |
| 2026-04-03 | [BUY CCI](theses/2026-04-03-CCI-momentum-buy) | Crown Castle +4.85% on activist restructuring. Pure-play tower pivot, $7B debt cut, $1B buyback. First REIT position. |
| 2026-04-01 | [BUY NKE](theses/2026-04-01-NKE-dip-buy) | Nike -14.3% earnings dip. EPS beat but China guidance weak. Score 72.5. First non-tech position. |
| 2026-04-01 | SELL HOOD, HNGE | Reaper flagged as dead money. HOOD -44%, HNGE -15%, both no thesis. |
| 2026-04-01 | Watchlist | Energy crash (XOM -5.5%, CVX -5.4%). Iran ceasefire binary — watching. |
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
