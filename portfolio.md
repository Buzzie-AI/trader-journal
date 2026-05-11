---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-11 10:00 ET (Monday — Autopilot manual run executed AFTER scheduled `autopilot_morning` missed at 09:27 ET. **2 BUYS placed today** on the back of the heaviest Mercury catalyst day of the month (23 alerts in 4h): **AVGO 1sh @ $431.40 catalyst-buy (semi_ai sleeve, score 91 — record $35B private credit Apollo+Blackstone)** + **AMAT 1sh @ $441.47 catalyst-buy (semi_ai sleeve, score 82.75 — TSMC joint AI semi dev)**. Both bracket orders with stop+target legs armed. Cash flex invoked for AVGO (semi_ai HOT regime, 1/day). Daily trade cap reached 2/2. Reaper flagged NKE @ $42.98 vs $42.50 stop = 1.1% cushion (likely natural exit) and CEG @ $300.83 vs $290 stop = 3.7% cushion (Q1 mega-beat day vol; hold).)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$26,599.32** (intraday) |
| Cash | **$1,859.90** (7.0%) — post AVGO+AMAT spend; below normal $2K reserve, within flexed $1K floor |
| Invested | $24,739.42 (93.0%) |
| Positions | **15 equity** (added AVGO + AMAT today) + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **2 BUYS EXECUTED via bracket orders, both filled @ favorable prices**: (1) **AVGO BUY** 1 sh @ $431.40 (limit $433.50 — $2.10 better fill), bracket stop $407 / target $485, order `cf49e883`; (2) **AMAT BUY** 1 sh @ $441.47 (limit $444.50 — $3.03 better fill), bracket stop $416 / target $498, order `221aae7e`. Total spend $872.87. Cash flex invoked for AVGO (semi_ai HOT, score 91 ≥ 85, 1/day). Daily cap 2/2 reached. |
| Stop coverage | ✅ All 12 prior stops still GTC + 2 new bracket stops (AVGO $407, AMAT $416 — TIF=day until close, next harvest cron will convert to GTC). |
| 🎯 Best held | **MU +43.0%** (3 sh, stop $700 = entry+5R) · **INTC +31.3%** (6 sh, stop $120, AAPL foundry corroborated today) · **UNH +30.7%** (frac) · **CVS +21.3%** · **BTC +14.4%** · **CCI +9.0%** · **CEG +7.4%** · **TXN +7.8%** |
| Day P&L | **+$143.84 / +0.54%** vs Fri close $26,455.49 (intraday, before AVGO/AMAT settle) |
| **Realized today** | **$0** — no trims/exits |

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25251.27,25699.52,26182.80,25767.88,26455.49,26599.32],
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

**Mon May 11 intraday:** $26,599.32 (+$143.84 / +0.54% vs Fri close $26,455.49). Two semi-sleeve buys filled in first 30 min of session on heaviest Mercury catalyst day of the month.

---

## Current Positions (15 equity + 1 frac + 1 crypto, intraday May 11)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** 🚀🚀 | 3 | $541.11 | $773.70 | +$698 | **+43.0%** 🎯 | $700 | -9.5% (LOCKS +$478) |
| **INTC** 🎯 | 6 | $96.85 | $127.16 | +$182 | **+31.3%** 🎯 | $120 | -5.6% (intentional EOD lock) |
| **CVS** 🎯 | 27 | $75.83 | $91.95 | +$435 | **+21.3%** | $82 | -10.8% |
| **CEG** | 7 | $280.00 | $300.83 | +$146 | **+7.4%** ⚠️ | $290 | **-3.7%** (Q1 mega-beat vol — day low $291.83) |
| **CCI** | 20 | $84.31 | $91.87 | +$151 | **+9.0%** | $84.31 | -8.2% (breakeven lock) |
| **TXN** | 5 | $272.83 | $294.12 | +$106 | **+7.8%** | $252.58 | -14.1% |
| **MRVL** | 9 | $159.54 | $167.05 | +$68 | **+4.7%** | $145 | -13.2% |
| **BILL** 🆕 | 64 | $40.17 | $42.30 | +$136 | **+5.3%** | $36 | -14.9% |
| **BLK** | 2 | $1,057.92 | $1,080.41 | +$45 | +2.1% | $990 | -8.4% |
| **NUE** | 9 | $223.00 | $227.74 | +$43 | +2.1% | $210 | -7.8% |
| **AVGO** 🆕🆕 | 1 | **$431.40** | $432.42 | +$1 | +0.2% | **$407** | -5.7% (bracket day-TIF) |
| **AMAT** 🆕🆕 | 1 | **$441.47** | $443.54 | +$2 | +0.5% | **$416** | -5.8% (bracket day-TIF) |
| **MRK** | 18 | $112.47 | $113.05 | +$10 | +0.5% | $103.50 | -8.4% |
| **NKE** | 44 | $45.29 | $42.98 | -$101 | -5.1% | $42.50 | **-1.1%** ⚠️ (near-stop) |
| **UNH** | 0.69 | $290.00 | $378.54 | +$61 | **+30.5%** | — frac | n/a |
| **BTC** | 0.0034 | $70,867 | $81,080 | +$35 | **+14.4%** | — crypto | n/a |
| 737CVR019 | 4.06 | $0 | (CVR) | — | — | — | — |

**Total open unrealized P&L: ~$2,021** (intraday). **Realized today: $0**.

⚠️ **Tight-stop watch:**
- **NKE** -1.1% buffer (TIGHTEST). Down -2.6% intraday on consumer-disc weakness. Likely natural stop-out if tape weakens further; Reaper recommends acceptance of clean exit.
- **CEG** -3.7% buffer. Q1 mega-beat day vol; intraday low touched $291.83 (within $2 of stop). Hold; reassess at 12:47 midday.
- **AVGO/AMAT** -5.7%/-5.8% (initial bracket stops). Day-TIF → next harvest cron converts to GTC.

🎯 **Catalysts driving today's positions:**
- **AVGO** record $35B private credit (Apollo+Blackstone) — Mercury score 91, top of 23 alerts
- **AMAT** TSMC joint AI semi dev partnership — Mercury score 82.75
- **INTC** Apple foundry partnership CORROBORATED today (Sat TechStock² + Mon Benzinga two-source confirm) — +1.9% intraday after gap-up open
- **CEG** Q1 mega-beat (28% sales beat) but tape sold-the-news -0.9%
- **MU** continues to grind higher on HBM/AI capex thesis

🚪 **Closed today:** None.

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,650 (25%) | $6,931 (26.1%) | **104% of soft target** | MU $2,321 + INTC $763 + MRVL $1,503 + TXN $1,471 + **AVGO $432** 🆕 + **AMAT $443** 🆕 |

Sleeve regime: **HOT** (>5 qualifying alerts ≥70 in 7d window). Cash flex used today (1/1). Above soft target ($6,650) but under hard ceiling ($9,310 / 35%) — within design. Member-by-member: 2 mega-cap (MU, INTC, AVGO are now 3 mega-cap including new AVGO add), 2 mid-cap (MRVL, AMAT). Next semi catalyst that scores ≥70 would push us toward ceiling — would need harvest of a winner (MU at +43% is a candidate) before adding.

---

## Allocation (Intraday May 11)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MU, INTC, MRVL, TXN, AVGO, AMAT) | $6,931 | **26.1%** (104% of 25% target, under 35% ceiling) |
| **SaaS (BILL)** | $2,707 | 10.2% |
| Healthcare (MRK, CVS, UNH) | $4,779 | 18.0% |
| Utility/Nuclear/AI-Power (CEG) | $2,106 | 7.9% |
| Financials (BLK) | $2,161 | 8.1% |
| Materials (NUE) | $2,050 | 7.7% |
| Real Estate (CCI) | $1,837 | 6.9% |
| Consumer (NKE — near-stop) | $1,890 | 7.1% |
| Energy | $0 | 0.0% (CVX stopped out 5/7; sector still zero) |
| Crypto (BTC) | $280 | 1.1% |
| **Cash** | $1,860 | **7.0%** — below normal $2K reserve, within flexed $1K floor (semi_ai HOT cash flex active today) |

---

## Open Orders (14 active stops + 2 bracket take-profit legs)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 3 | **$700.00** | GTC | Entry+5R lock |
| Stop | **INTC** | 6 | **$120.00** | GTC | Post AAPL-deal lock |
| Stop | CVS | 27 | $82.00 | GTC | |
| Stop | BILL | 64 | $36.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | Buffer **-1.1%** — TIGHTEST |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |
| **Stop** | **AVGO** 🆕 | 1 | **$407.00** | day | Bracket leg — convert to GTC next harvest |
| **Take-profit** | **AVGO** 🆕 | 1 | **$485.00** | day | Bracket leg |
| **Stop** | **AMAT** 🆕 | 1 | **$416.00** | day | Bracket leg — convert to GTC next harvest |
| **Take-profit** | **AMAT** 🆕 | 1 | **$498.00** | day | Bracket leg |

🚪 **Filled today:** AVGO buy 1 sh @ $431.40 (order `cf49e883`), AMAT buy 1 sh @ $441.47 (order `221aae7e`). Total spend $872.87.

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-08** 🎯 | **INTC** | Target trim 6 sh @ $116.37 (50%) | **+$117.15 / +20.1%** | Apple-Intel deal then ran remaining 6 sh to $124.88. |
| 2026-05-07 | CVX | Stop fired @ $181.50 (10 sh) | -$104.20 / -5.4% | Energy sector now zero-weight (until today's CVX Mercury alert). |
| 2026-05-06 | MU | 3R trim 1 sh @ $653.32 | +$112.21 / +20.7% | Entry 5/1 @ $541.11 |
| 2026-05-04 | NVDA | Stop fired @ $194.885 (10 sh) | +$179.55 / +10.1% | Entry 3/9 @ $176.93 |
| 2026-04-28 | INTC | Stop fired @ $81.50 (gap-down) | +$204 | Q1 blowout +29× then sleeve compression |

---

## Today's Mercury catalyst stack (23 alerts in 4h, May 11)

**TOP TIER (score ≥ 80):**
- AVGO 91 mega_partnership — record $35B private credit (Apollo+Blackstone) 🟢 **BOUGHT 1 SH**
- MASI 85.5 acquisition_announced — DHR $10B takeover-arb (dropped, flat-tape arb asymmetry)
- AMAT 82.75 mega_partnership — TSMC joint AI semi dev 🟢 **BOUGHT 1 SH**
- CEG 81.75 earnings_beat — 28% Q1 sales mega-beat (HELD, hold)
- INTC ~85 mega_partnership — Apple foundry corroborated (HELD, runs)

**MID TIER (score 70-80):**
- CVX 77.75 (Q1+Iran-premium), AZN 77.75 (Q1), MKC 77.25 ($44.8B Unilever), KRYS 75.5 (FDA at-home Vyjuvek), BAM 75.5 ($500M OpenAI deploy), ABBV 75.25 (Capstan immuno), SITM 73.75 ($1.5B Renesas), NEE 71.75 (EPS reaff), OKLO 70 (NRC win)

**BEAR (no position):**
- DIS ~70 legal_regulatory — FCC censorship WSJ exclusive (watchlist only, no short)

---

*Generated by /autopilot manual run. Next scheduled fire: autopilot_midday at 12:47 ET.*
