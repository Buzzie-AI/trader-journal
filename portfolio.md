---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-06 6:36 PM ET (Wednesday post-close — eod_summary refresh after autopilot_close at 16:23 ET)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$26,182.80** |
| Cash | $2,790.76 (10.7%) ✅ above $2K min-reserve |
| Invested | $23,392.04 (89.3%) |
| Positions | 13 equity + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **4 actions**: (1) **MU 3R trim 09:59 ET** — sold 1 sh @ $653.32 / realized +$112.21; (2) MU stop $510 → $603 (entry+2R); (3) CVS stop $75.83 → $82 on triple-bull-stack (Q1 BEAT + Adj guide raise + GAAP guide raise); (4) **MU 4R stop advance 16:24 ET** — $603 → $634 (entry+3R). |
| Stop coverage | ✅ 13 active stops. Exempt: UNH (fractional), 737CVR019 (CVR), BTC. |
| 🎯 Best held | **MU +23.9%** (3 sh post-trim) · **INTC +17.4%** (52w high, target $115 within 1.1%) · **CEG +15.3%** · **CVS +14.5%** (Q1 triple-bull) · **UNH +26.3%** (frac) · **BTC +15.2%** ($81,614) |
| Day P&L | **+$483.27 / +1.88%** vs Tues close $25,699.52 |
| **Realized today** | **+$112.21** (MU 3R trim) |

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25251.27,25699.52,26182.80],
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
| **Today (May 6)** | $25,699.52 (Tues close) | $26,182.80 | **+1.88% (+$483)** | MU 3R trim +$112 realized; MU stop advanced 2× ($510→$603→$634); CVS stop advance on triple-bull-stack |
| 1 Week | $25,093.43 (Apr 30) | $26,182.80 | **+4.3% (+$1,089)** | INTC sleeve buy 5/4 fired well (+17.4%); MU 3R harvest cycle; CVS Q1 catalyst stack |
| **Since Agents (Mar 28)** | $20,489 | $26,182.80 | **+$5,694 (+27.8%)** | Excludes $3,000 Apr 23 deposit; agent P&L only ≈ +$2,694 (+13.1%) |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$2,694 (+13.1% in 39 days)**. The total-equity chart includes a $3,000 deposit on Apr 23 (purple dot).

---

## Current Positions (13 equity + 1 frac + 1 crypto, EOD May 6)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** | 3 | $541.11 | $670.69 | **+$389** | **+23.9%** 🎯 | $634 (NEW today) | -5.5% |
| **INTC** | 12 | $96.85 | $113.74 | +$203 | **+17.4%** 🎯 | $100 | -12.1% |
| **CEG** | 7 | $280.00 | $322.95 | +$301 | **+15.3%** | $290 | -10.2% |
| **CVS** 🆕 | 27 | $75.83 | $86.86 | +$298 | **+14.5%** 🎯 | $82 (NEW today) | -5.6% |
| **MRVL** | 9 | $159.54 | $172.50 | +$117 | +8.1% | $145 | -16.0% |
| **CCI** | 20 | $84.31 | $90.24 | +$119 | +7.0% | $84.31 | -6.6% |
| **TXN** | 5 | $272.83 | $289.44 | +$83 | +6.1% | $252.58 | -12.7% |
| **NUE** | 9 | $223.00 | $233.68 | +$96 | +4.8% | $210 | -10.1% |
| **BLK** | 2 | $1,057.92 | $1,073.57 | +$31 | +1.5% | $990 | -7.8% |
| **MRK** | 18 | $112.47 | $113.56 | +$20 | +1.0% | $103.50 | -8.9% |
| **NKE** | 44 | $45.29 | $43.76 | -$67 | -3.4% | $42.50 | -2.9% ⚠️ |
| **CVX** | 10 | $191.92 | $185.08 | -$68 | -3.6% | $182 | -1.66% ⚠️ TIGHT |
| **UNH** | 0.69 | $290.00 | $366.35 | +$53 | **+26.3%** | — frac | n/a |
| **BTC** | 0.0034 | $70,867 | $81,614 | +$37 | **+15.2%** | — crypto | n/a |
| 737CVR019 | 4.06 | $0 | (CVR) | — | — | — | — |

**Total open unrealized P&L: +$1,712.** **Realized today: +$112.21** (MU trim).

⚠️ **Tight-stop watch into Thursday open:**
- **CVX** -1.66% buffer; -3.92% intraday on US-Iran/Hormuz oil weakness. If oil weakness extends overnight → accept stop trigger.
- **NKE** -2.9% buffer; position recovering slowly (-3.4% on cost still). Worth widening if uptrend confirms.

🎯 **Trim trigger watch:** **INTC** thesis target $115 within 1.1% at close. If breached at open → 50% trim per Harvest Rule 2.

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,546 (25%) | $6,377 (24.4%) | **WITHIN TARGET** (post-MU trim) | MRVL, TXN, MU (3 sh), INTC |

Semi sleeve fell from 26.6% (over) to 24.4% (within) after MU 3R trim. Room for ~1 small add (FTNT/AMD/etc.) tomorrow if Phase 0.5 pipeline confirms.

---

## Allocation (EOD May 6)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MRVL, TXN, MU, INTC) | $6,377 | 24.4% (within target) |
| Healthcare (MRK, CVS, UNH) | $4,642 | 17.7% |
| Utility/Nuclear (CEG) | $2,261 | 8.6% |
| Financials (BLK) | $2,147 | 8.2% |
| Materials (NUE) | $2,103 | 8.0% |
| Real Estate (CCI) | $1,805 | 6.9% |
| Energy (CVX) | $1,851 | 7.1% (weakest today on Iran de-escalation) |
| Consumer (NKE) | $1,925 | 7.4% |
| Crypto (BTC) | $282 | 1.1% |
| **Cash** | **$2,791** | **10.7%** ✅ |

---

## Open Orders (13 active stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** 🆕 | 3 | **$634.00** | GTC | **NEW today (entry+3R, 4R milestone advance)** |
| Stop | **CVS** 🆕 | 27 | **$82.00** | GTC | **NEW today (advanced from $75.83 breakeven on triple-bull stack)** |
| Stop | INTC | 12 | $100.00 | GTC | T+1 placed 5/5 |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | TIGHT buffer (-2.9%) |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | CVX | 10 | $182.00 | GTC | TIGHT buffer (-1.66%) |
| Stop | NUE | 9 | $210.00 | GTC | |

🚪 **Filled today:** MU 1 sh @ $653.32 (3R trim) — order `3708aa1a`. Realized +$112.21.

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-06** | **MU** | 3R trim 1 sh @ $653.32 | **+$112.21 / +20.7%** | Entry 5/1 @ $541.11. Position 4 → 3 sh. Stop advanced to $634 (entry+3R) on 4R milestone breach. |
| 2026-05-04 | NVDA | Stop fired @ $194.885 (10 sh) | +$179.55 / +10.1% | Entry 3/9 @ $176.93 |
| 2026-04-28 | INTC | Stop fired @ $81.50 (gap-down) | +$204 | Q1 blowout +29× then sleeve compression |
| 2026-04-28 | LRCX | Stop fired @ $245.94 | -$86 | US Commerce Hua Hong tool-ban |
| 2026-04-28 | BA | Stop fired @ $227.87 | +$44 | Airbus Q1 mixed peer-cohort |

---

## Today's Mercury alert highlights (~50 alerts)

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

## Tomorrow's autopilot_morning watchlist (top deferred)

| Score est | Ticker | Catalyst | Notes |
|-----------|--------|----------|-------|
| 92 | **FTNT** | Quintuple-positive Q1 cycle (print + Q2 guides + FY26 EPS + FY26 sales raise) | Cybersecurity mega-cap; pipeline-ready |
| 88 | **OGN** | $13B Sun Pharma sweetened takeover (+31%) | Takeover-arb shape, small position |
| 88 | **NBIS** | Eigen AI acquisition + META partnership (record highs) | AI-infra mid-cap |
| 85 | **DIS** | Q2 quadruple-positive (print + buyback + FY26 + FY27 guides) | Media mega-cap |
| 80 | **NVO** | Q1 +36% sales beat + FY26 guide raise + China moat | Pharma; sleeve room |
| 80 | **MET** | Q1 +23.47% YoY EPS beat | Insurance |
| 78 | **SHOP** | Q1 +34% YoY revenue + analyst PT raise | E-commerce/SaaS |
| 78 | **ARVN** | FDA breast cancer approval a month early (+10%) | Biotech (small only) |
| 75 | **MRNA** | Phase 3 mRNA-1010 NEJM publication + 4-jurisdiction filings | Counter-narrative to vaccine policy bears |
| 75 | **TEM** | Q1 +36.1% revenue beat + FY26 raise + multi-pharma partnerships | AI-diagnostics |

---

*Auto-generated by autopilot day recap; published to Buzzie-AI/trader-journal at 2026-05-06 18:38 ET.*
