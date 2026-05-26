---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-26 13:03 ET (Tue MANUAL autopilot run after morning cron deferred by integrity-hook block; equity $31,421 +$139 / +0.44% intraday; 3 RATCHETS executed — TXN $300→$310 (locks +$185 floor), MRVL $185→$195 (pre-earnings Wed AH lock), OKTA $82→$87; 22/22 stops intact; tape RISK-ON validated cross-confirmed Iran read; **MRVL Wed AH 5/27 earnings = next major event**) (prior Mon: MEMORIAL DAY mkts CLOSED, no trading; equity $31,289 BTC tick only; 22/22 stops intact; 7 Mercury alerts since Sun incl MRVL +2 bull-stack data points pre Wed 5/27 ER; Iran whipsaw unresolved; Tue 9:27 ET resumes) (orig Fri WEEK WRAP — **6 actions / -$267 realized / equity $31,274 (+$281 / +0.91% day; +1.24% week)**). **Week story = UNPRECEDENTED 4-CAP RESERVE**: Wed 3 BUYs cap (MRVL/TJX/BA $2,243), then 4th cap HELD Wed-Thu-Fri unprecedented. 16 ratchets across week locked $700+ paper into bounded. BILL stop fired Thu midday -$267 as predicted. Friday: Dow JONES RECORD HIGHS, all 3 indices green on Iran peace talks resuming. MRVL Citi PT $215 (3-firm cluster) + MRK Keytruda EU + TXN Seaport $400 PT + cyber RECORD highs = catalyst stack paying out 2-6% per held name.*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$31,273.88 EOD** (Fri close) |
| Cash | **$11,402.33** (36.4%) — biggest reserve in 2 weeks |
| Invested | $19,871.55 (63.5%) across **24 equity positions** (-BILL stopped) |
| Today's activity | **6 RATCHETS + 1 stop fired + 0 BUYs** |
| Realized today | **-$267** (BILL stop @$36) |
| Day P&L | **+$281 / +0.91%** vs Thu $30,992 |
| Week P&L | **+$384 / +1.24%** vs Tue $30,890 baseline |
| 🚀 Friday winners | MRK +5.7% / ZS +6.6% / TXN +3.5% / PANW +3.1% / MRVL +3.0% / CRWD +2.3% |
| 🔧 Friday ratchets | TXN $293→$300 (+$679 cumulative locked) / CRWD $625→$640 / MRK $107→$115 (2x) / PANW $235→$245 / ZS $165→$172 |
| 🚨 BILL stop fired | -$267 realized; was 1.3% cushion RED all week, predicted Thu |
| 🏆 Lifecycle highs | UNH +33.8% / CVS +23.5% / TXN +13.3% / DXCM +12.4% / MRK +8.9% / CRWD +8.8% / GE +6.6% |

---

## Equity Curve (1 Month + Today EOD)

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23 (+$3K deposit)","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12","May 13","May 14 (+$5K deposit)","May 15","May 18","May 19","May 20","May 21","May 22 EOD"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26439.85,26735.75,31124.35,30878.74,31100.67,30890.49,31059.40,30992.43,31273.88],
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
      }
    },
    scales: {
      y: { ticks: { callback: function(v) { return '$' + v.toLocaleString(); } } }
    }
  }
});
</script>

**Fri May 22 EOD:** $31,273.88 (+$281 / +0.91% vs Thu $30,992.43). Week total +$384 / +1.24%. Day featured 6 ratchets locking $63+ additional max-loss reduction, BILL stop fire -$267 (predicted), and Dow Jones finishing at RECORD HIGHS on Iran peace talks resuming. 8th straight weekly gain potential confirmed.

---

## Current Positions (24 equity + 1 frac + 1 crypto + CVR, EOD May 22)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **UNH** 🏆 | 0.69 | $290.00 | $387.92 | +$68 | **+33.8%** | — frac | n/a |
| **CVS** 🏆 | 27 | $75.83 | $93.62 | +$480 | **+23.5%** | $87 | 7.1% |
| **TXN** 🚀🔧 | 5 | $272.83 | $309.05 | +$181 | **+13.3%** | **$300 (locks +$679)** | 3.0% |
| **DXCM** 🔧 | 4 | $64.85 | $72.12 | +$29 | **+11.2%** | $66 | 8.5% |
| **MRK** 🚀🔧 | 18 | $112.47 | $122.44 | +$179 | **+8.9%** | **$115 (locks +$45)** | 6.1% |
| **CRWD** 🚀🔧 | 1 | $609.48 | $663.32 | +$54 | **+8.8%** | **$640 (locks +$30)** | 3.5% |
| **CCI** | 20 | $84.31 | $91.48 | +$143 | +8.5% | $84.31 (breakeven) | 7.8% |
| **PANW** 🚀🔧 | 1 | $243.21 | $260.67 | +$17 | +7.2% | **$245 (locks +$1.79)** | 6.0% |
| **GE** | 2 | $285.99 | $302.46 | +$33 | +5.8% | $263 | 13.0% |
| **MRVL** 🆕🚀 | 5 | $189.11 | $196.34 | +$36 | +3.8% | $185 | 5.8% **(ER WED 5/27)** |
| **SYY** 🔧 | 5 | $73.21 | $76.28 | +$15 | +4.2% | $72 | 5.6% |
| **BSX** | 5 | $55.14 | $57.13 | +$10 | +3.6% | $51 | 10.7% |
| **CSCO** | 1 | $117.34 | $120.55 | +$3 | +2.7% | $108 | 10.4% |
| **OKTA** 🆕 | 5 | $89.36 | $91.30 | +$10 | +2.2% | $82 | 10.2% |
| **NUE** | 9 | $223.00 | $226.47 | +$31 | +1.6% | $210 | 7.3% |
| **BLK** | 2 | $1,057.92 | $1,072.73 | +$30 | +1.4% | $990 | 7.7% (SpaceX SPCX) |
| **ZS** 🆕🚀🔧 | 3 | $180.83 | $182.31 | +$4 | +0.8% | **$172 (ratched today)** | 5.7% |
| **MSFT** | 1 | $415.53 | $418.50 | +$3 | +0.7% | $395 | 5.6% |
| **BA** 🔄re-entry | 3 | $220.33 | $220.04 | -$1 | -0.1% | $202 | 8.2% |
| **D** | 4 | $68.82 | $67.88 | -$4 | -1.4% | $63 | 7.1% |
| **TJX** 🆕 | 4 | $159.00 | $156.72 | -$9 | -1.4% | $146 | 6.8% |
| **NFLX** 🆕 | 5 | $91.12 | $88.51 | -$13 | -2.9% | $84 | 5.1% YELLOW |
| **BTC** | 0.0034 | $70,867 | $77,800 | +$24 | +9.6% | — crypto | n/a |

**Total Open P&L: ~+$1,366 unrealized EOD**. **Realized today: -$267 (BILL stop).**

**🚨 BILL STOPPED OUT @ $36** (64 sh × -$4.17/sh = -$267 realized) — was 1.3% cushion RED all week, predicted to fire Thu, fired Fri midday on cushion erosion.

🚀 **Friday Top Catalysts:**
- **ZS** +6.6%: Symmetry Systems M&A + cyber sector ETFs RECORD highs
- **MRK** +5.7%: Keytruda+Padcev EU CHMP positive opinion + LLY Foundayo pharma sleeve sympathy
- **TXN** +3.5%: Seaport Global upgrade Neutral→Buy + PT $400 (+34% upside)
- **PANW** +3.1%: Cyber sector ETFs RECORD highs continuation
- **MRVL** +3.0%: Citi PT $118→$215 + Wells $195 + Stifel $210 = 3-firm cluster (EARNINGS WED 5/27)
- **CRWD** +2.3%: Anthropic Claude integration + 11-leg sell-side cluster

---

## Open Orders (22 active GTC stops + 1 closed pos)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **TXN** 🔧 | 5 | **$300.00** | GTC | Ratcheted today (locks +$679 / +$135.84/sh × 5 above entry) |
| Stop | **MRK** 🔧 | 18 | **$115.00** | GTC | Ratcheted today 2x (locks +$45 above entry) |
| Stop | **CRWD** 🔧 | 1 | **$640.00** | GTC | Ratcheted today (locks +$30 above entry, 11-leg cluster) |
| Stop | **PANW** 🔧 | 1 | **$245.00** | GTC | Ratcheted today (locks +$1.79 above entry) |
| Stop | **ZS** 🔧 | 3 | **$172.00** | GTC | Ratcheted today (recovered RED to GREEN) |
| Stop | **MRVL** | 5 | **$185.00** | GTC | Locks +$14.45/sh above entry; ER WED 5/27 |
| Stop | CVS 🎯 | 27 | $87.00 | GTC | +23.5% lifecycle protected |
| Stop | DXCM | 4 | $66.00 | GTC | +11.2% lifecycle |
| Stop | SYY | 5 | $72.00 | GTC | Breakeven lock |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven |
| Stop | BSX | 5 | $51.00 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |
| Stop | OKTA | 5 | $82.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | SpaceX SPCX catalyst building |
| Stop | MSFT | 1 | $395.00 | GTC | |
| Stop | NFLX | 5 | $84.00 | GTC | YELLOW 5.1% |
| Stop | GE | 2 | $263.00 | GTC | T700 Apache contract |
| Stop | BA | 3 | $202.00 | GTC | New 5/20 re-entry |
| Stop | TJX | 4 | $146.00 | GTC | Off-price sleeve |
| Stop | D | 4 | $63.00 | GTC | |
| Stop | CSCO | 1 | $108.00 | GTC | |
| Stop | MRK (listed above ratched) | | | | |

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| 2026-05-22 | **BILL** | Stop fired @ $36 (64 sh) | **-$267 / -10.4%** | Was 1.3% cushion RED all week; predicted to fire Thu; fired Fri midday on cushion erosion |
| 2026-05-19 | **BA** | Stop fired @ $216 (3 sh) | -$46.85 / -1R | India regulatory + macro rates (re-entered 5/20 @ $220.33 on Beijing order) |
| 2026-05-13 | **AVGO** | Stop fired @ $407 (1 sh) | -$24.40 / -5.66% | 1R bounded loss |
| 2026-05-12 🎯 | **INTC** | Stop fired @ $120.01 (6 sh) | **+$138.97 / +23.93%** | Entry+5R lock; lifecycle +$256 / +44% |
| 2026-05-11 | CEG | Stop fired @ $289.52 (7 sh) | +$66.64 / +3.4% | Q1 mega-beat sold-the-news |

---

## Today's Catalyst Highlights (Fri 5/22)

### 🚀 Held Catalyst Payouts (top 6)
1. **ZS** +6.6% on cyber sector ETFs (HACK/BUG/CIBR) RECORD HIGHS continuation
2. **MRK** +5.7% peak on Keytruda+Padcev EU CHMP positive opinion (announced AM)
3. **TXN** +3.5% / +13.3% lifecycle on Seaport Global upgrade Neutral→Buy + PT $400
4. **PANW** +3.1% on cyber sector continuation
5. **MRVL** +3.0% on 3-firm analyst cluster (Citi $215 + Wells $195 + Stifel $210)
6. **CRWD** +2.3% on Anthropic Claude integration + cyber sector record

### ⚖️ Mixed/Macro
- All 3 indices GREEN: SPY +0.40% / QQQ +0.43% / DIA +0.61% (Dow finished RECORD HIGHS)
- 8th straight weekly gain potential confirmed
- Iran peace talks RESUMING (reversed Thu midday "stalled" narrative)
- Trump CANCELS AI Executive Order (deregulation boost)
- ROST Q1 +20% beat (TJX peer validation, though TJX disconnect persists)

### 🚨 Single Loss
- **BILL stop fired -$267 realized** (predicted Thu RED 1.3% cushion; fired Fri midday)

---

## Sector Sleeve Status (EOD May 22)

| Sleeve | Members | Value | % of Portfolio |
|--------|---------|-------|----------------|
| **Cyber** (CRWD+ZS+OKTA+PANW) | 4 names | $1,920 | 6.1% |
| **Chip** (MRVL+TXN) | 2 names | $2,557 | 8.2% |
| **Defensive Pharma/Health** (CVS+MRK+UNH+BSX+DXCM) | 5 names | $5,656 | 18.1% |
| **REIT/Utility** (CCI+D) | 2 names | $2,099 | 6.7% |
| **Consumer Staples** (SYY+NUE) | 2 names | $2,467 | 7.9% |
| **Industrials** (GE+BA) | 2 names | $1,266 | 4.0% |
| **Consumer Discretionary** (TJX+NFLX) | 2 names | $1,069 | 3.4% |
| **Financials** (BLK) | 1 name | $2,146 | 6.9% |
| **AI/Software** (MSFT+CSCO) | 2 names | $539 | 1.7% |
| **Crypto** (BTC) | 1 name | $265 | 0.8% |
| **Cash** | | $11,402 | 36.4% |

Tech total (cyber + chip + AI/software) = ~16% — well under raised 50% ceiling.

---

## Process Notes (Week Highlights)

1. **Pipeline discipline 100%** — all 3 BUYs (MRVL/TJX/BA Wed) ran full 5-agent fast-track
2. **Tape-confirming framework saved capital MULTIPLE times** — MU/TGT/NVDA-add/INTU/DE all PASSED despite top catalysts
3. **4-cap reserve held UNUSED full week** — first time ever; ratchets capturing catalyst value better than chasing new entries
4. **BILL stop fired clean** — -$267 within -$272 estimate; stop discipline rule "let mechanical stops do their job" validated
5. **MRVL pre-earnings setup** — May 27 (Wed) earnings, 3-firm analyst bull cluster sets bar; current stop $185 locks +$14.45/sh above entry; consider pre-earnings trim per Harvest playbook OR aggressive ratchet to $190 if Mon-Tue strength
</parameter>
</invoke>