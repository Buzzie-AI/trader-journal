---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-12 09:58 ET (Tue intraday — **autopilot_morning ran 35 min late, 0 trades, 5 watchlisted.** 21 Mercury alerts in 4h window but tape risk-off rejecting most catalysts: ORCL/AMD/GS/AKAM all RED despite bullish news. Only XLV +1% green. Top pipeline candidates AFRM/CSCO/AZN all PASSED (Diana) — AFRM the cleanest setup with Google BNPL integration absorbing positive (+0.79% idio alpha vs XLF) but lacking breakout momentum off 5/8 -10% gap zone. Disciplined day: better entry $69+ on AFRM with tape confirmation. Semi sleeve at 104% fill + YELLOW stops (AMAT 2.1% cushion, INTC 3.3%, AVGO 4.3%) → no semi adds even on AMD Mizuho $515 upgrade.)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$26,341.78 intraday** |
| Cash | **$5,756.44** (21.9%) |
| Invested | $20,585.34 (78.1%) |
| Positions | **14 equity** + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **0 trades** (5 watchlisted: AFRM/CSCO/AZN/AMD/GS) |
| Stop coverage | ✅ 12 GTC stops (all major positions) — AVGO/AMAT GTC stops active post-Mon bracket-day expiry |
| 🎯 Best held intraday | **MU +41.4%** (3 sh @ $765, stop $700 +5R) · **UNH +32.2%** (frac) · **INTC +28.0%** (stop $120 ratchet) · **CVS +21.7%** · **BTC +13.6%** · **CCI +7.5%** · **TXN +6.3%** |
| Day P&L | **-$234 / -0.88%** vs Mon close $26,575.95 |
| **Realized today** | **$0** |

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26341.78],
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

**Tue May 12 intraday:** $26,341.78 (-$234 / -0.88% vs Mon close $26,575.95). Risk-off tape day; semi sleeve red across the board; no trades.

---

## Current Positions (14 equity + 1 frac + 1 crypto, intraday May 12 09:58 ET)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** 🚀🚀 | 3 | $541.11 | $765.32 | +$673 | **+41.4%** 🎯 | $700 | -8.5% (locks +$478) |
| **UNH** | 0.69 | $290.00 | $383.37 | +$64 | **+32.2%** | — frac | n/a |
| **INTC** 🎯 | 6 | $96.85 | $123.96 | +$163 | **+28.0%** 🎯 | $120 | -3.3% (YELLOW++) |
| **CVS** 🎯 | 27 | $75.83 | $92.25 | +$443 | **+21.7%** | $82 | -11.1% |
| **BTC** | 0.0034 | $70,867 | $80,500 | +$33 | **+13.6%** | — crypto | n/a |
| **CCI** | 20 | $84.31 | $90.62 | +$126 | **+7.5%** | $84.31 | -6.9% (breakeven lock) |
| **TXN** | 5 | $272.83 | $290.10 | +$86 | **+6.3%** | $252.58 | -12.9% |
| **BILL** | 64 | $40.17 | $41.57 | +$89 | **+3.5%** | $36 | -13.4% |
| **MRVL** | 9 | $159.54 | $165.46 | +$53 | **+3.7%** | $145 | -12.4% |
| **NUE** | 9 | $223.00 | $229.51 | +$59 | +2.9% | $210 | -8.5% |
| **BLK** | 2 | $1,057.92 | $1,076.36 | +$37 | +1.7% | $990 | -8.0% |
| **MRK** | 18 | $112.47 | $112.87 | +$7 | +0.4% | $103.50 | -8.3% |
| **AVGO** | 1 | $431.40 | $425.20 | -$6 | -1.4% | $407 | **-4.3%** (YELLOW) |
| **AMAT** | 1 | $441.47 | $424.67 | -$17 | -3.8% | $416 | **-2.1%** (YELLOW+++) |
| 737CVR019 | 4.06 | $0 | (CVR) | — | — | — | — |

**Total open unrealized P&L: ~$1,810** (intraday). **Realized today: $0**.

⚠️ **Tight-stop watch (Reaper YELLOW):**
- **AMAT** 2.1% stop cushion — fresh entry yesterday at $441.47; -3.8% day-2 already pressing $416 stop
- **INTC** 3.3% stop cushion — running winner +28%; ratchet stop $120 locks ~$140 profit per share if triggered (still +24% locked)
- **AVGO** 4.3% stop cushion — fresh yesterday entry; similar to AMAT but cleaner P&L

🎯 **Held catalysts (next 7 days):**
- **MU** AI/HBM thesis continues; no near-term earnings
- **CVS** today's Mercury alert: analyst upgrade pushes 52-wk high (+21.7% holding strong)
- **INTC** AAPL foundry tailwind running multi-week
- **AVGO/AMAT** semi sleeve members; AMD Mizuho upgrade today corroborates the sleeve thesis but sleeve full

🚪 **Closed today:** None.

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,585 (25%) | $6,830 (25.9%) | **104% of soft target** | MU $2,296 + INTC $744 + MRVL $1,489 + TXN $1,450 + AVGO $425 + AMAT $425 |

Sleeve regime: **HOT**. Above soft target — no new semi adds today even on AMD Mizuho $515 upgrade. Next move: harvest a winner (MU +41% is the candidate) before any sleeve refresh.

---

## Allocation (Intraday May 12 09:58 ET)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MU, INTC, MRVL, TXN, AVGO, AMAT) | $6,830 | **25.9%** (104% of 25% target, under 35% ceiling) |
| Healthcare (MRK, CVS, UNH) | $4,787 | 18.2% |
| **SaaS (BILL)** | $2,660 | 10.1% |
| Financials (BLK) | $2,153 | 8.2% |
| Materials (NUE) | $2,066 | 7.8% |
| Real Estate (CCI) | $1,812 | 6.9% |
| Crypto (BTC) | $278 | 1.1% |
| **Cash** | $5,756 | **21.9%** — well above $2K reserve |

---

## Open Orders (12 active GTC stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 3 | **$700.00** | GTC | Entry+5R lock |
| Stop | **INTC** | 6 | **$120.00** | GTC | Post AAPL-deal ratchet (YELLOW++ buffer) |
| Stop | CVS | 27 | $82.00 | GTC | |
| Stop | BILL | 64 | $36.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |
| Stop | **AVGO** | 1 | **$407.00** | GTC | YELLOW buffer 4.3% |
| Stop | **AMAT** | 1 | **$416.00** | GTC | YELLOW+++ buffer 2.1% |

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-11** | CEG | Stop fired @ $289.52 (7 sh) | **+$66.64 / +3.4%** | Q1 mega-beat sold-the-news at 11:09 ET |
| **2026-05-11** | NKE | Stop fired @ $42.50 (44 sh) | **−$122.62 / −6.2%** | Consumer-disc sector pressure at 14:54 ET |
| 2026-05-08 🎯 | INTC | Target trim 6 sh @ $116.37 (50%) | +$117.15 / +20.1% | Apple-Intel deal day |
| 2026-05-07 | CVX | Stop fired @ $181.50 (10 sh) | -$104.20 / -5.4% | Energy sector zero-weight again |
| 2026-05-06 | MU | 3R trim 1 sh @ $653.32 | +$112.21 / +20.7% | Entry 5/1 @ $541.11 |

---

## Today's Mercury catalyst stack (21 alerts in 4h, Tue May 12)

**Top scored (≥ 70):**
- **AFRM 75-82** partnership_deal — Google Pay BNPL integration in Gemini App + Search (TAM expansion) — **WATCHLIST** ($69+ re-entry)
- **AZN 70** fda_approval — CALYPSO Phase 3 hit composite primary endpoint (rare-disease orphan win) — WATCHLIST

**Score 60-70:**
- ORCL (Samsung Java SE) — tape faded; PASS
- AMD (Mizuho PT $515) — sleeve full; PASS
- FTNT (NVDA AI partner) — marginal alpha; WATCHLIST
- GS (record GBM quarter) — tape faded; PASS
- CSCO (analyst upgrade 1-yr high) — relative strength but single-shop; PASS
- VIST (JPM PT $93 on M&A) — Argentine ADR; PASS

**Bearish absorption (tape rejecting catalyst):**
- AI (C3.ai) -6.4% on prelim Q4 + Siebel CEO return
- AKAM -4.0% despite upgrade
- ORCL -4.3% despite Samsung halo win

**Healthcare cluster (XLV +1% only green sector):** NVO Wegovy, JNJ Shockwave, AZN Phase 3, ARVN/PFE/RIGL $405M licensing — modest individual absorption

---

## Watchlist (5 tickers from today)

| Ticker | Setup | Re-entry trigger |
|--------|-------|-----------------|
| **AFRM** | Google BNPL integration | $69+ break with XLK green |
| AZN | CALYPSO Phase 3 hit | BLA timeline guidance + pharma cluster bull leg |
| CSCO | Analyst upgrade 1-yr high | 2nd shop upgrade (cluster confirmation = +20 score) |
| AMD | Mizuho PT $515 continuation | Wait for sleeve harvest (MU candidate) + tape confirmation |
| GS | Record GBM quarter | Tape green + financials sector recovery |

---

*Generated by autopilot_morning (35 min late). Next scheduled fire: autopilot_midday at 12:47 ET.*
