---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-12 16:35 ET (Tue EOD — **Day -$136 / -0.51%** with **1 stop fire (INTC) realizing +$138.97 / +44% lifecycle.** Hot CPI + Iran oil triggered textbook risk-off rotation: tech XLK -3.2% / financials XLF +0.9% / healthcare XLV +2.3% / energy XLE +1.1%. **35+ Mercury alerts but 0 BUYs** — catalyst rejection pattern dominant (AMD/AVGO/ORCL/GS/AKAM/AFRM/MNDY/CRCL/TRI all bullish-catalyst-but-tape-sold). **QCOM -11% on $20B buyback** = sell-the-news mega-event explaining broader semi profit-taking. Top idio-alpha candidates CSCO (+3.21% vs XLK), META (+2.75%), FTNT (+1.77%) ALL BLOCKED by tech concentration at 36%. Semi sleeve survived deep stress test: **AMAT cushion 0.22% min / AVGO 0.45% min / MU 1.29% min** intraday lows, all stops held, recovered to 3.82% / 2.43% / 9.62% by close. **INTC stop $120 fired at 10:31 ET** = entry+5R lock did its job (1h11min detection latency → position-diff check deployed mid-session as remediation). **Wed AM action: CVS stop ratchet $82→$87** (lock +14.7%, was +8.2%) queued. Mag-7 product/AI day: GOOGL 4 alerts (SpaceX/Googlebook/AFRM-KLAR/AI engineers), META 2 (DESRI/WhatsApp AI), MSFT 1 (>2x OpenAI ROI), AAPL 1 (iOS 27).)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$26,439.85 EOD** |
| Cash | **$6,476.47** (24.5%) — includes $720 INTC stop proceeds |
| Invested | $19,963.38 (75.5%) |
| Positions | **13 equity** (INTC stopped) + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **1 stop fire**: INTC 6 sh @ $120.01 = **+$138.97 realized / +23.93%** (cost $96.85). 0 BUYs. |
| Stop coverage | ✅ 12 GTC stops on all positions; all survived deep stress test |
| 🎯 Best held EOD | **MU +41.8%** (3 sh @ $767, stop $700) · **UNH +36.7%** (frac) · **CVS +25.3%** ($95.00) · **BTC +14.1%** · **CCI +8.5%** · **TXN +8.2%** · **BLK +3.3%** |
| Day P&L | **-$136 / -0.51%** vs Mon close $26,575.95 |
| **Realized today** | **+$138.97** (INTC stop +44% lifecycle: 5/4 entry → 5/8 trim → 5/12 stop) |

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26439.85],
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

**Tue May 12 EOD:** $26,439.85 (-$136 / -0.51% vs Mon close $26,575.95). Net realized +$139 (INTC stop +44% lifecycle); unrealized down ~$275 across semi sleeve weakness. Stops held all day through deep stress test.

---

## Current Positions (13 equity + 1 frac + 1 crypto, EOD May 12)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** 🚀🚀 | 3 | $541.11 | $767.36 | +$679 | **+41.8%** 🎯 | $700 | -8.8% (locks +$478) |
| **UNH** | 0.69 | $290.00 | $396.50 | +$73 | **+36.7%** | — frac | n/a |
| **CVS** 🎯 | 27 | $75.83 | $95.00 | +$518 | **+25.3%** 🎯 | $82 | -13.7% (Wed AM ratchet to $87 queued) |
| **BTC** | 0.0034 | $70,867 | $80,863 | +$34 | **+14.1%** | — crypto | n/a |
| **CCI** | 20 | $84.31 | $91.50 | +$144 | **+8.5%** | $84.31 | -7.9% (breakeven lock) |
| **TXN** | 5 | $272.83 | $295.17 | +$112 | **+8.2%** | $252.58 | -14.4% |
| **MRVL** | 9 | $159.54 | $163.51 | +$36 | **+2.5%** | $145 | -11.3% |
| **BILL** | 64 | $40.17 | $41.27 | +$70 | **+2.7%** | $36 | -12.8% |
| **NUE** | 9 | $223.00 | $229.83 | +$61 | +3.1% | $210 | -8.6% |
| **BLK** | 2 | $1,057.92 | $1,092.50 | +$69 | +3.3% | $990 | -9.4% |
| **MRK** | 18 | $112.47 | $112.37 | -$2 | -0.1% | $103.50 | -7.9% |
| **AVGO** | 1 | $431.40 | $417.15 | -$14 | -3.3% | $407 | -2.4% (survived 0.45% min) |
| **AMAT** | 1 | $441.47 | $431.88 | -$10 | -2.2% | $416 | -3.8% (survived 0.22% min) |

**Total open unrealized P&L: ~$1,790 EOD**. **Realized today: +$138.97** (INTC stop).

⚠ **Stop stress test summary (semi sleeve):**
- AMAT: cushion 2.1% AM → **0.22% min at 12:57 ET** → 3.82% close
- AVGO: cushion 4.3% AM → **0.45% min at 12:42 ET** → 2.43% close
- MU: cushion 5.0% AM → **1.29% min at 12:42 ET** → 9.62% close

**All 3 semi sleeve stops survived the day's worst intraday pressure.** Discipline held.

🎯 **EOD catalysts driving positions:**
- **CVS +3.0% intraday** — healthcare cluster bull (XLV +2.3%) ignored TX AG threat
- **MU recovered +4.5% off lows** — Korea memory shockwave faded into close
- **AMAT/AVGO recovered** but still red vs Mon close
- **MRK +1.0%** — pharma cluster bull
- **BLK +1.0%** — financials rotation bull (XLF +0.9%)
- **UNH +3.1%** — healthcare cluster best
- **BILL -0.6%** — SaaS mild red on tech sell-off

🚪 **Closed today:** INTC stopped at $120.01 (6 sh, +$138.97). [Trade journal](trades/2026-05-12-INTC-stop-trigger). Total INTC trade lifecycle (entry 5/4 → trim 5/8 → stop 5/12): **+$256.12 / +44%**.

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,610 (25%) | $6,886 (26.0%) | **104% of soft target** | MU $2,302 + MRVL $1,472 + TXN $1,476 + AVGO $417 + AMAT $432 |

Sleeve regime: **HOT** but **TECH CONCENTRATION CEILING BINDING at 36.0%.** Total tech = semi $6,886 + BILL $2,641 (SaaS, tech-adjacent) = **$9,527 / 36.0% — over 35% hard ceiling.** No tech adds Wed until harvest of a winner (MU prime candidate at +41.8% / 5R+ lock).

---

## Allocation (EOD May 12)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI** (MU, MRVL, TXN, AVGO, AMAT) | $6,886 | 26.0% |
| **SaaS (BILL)** | $2,641 | 10.0% |
| **TECH TOTAL** | **$9,527** | **36.0%** ⚠ OVER 35% CEILING |
| Healthcare (MRK, CVS, UNH) | $4,861 | 18.4% |
| Financials (BLK) | $2,185 | 8.3% |
| Materials (NUE) | $2,068 | 7.8% |
| Real Estate (CCI) | $1,830 | 6.9% |
| Crypto (BTC) | $279 | 1.1% |
| **Cash** | $6,476 | **24.5%** |

---

## Open Orders (12 active GTC stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 3 | **$700.00** | GTC | Entry+5R; stress-tested 1.29% min |
| Stop | CVS | 27 | $82.00 | GTC | **Wed AM ratchet to $87 queued** (lock +14.7% vs +8.2%) |
| Stop | BILL | 64 | $36.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |
| Stop | **AVGO** | 1 | **$407.00** | GTC | Survived 0.45% min; 2.43% close |
| Stop | **AMAT** | 1 | **$416.00** | GTC | Survived 0.22% min; 3.82% close |

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-12** 🎯 | **INTC** | Stop fired @ $120.01 (6 sh) 10:31 ET | **+$138.97 / +23.93%** | Entry+5R lock; total INTC lifecycle +$256 / +44% across 5/4 entry → 5/8 trim → 5/12 stop. [Journal](trades/2026-05-12-INTC-stop-trigger) |
| 2026-05-11 | CEG | Stop fired @ $289.52 (7 sh) | +$66.64 / +3.4% | Q1 mega-beat sold-the-news |
| 2026-05-11 | NKE | Stop fired @ $42.50 (44 sh) | −$122.62 / −6.2% | Consumer-disc sector pressure |
| 2026-05-08 🎯 | INTC | Target trim 6 sh @ $116.37 | +$117.15 / +20.1% | Apple-Intel deal day |
| 2026-05-07 | CVX | Stop fired @ $181.50 | -$104.20 / -5.4% | |

---

## Today's Mercury Catalyst Stack (35+ alerts)

### Mag-7 Product/AI Cluster (8 alerts)
- **GOOGL** 4: AFRM/KLAR Gemini BNPL · WSJ SpaceX orbital data centers · Googlebook laptop · Hundreds of engineers AI customer adoption
- **META** 2: DESRI 850MW PPA (2.5GW total) · Free WhatsApp access for rival AI chatbots
- **MSFT** 1: >$26B revenue recouped (>2x its $13B OpenAI investment) per The Information
- **AAPL** 1: iOS 27 customizable Pro camera + Siri redesign per Bloomberg

### Tape REWARDED (positive idio alpha, all blocked by tech ceiling)
- CSCO +3.21% idio vs XLK — analyst upgrade pushing 1-yr high
- META +2.75% idio vs XLK — DESRI mega-partnership absorbed
- FTNT +1.77% idio vs XLK — NVDA AI security partner

### Tape REJECTED (catalyst-rejection pattern dominant)
- AMD Mizuho $515 PT — stock -5%
- AVGO Citi $500 PT — stock -3% (HELD position)
- ORCL Samsung Java SE win — stock -3%
- GS record GBM quarter — stock -1%
- **QCOM -11% on $20B buyback** = day's structural sell-the-news signal
- AFRM Google Pay (-2.04% idio alpha = INVALIDATED)
- AKAM upgrade — stock -4%
- MNDY record Q1 beat — stock -5%
- CRCL Q1 beat — stock -6%
- TRI × Anthropic Claude legal AI MCP — stock -2%

### Healthcare Cluster (XLV +2.3% best sector)
- AZN CALYPSO Phase 3 hit primary endpoint
- NVO Wegovy premenopausal 22.6% loss
- JNJ Shockwave C2 Aero global launch
- ARVN/PFE/RIGL VEPPANU $405M breast cancer licensing
- CVS analyst upgrade 52-wk high (HELD position +3%)

### Bearish / Legal / Regulatory
- **CVS** TX AG Medicaid fraud DEI warning (HELD; tape ignored)
- **PYPL** $30M DOJ DEI settlement
- **GTLB** RIF / restructuring
- **SEZL/SHOP** court allows antitrust claims to proceed (post-close)

### M&A / Strategic
- CRBG + EQH merger leadership team
- FCC approves SATS/T EchoStar 65MHz spectrum sale to SpaceX + 50MHz to AT&T
- VIST JPM PT $93 on M&A

---

## Watchlist for Wed (8 tickers)

| Ticker | Setup | Wed re-entry trigger |
|--------|-------|---------------------|
| **AFRM** | INVALIDATED — Google BNPL catalyst rejected | $69+ break with XLK green |
| **CSCO** | Strong relative strength; blocked by tech ceiling | Harvest MU/AVGO winner first OR pivot to financials |
| **META** | DESRI 2.5GW + product slate | Same — sector cap binding |
| **FTNT** | Cybersec-AI cluster | Sector cap binding |
| **AZN** | CALYPSO Phase 3 hit | 2nd shop / BLA timeline confirmation |
| **AVGO** | Citi $500 PT rejected today | Wed open price action |
| **AMD** | Mizuho $515 PT — rejected | Re-entry post sleeve harvest |
| **GS** | Record GBM rejected | Financials cluster bull leg confirmation |

---

## Wed AM Action Items

1. **CVS stop ratchet $82 → $87** (lock +14.7%, was +8.2%) — first action
2. Position-diff check after overnight tape
3. Re-evaluate AFRM/CSCO/META if XLK recovers
4. Consider MU 5R+ → 6R+ trim if breaks $800 (currently $767)

---

*Generated by autopilot_close (30 min late). Next scheduled fire: autopilot_morning Wed at 09:23 ET.*
