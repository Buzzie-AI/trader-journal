---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-07 9:57 AM ET (Thursday — manual /autopilot fire; CVX stopped out at open, 0 new buys, 6 tickers watchlisted)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$25,963.05** |
| Cash | $4,605.71 (17.7%) — overweight post-CVX exit |
| Invested | $21,357.34 (82.3%) |
| Positions | 12 equity + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **1 action: CVX stop fired 09:30 ET** — 10 sh sold @ $181.50 / realized **-$104.20** on XLE -2.13% sector weakness. Autonomous stop @ $182 GTC executed cleanly. Manual /autopilot at 09:50 evaluated 8 Mercury-flagged tickers (C/MCD/UBER/LLY/ON/AMD/DDOG/NVDA), 0 new buys (Citi investor-day ROTCE disappointed; others either chased or no edge). |
| Stop coverage | ✅ 11 active stops on 11 stoppable equity positions. Exempt: UNH (fractional), 737CVR019 (CVR), BTC. |
| 🎯 Best held | **MU +21.1%** (3 sh post-trim, stop $634) · **INTC +14.8%** (target $115 = 3.4% away) · **CEG +15.0%** · **CVS +14.9%** · **UNH +27.0%** (frac) · **BTC +13.4%** ($80,346) |
| Day P&L | **-$204.35 / -0.78%** vs Wed last $26,167.40 |
| **Realized today** | **-$104.20** (CVX stop fire) |

---

## Equity Curve (1 Month + Today)

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25251.27,25699.52,26182.80,25963.05],
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
          sleeveLine: {
            type: 'line',
            xMin: 'Apr 23',
            xMax: 'Apr 23',
            borderColor: '#3b82f6',
            borderWidth: 2,
            borderDash: [4, 4]
          },
          depositMarker: {
            type: 'point',
            xValue: 'Apr 23',
            yValue: 24602.55,
            backgroundColor: '#a855f7',
            radius: 7,
            borderColor: '#fff',
            borderWidth: 2
          },
          depositLabel: {
            type: 'label',
            xValue: 'Apr 23',
            yValue: 24602.55,
            yAdjust: -20,
            content: ['+$3K deposit'],
            color: '#a855f7',
            font: { size: 11, weight: 'bold' },
            backgroundColor: 'rgba(255,255,255,0.85)',
            padding: 3
          }
        }
      }
    },
    scales: {
      y: {
        ticks: { callback: function(v) { return '$' + (v/1000).toFixed(1) + 'k'; } },
        min: 19000, max: 27000
      }
    }
  }
});
</script>

| Period | Start | End | Change | Notes |
|--------|-------|-----|--------|-------|
| **Today (May 7, intraday)** | $26,167.40 (Wed last) | $25,963.05 | **-0.78% (-$204)** | CVX stop fired 09:30 ET (-$104 realized); semi cohort MRVL/TXN soft on broader semi rotation; 0 new buys after pipeline-discipline PASS on Citi (ROTCE disappointment) |
| 1 Week | $25,251.27 (Apr 30) | $25,963.05 | **+2.8% (+$712)** | INTC sleeve buy +14.8%; MU 3R harvest cycle; CVS Q1 catalyst stack; CVX stopped out today |
| **Since Agents (Mar 28)** | $20,489 | $25,963.05 | **+$5,474 (+26.7%)** | Excludes $3,000 Apr 23 deposit; agent P&L only ≈ +$2,474 (+12.1%) |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$2,694 (+13.1% in 39 days)**. The total-equity chart includes a $3,000 deposit on Apr 23 (purple dot).

---

## Current Positions (12 equity + 1 frac + 1 crypto, intraday May 7)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** | 3 | $541.11 | $655.46 | +$343 | **+21.1%** 🎯 | $634 | -3.4% TIGHT |
| **CEG** | 7 | $280.00 | $322.42 | +$297 | **+15.0%** | $290 | -10.1% |
| **CVS** | 27 | $75.83 | $87.13 | +$305 | **+14.9%** 🎯 | $82 | -5.9% |
| **INTC** | 12 | $96.85 | $111.21 | +$172 | **+14.8%** 🎯 | $100 | -10.1% |
| **CCI** | 20 | $84.31 | $91.05 | +$135 | +8.0% | $84.31 | -7.4% |
| **TXN** | 5 | $272.83 | $283.56 | +$54 | +3.9% | $252.58 | -10.9% |
| **MRVL** | 9 | $159.54 | $165.33 | +$52 | +3.6% | $145 | -12.3% |
| **NUE** | 9 | $223.00 | $230.66 | +$69 | +3.4% | $210 | -8.9% |
| **BLK** | 2 | $1,057.92 | $1,071.18 | +$27 | +1.3% | $990 | -7.6% |
| **MRK** | 18 | $112.47 | $112.45 | -$0 | -0.0% | $103.50 | -8.0% |
| **NKE** | 44 | $45.29 | $44.28 | -$44 | -2.2% | $42.50 | -4.0% |
| **UNH** | 0.69 | $290.00 | $368.17 | +$54 | **+27.0%** | — frac | n/a |
| **BTC** | 0.0034 | $70,867 | $80,346 | +$33 | **+13.4%** | — crypto | n/a |
| 737CVR019 | 4.06 | $0 | (CVR) | — | — | — | — |

**Total open unrealized P&L: +$1,497.** **Realized today: -$104.20** (CVX stop fire).

⚠️ **Tight-stop watch:**
- **MU** -3.4% buffer post-3R-trim — ratchet design, acceptable for runner.
- **NKE** -4.0% buffer (improved from yesterday's -2.9%); position recovering toward breakeven.

🎯 **Trim trigger watch:** **INTC** target $115 = 3.4% away. If breached → 50% trim per Harvest Rule 2.

🚪 **Closed today:**
- **CVX** stop $182 GTC fired @ open print 09:30 ET, 10 sh @ $181.50 = **-$104.20 realized** on XLE -2.13% sector drag. Autonomous stop did its job.

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,491 (25%) | $6,206 (23.9%) | **WITHIN TARGET — 95.6% fill** | MRVL, TXN, MU (3 sh), INTC |

Sleeve dry powder: $285 (effectively none for new buys). Regime: HOT (recent Mercury alert cluster on semis). No actionable sleeve adds this run; revisit if a sleeve member dips meaningfully or sleeve consolidates back below 90%.

---

## Allocation (intraday May 7)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MRVL, TXN, MU, INTC) | $6,206 | 23.9% (within target) |
| Healthcare (MRK, CVS, UNH) | $4,630 | 17.8% |
| Utility/Nuclear (CEG) | $2,257 | 8.7% |
| Financials (BLK) | $2,142 | 8.3% |
| Materials (NUE) | $2,076 | 8.0% |
| Consumer (NKE) | $1,948 | 7.5% |
| Real Estate (CCI) | $1,821 | 7.0% |
| Energy | **$0** | **0.0%** (CVX stopped out today; sector ZERO-WEIGHT) |
| Crypto (BTC) | $277 | 1.1% |
| **Cash** | **$4,606** | **17.7%** — overweight post-CVX exit |

---

## Open Orders (11 active stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | MU | 3 | $634.00 | GTC | Post-3R-advance (5/6); buffer -3.4% TIGHT |
| Stop | CVS | 27 | $82.00 | GTC | Advanced 5/6 from $75.83 BE-lock on triple-bull |
| Stop | INTC | 12 | $100.00 | GTC | Placed 5/6 backfill |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | Buffer -4.0% (improved from yesterday's -2.9%) |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |

🚪 **Filled today:** CVX 10 sh @ $181.50 (stop $182 GTC fire 09:30 ET) — order `a53e6278`. Realized **-$104.20**.

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-07** | **CVX** | Stop fired @ $181.50 (10 sh) | **-$104.20 / -5.4%** | Entry 4/30 @ $191.92. Stop $182 GTC fired at 09:30 ET open print on XLE -2.13% sector drag. Energy sector now zero-weight. |
| 2026-05-06 | MU | 3R trim 1 sh @ $653.32 | +$112.21 / +20.7% | Entry 5/1 @ $541.11. Position 4 → 3 sh. Stop advanced to $634. |
| 2026-05-04 | NVDA | Stop fired @ $194.885 (10 sh) | +$179.55 / +10.1% | Entry 3/9 @ $176.93 |
| 2026-04-28 | INTC | Stop fired @ $81.50 (gap-down) | +$204 | Q1 blowout +29× then sleeve compression |
| 2026-04-28 | LRCX | Stop fired @ $245.94 | -$86 | US Commerce Hua Hong tool-ban |
| 2026-04-28 | BA | Stop fired @ $227.87 | +$44 | Airbus Q1 mixed peer-cohort |

---

## Today's Mercury alert highlights (40 alerts, May 7 09:40 drain)

- **DDOG TRIPLE-BULL** — Q1 EPS $0.60 vs $0.51 (+17.6%) + Q2 guide above + FY26 raise (best single-name catalyst stack of drain) — tape +29.5% intraday, CHASED
- **TPR DOUBLE-PRINT** — Q3 EPS $1.66 vs $1.30 (+27.7%) + FY26 guide raise to $6.95 vs $6.51 — but tape -9.2% (sell-the-news / dip-buy candidate tomorrow)
- **C INVESTOR DAY** — $30B BUYBACK + ROTCE 11-13% (2027-28) / 14-15% (2029-31) — but headlines confirm market disappointed in pace; tape -0.2%
- **MCD** — Q1 EPS $2.83 vs $2.74 + global comp +3.8% / system +11% (under-reacted, tape +0.4%)
- **FTNT TRIPLE** — Q1 BEAT + Q2 guide above + FY26 raise; tape +22.9% (chased)
- **U** — Q1 EPS $0.23 vs $(0.23) **swing-to-profit**; tape +8.6%
- **ZTS DOUBLE-BEAR** — Q1 miss + FY26 guide CUT; tape -21% (clean bear)
- **ON** — $1.3B 0% conv at 52.5% premium (sleeve member; tape -2.6% on dilution worry)
- **AMD/RXT** — sovereign-cloud MOU (regulated/financial/defense TAM)
- **NVDA** — SpaceX + Anthropic both committing to GB300
- **AAPL/AMZN/GOOGL/MSFT BEAR** — EU cloud-sovereignty restriction multi-name
- **LLY** — $4.5B Indiana capex (GLP-1 supply); tape -1.3%

### Yesterday's Mercury highlights (May 6 EOD ~50 alerts)

- **AMD analyst-upgrade cluster** — 9 shops same day, PT range $430-$525 (Goldman/Stifel/Seaport/Bernstein/Truist/Rosenblatt/Benchmark/Barclays/TD Cowen)
- **Earnings/M&A wave** — 10 deals ~$77B+ aggregate cross-sector (Sysco-Restaurant Depot $29B, Shell-Canadian $14B, Organon-Sun Pharma $13B, KDP-coffee $18B closed, Bayer-Perfuse $2.45B, AMETEK $5B, Lattice-AMI $1.65B, WES-Delaware $1.6B, Sony-Music $4B, Compass-Anywhere)
- **Held cohort positives:** CVS triple-bull-stack (Q1 BEAT + Adj guide raise + GAAP guide raise) — actioned via stop advance; INTC mgmt hire + 52w high; BLK Preqin private credit + DTCC tokenized equities; MRK Salesforce Animal Health platform
- **AI infrastructure:** NVDA 3 partnership wins (GLW $500M optical interconnect + warrant, TTE Pangea 5 supercomputer, SLP drug-dev simulation) + OpenAI Multipath protocol + xAI Colossus 220K-GPU sharing with Anthropic; offsetting bear: Rubin GPU production-delay rumor, SpaceX/Musk $119B "Terafab" rumor, China DeepSeek; **TSM $56B AI expansion concrete counter**
- **BTC-miner-to-AI pivot cohort:** HUT $9.8B AI lease, IREN $625M Mirantis, NBIS Eigen AI + META partnership; CORZ Q1 wider loss as cohort dispersion
- **FTNT quintuple-positive Q1 cycle** (post-close): print +32% EPS BEAT + Q2 EPS guide + Q2 sales guide + FY26 EPS raise + FY26 sales raise — likely Phase 0.5 fast-track candidate tomorrow
- **DIS quadruple-positive Q2:** print BEAT + $8B FY26 buyback + FY26 12-16% EPS guide + FY27 double-digit affirm
- **NVO triple-stack:** Q1 +36.3% MASSIVE sales beat + FY26 guide raise + China generic Ozempic delay (competitive moat)
- **Pharma policy bear stack** (3 alerts): RFK Jr. deprescribing + Trump $529B drug-pricing claim + Sanofi Teplizumab/FDA voucher political-interference
- **Payments cohort mixed/bear:** MA/V/PYPL UK FCA antitrust + MS undercutting COIN/HOOD on E*Trade crypto fees + GPN tape-down + FISV revenue miss
- **Energy weakness:** US-Iran de-escalation + alleged $920M oil-short trade pattern → CVX/XOM/DVN tape down

---

## Today's autopilot watchlist additions (May 7 manual fire)

| Score | Ticker | Catalyst | Action | Re-eval Trigger |
|------:|--------|----------|--------|-----------------|
| 85.5 | **C** | $30B buyback + investor-day ROTCE roadmap | **WATCH** | Pull below $120 OR ROTCE acceleration in Q2 |
| 82.5 | **MCD** | Q1 beat + comp accel | **WATCH** | Pullback to $280 zone |
| 79.5 | **LLY** | $4.5B Indiana capex | **WATCH** | Dip below $950 |
| 77.8 | **UBER** | Ulta partnership + DASH cohort | **WATCH** | Q1 print or 5%+ pullback |
| 70.8 | **ON** | $1.3B 0% conv (sleeve member) | **WATCH** | Sleeve room opens OR sub-$100 |
| (bear) | **TPR** | Q3 +27.7% beat + FY26 raise but **tape -9.2%** | **WATCH (DIP-BUY candidate)** | Tape stabilizes tomorrow + quality intact |
| (bear) | **ZTS** | Q1 miss + FY26 cut, tape -21% | **AVOID** | Genuine fundamental miss; not a dip-buy |

### Yesterday's deferred watchlist (still active)

| Score est | Ticker | Catalyst | Notes |
|-----------|--------|----------|-------|
| 92 | **FTNT** | Quintuple-positive Q1 cycle | Already +22.9% today (chased — fade risk) |
| 88 | **OGN** | $13B Sun Pharma takeover | Takeover-arb shape, small position |
| 88 | **NBIS** | Eigen AI + META partnership | AI-infra mid-cap |
| 85 | **DIS** | Q2 quadruple-positive | Media mega-cap |
| 80 | **NVO** | Q1 +36% sales beat | Pharma |
| 78 | **SHOP** | Q1 +34% YoY revenue + analyst PT raise | E-commerce/SaaS |
| 75 | **MRNA** | Phase 3 mRNA-1010 NEJM publication | Counter-narrative to vaccine policy bears |
| 75 | **TEM** | Q1 +36.1% revenue beat + FY26 raise | AI-diagnostics |

---

*Auto-generated by manual /autopilot fire; published to Buzzie-AI/trader-journal at 2026-05-07 09:58 ET.*
