---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-08 4:23 PM ET (Friday EOD — **MASSIVE DAY +$716 / +2.78%**. Closed at $26,483.61. Three executed trade-actions during the session under new autonomous policy plus 2 stop ratchets: **INTC TRIM 50% @ $116.37 = +$117.15 realized** (target hit), **BILL BUY 64 sh @ $40.17 = $2,571** (quad-bull catalyst-buy, +4.1% Day 1), **MU stop ratchet x2** ($634 → $665 → $700, locks +$478 on 3 sh), **INTC stop ratchet x2** ($108 → $118 → $120 EOD). Catalysts that drove the day: **WSJ EXCLUSIVE Apple-Intel chip deal CONFIRMED** → INTC +13.92%; **MU HBM thesis ACTIVATED** (SK Hynix bottleneck overnight + TSM April +17.5% + CoreWeave + 67% AI GDP) → MU +15.26%; **SOX 25-year HIGH**; AVGO Bloomberg confirmed $35B Apollo+Blackstone financing. Held semi cohort all green: MU +15.3%, INTC +13.9%, MRVL +6.4%, TXN +0.9%. Pipeline-discipline + autonomous execution working as designed.)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$26,483.61 EOD** |
| Cash | $2,732.77 (10.3%) — replenished post INTC trim |
| Invested | $23,750.84 (89.7%) |
| Positions | **13 equity** (added BILL today) + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **5 ACTIONS EXECUTED autonomously**: (1) **INTC TRIM** 6 sh @ $116.37 / realized **+$117.15** (target $115 hit at open); (2) **BILL BUY** 64 sh @ $40.17 = $2,571 (QUAD-bull catalyst-buy: Q3 +21.4% + Q4 guide above + FY26 raise + $1B buyback) closed +4.1% Day 1; (3) **MU stop ratchet x2** $634 → $665 (entry+4R) → $700 (entry+5R, locks +$478); (4) **INTC stop ratchet x2** $108 → $118 (post-WSJ Apple deal) → $120 (EOD); (5) **BILL stop $36** GTC placed same day (PDT cleared above $25K). |
| Stop coverage | ✅ 12 active stops on 12 stoppable equity positions (BILL $36 placed same-day per new PDT rule). |
| 🎯 Best held | **MU +37.7%** (3 sh, stop $700 = entry+5R) · **UNH +30.7%** (frac) · **INTC +28.9%** (6 sh post-trim, stop $120) · **CVS +19.4%** · **BTC +13.2%** · **CEG +9.2%** · **CCI +8.6%** · **MRVL +6.7%** |
| Day P&L | **+$715.73 / +2.78%** vs Wed last $25,767.88 |
| **Realized today** | **+$117.15** (INTC target trim 50%) |

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25251.27,25699.52,26182.80,25767.88,26483.61],
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
| **Today (May 8 EOD)** 🚀 | $25,767.88 (Thu last) | **$26,483.61** | **+2.78% (+$716)** 🚀 | INTC Apple-deal +13.9% / MU HBM-activation +15.3% / BILL bought 64sh @ $40.17 +4.1% / MRVL +6.4% / CVS +3.7%. INTC trim +$117 realized. SOX 25-year high. WSJ confirmed Apple-Intel preliminary chip agreement. |
| 1 Week | $25,251.27 (May 1) | $26,483.61 | **+4.9% (+$1,232)** | INTC sleeve compounding (+14.8% then +13.9%); MU HBM thesis from $541 → $745; CVS Q1 catalyst stack; BILL quad-bull catalyst-buy added; CVX stopped out 5/7 |
| **Since Agents (Mar 28)** | $20,489 | $26,483.61 | **+$5,995 (+29.3%)** | Excludes $3,000 Apr 23 deposit; agent P&L only ≈ +$2,995 (+14.6%) |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$2,995 (+14.6% in 41 days)**. The total-equity chart includes a $3,000 deposit on Apr 23 (purple dot).

---

## Current Positions (13 equity + 1 frac + 1 crypto, EOD May 8)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** 🚀🚀 | 3 | $541.11 | $745.33 | +$613 | **+37.7%** 🎯 | $700 | -6.1% (LOCKS +$478) |
| **CVS** 🎯 | 27 | $75.83 | $90.55 | +$397 | **+19.4%** | $82 | -9.4% |
| **INTC** (post-trim) | 6 | $96.85 | $124.88 | +$168 | **+28.9%** 🎯 | $120 | -3.9% (intentional EOD lock) |
| **CEG** | 7 | $280.00 | $305.73 | +$180 | **+9.2%** | $290 | -5.1% |
| **CCI** | 20 | $84.31 | $91.52 | +$144 | **+8.6%** | $84.31 | -7.9% |
| **BILL** 🆕 | 64 | $40.17 | $41.83 | +$106 | **+4.1%** | $36 | -13.9% |
| **MRVL** | 9 | $159.54 | $170.18 | +$96 | **+6.7%** | $145 | -14.8% |
| **TXN** | 5 | $272.83 | $287.80 | +$75 | +5.5% | $252.58 | -12.2% |
| **BLK** | 2 | $1,057.92 | $1,084.83 | +$54 | +2.5% | $990 | -8.7% |
| **NUE** | 9 | $223.00 | $227.50 | +$41 | +2.0% | $210 | -7.7% |
| **MRK** | 18 | $112.47 | $111.38 | -$20 | -1.0% | $103.50 | -7.1% |
| **NKE** | 44 | $45.29 | $44.14 | -$50 | -2.5% | $42.50 | -3.7% |
| **UNH** | 0.69 | $290.00 | $379.12 | +$61 | **+30.7%** | — frac | n/a |
| **BTC** | 0.0034 | $70,867 | $80,252 | +$32 | **+13.2%** | — crypto | n/a |
| 737CVR019 | 4.06 | $0 | (CVR) | — | — | — | — |

**Total open unrealized P&L: +$2,127.** **Realized today: +$117.15** (INTC target trim 50%).

⚠️ **Tight-stop watch into Monday:**
- **NKE** -3.7% buffer; recovering toward breakeven; smallest cushion.
- **INTC** -3.9% (intentionally tight — locks Apple-deal pop gains; if INTC pulls back next session this fires & locks +$144 on remaining 6 sh).
- **CEG** -5.1% buffer; AI-power softness today.
- **MU** -6.1% post-2-ratchet (locks +$478 on 3 sh; gap-risk acceptable).

🎯 **Today's hits:** INTC target $115 hit at AM → 50% trim auto-fired @ $116.37; MU HBM thesis activated → stop ratcheted twice to $700.

🚪 **Closed today:**
- **INTC** target trim 6 sh @ $116.37 (50% of 12) = **+$117.15 realized**. Apple-Intel chip deal then ran 6 remaining shares to $124.88.

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,621 (25%) | $5,956 (22.5%) | **89.9% fill** | MU $2,236 + INTC $749 + MRVL $1,532 + TXN $1,439 |

Sleeve fill dropped from 95.6% to 89.9% intentionally (INTC target-trim 50% executed at AM; sleeve members otherwise UP huge today: MU +15.3%, INTC +13.9% on remaining 6 sh, MRVL +6.4%). Regime: HOT (multi-week Mercury alert density). Sleeve dry powder $665 — could deploy on Monday if a sleeve catalyst (NVDA pre-May 20 earnings? ARM analyst cluster?) appears.

---

## Allocation (EOD May 8)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MU, INTC, MRVL, TXN) | $5,956 | 22.5% (89.9% of 25% target) |
| **SaaS (BILL — NEW)** | $2,677 | 10.1% |
| Healthcare (MRK, CVS, UNH) | $4,711 | 17.8% |
| Utility/Nuclear (CEG) | $2,140 | 8.1% |
| Financials (BLK) | $2,170 | 8.2% |
| Materials (NUE) | $2,048 | 7.7% |
| Consumer (NKE) | $1,942 | 7.3% |
| Real Estate (CCI) | $1,830 | 6.9% |
| Energy | **$0** | **0.0%** (CVX stopped out 5/7; sector ZERO-WEIGHT) |
| Crypto (BTC) | $277 | 1.0% |
| **Cash** | **$2,733** | **10.3%** — comfortably above $2K reserve |

---

## Open Orders (12 active stops, EOD May 8)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 3 | **$700.00** | GTC | Ratcheted x2 today: $634→$665→$700 (entry+5R locks +$478) |
| Stop | **INTC** | 6 | **$120.00** | GTC | Ratcheted x2 today: $108→$118→$120 (post WSJ Apple-deal lock) |
| Stop | CVS | 27 | $82.00 | GTC | Advanced 5/6 from BE-lock; consider $84 advance Mon |
| Stop | **BILL** 🆕 | 64 | $36.00 | GTC | Placed same-day per new PDT rule (>$25K equity) |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | Buffer -3.7% — TIGHTEST |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |

🚪 **Filled today:** INTC trim 6 sh @ $116.37 (target trim) — order `ce80fef6`, BILL buy 64 sh @ $40.17 — order `583aaa52`. Realized **+$117.15**.

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-08** 🎯 | **INTC** | Target trim 6 sh @ $116.37 (50%) | **+$117.15 / +20.1%** | Entry 5/4 @ $96.85. Target $115 hit at open. Then WSJ exclusive at 12:51 confirmed Apple-Intel chip deal → INTC ran to $124.88 on remaining 6 sh; stop ratcheted to $120 EOD. Discipline + autonomous policy worked perfectly. |
| **2026-05-07** | **CVX** | Stop fired @ $181.50 (10 sh) | **-$104.20 / -5.4%** | Entry 4/30 @ $191.92. Stop $182 GTC fired at 09:30 ET open print on XLE -2.13% sector drag. Energy sector now zero-weight. |
| 2026-05-06 | MU | 3R trim 1 sh @ $653.32 | +$112.21 / +20.7% | Entry 5/1 @ $541.11. Position 4 → 3 sh. Stop advanced to $634. |
| 2026-05-04 | NVDA | Stop fired @ $194.885 (10 sh) | +$179.55 / +10.1% | Entry 3/9 @ $176.93 |
| 2026-04-28 | INTC | Stop fired @ $81.50 (gap-down) | +$204 | Q1 blowout +29× then sleeve compression |
| 2026-04-28 | LRCX | Stop fired @ $245.94 | -$86 | US Commerce Hua Hong tool-ban |
| 2026-04-28 | BA | Stop fired @ $227.87 | +$44 | Airbus Q1 mixed peer-cohort |

---

## Today's Mercury alert highlights (~40 alerts, May 8)

- **WSJ EXCLUSIVE: Apple-Intel preliminary chip-making AGREEMENT** confirmed at 12:51 ET → INTC +13.9% to $124.88
- **MU HBM thesis ACTIVATION** — SK Hynix bottleneck overnight + TSM April +17.5% + CoreWeave + 67% AI GDP contribution → +15.3% to $745
- **SOX semiconductors hit 25-YEAR HIGH** — macro confirmation
- **NFP April +115K vs +62K est** — strong jobs (bear-rate-cuts but bull-economy)
- **DDOG 5-shop PT cluster** $218-225 post triple-bull print (Mizuho/UBS/MS/RBC/Citi)
- **ARM 5-shop PT cluster** + Barclays today
- **AVGO Bloomberg-confirmed $35B Apollo+Blackstone financing rumor** — eases OpenAI deal pressure
- **TCI/Hohn $8B MSFT stake slash** — high-profile activist exit on AI-disruption thesis (contrarian)
- **HHS Sec Kennedy antidepressant regulatory exploration** — pharma cohort overhang continues
- **HON Quantinuum IPO filing**; **MAR dividend hike**; **DIS Citi PT $145**
- **TPR sell-the-news recovery** (dip-buy candidate Mon)
- **NVDA pre-May 20 earnings stack** — GS estimate raise + IREN $3.4B + SoftBank Japan + Apple-INTC ecosystem

### Yesterday's highlights (May 7)

- DDOG triple-bull + FTNT triple + DKNG +10x consensus + AFRM triple — earnings tsunami day
- C $30B buyback + investor-day ROTCE roadmap (pipeline saved misread C buy)
- DIS quad-positive Q2 (BUY proposal expired AFK 1h — directly motivated 5/8 autonomous policy)
- BILL QUAD-bull post-close (acted on 5/8 morning)
- ZTS double-bear, MELI margin compression, COIN double-miss

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

## Today's autopilot watchlist additions (May 8 EOD)

| Score | Ticker | Catalyst | Action | Re-eval Trigger |
|------:|--------|----------|--------|-----------------|
| 88 | **DDOG** | 5-shop PT cluster $218-225 vs ~$192 = 14-17% upside | **DIP-BUY CANDIDATE** | Pullback over weekend or Mon open weakness |
| 85 | **NVDA** | GS estimate +12% pre-print + IREN $3.4B + SoftBank Japan + ecosystem | **PRE-EARNINGS WATCH** | May 20 print or pullback |
| 82 | **TPR** | Sell-the-news recovery from 5/7 -10% | **DIP-BUY CANDIDATE** | Tape stabilizes Mon |
| 78 | **HON** | Quantinuum IPO filing | **WATCH** | Spin-off catalyst, complex setup |
| 75 | **C** | (carryover from 5/7) Investor-day ROTCE roadmap | **WATCH** | ROTCE pace acceleration |
| 75 | **MCD** | (carryover) Q1 beat + comp accel | **WATCH** | Pullback to $280 |

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

*Auto-generated by autopilot_close fire (delayed-late at 16:21 ET); published to Buzzie-AI/trader-journal at 2026-05-08 16:30 ET.*
