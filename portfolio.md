---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-12 13:30 ET (Tue midday — **autopilot_midday ran 26 min late, 0 trades, 8 watchlisted.** Big macro pivot since AM: **hot CPI print + Iran oil = textbook risk-off rotation** — tech XLK -3.02% (worse from -1.57% AM), financials XLF flipped to +0.90%, healthcare XLV +2.32%, energy XLE +1.08%. **INTC stopped out 10:31 ET @ $120.01 = +$138.97 realized** (entry+5R lock did its job; +44% across full trade lifecycle). Position-diff check added to mercury cron after 1h11min INTC detection lag — would have caught it in 5-8 min. Semi sleeve survived deep stress test: AMAT cushion hit 0.22% / AVGO 0.45% / MU 1.29% intraday lows, all stops held, afternoon bounce recovered to 0.95% / 0.89% / 3.69%. Top idio-alpha pipeline candidates (CSCO +3.21%, META +2.75%, FTNT +1.77% vs XLK) ALL BLOCKED by tech sector concentration at 36% (over 35% hard ceiling). No tech adds without harvest of a tech winner (MU +41% candidate).)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$26,200.29 intraday** |
| Cash | **$6,476.47** (24.7%) — well above $2K reserve, +$720 post INTC stop |
| Invested | $19,723.82 (75.3%) |
| Positions | **13 equity** (INTC stopped out 10:31 ET) + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **1 stop fire**: INTC 6 sh @ $120.01 = **+$138.97 realized / +23.93%** (cost $96.85). 0 BUYs. |
| Stop coverage | ✅ 12 GTC stops (all major positions); AVGO/AMAT survived deep stress test |
| 🎯 Best held intraday | **MU +32.4%** (3 sh @ $725.85, stop $700) · **UNH +35.5%** (frac) · **CVS +24.7%** ($94.68, +24% on +2.6% intraday) · **BTC +12.9%** · **CCI +8.3%** · **TXN +5.7%** |
| Day P&L | **-$376 / -1.41%** vs Mon close $26,575.95 |
| **Realized today** | **+$138.97** (INTC stop) |

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
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26200.29],
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

**Tue May 12 intraday:** $26,200.29 (-$376 / -1.41% vs Mon close $26,575.95). Hot CPI + Iran oil triggered tech sell-off; semi sleeve survived deep stress test (AMAT/AVGO/MU stops all held through afternoon lows).

---

## Current Positions (13 equity + 1 frac + 1 crypto, intraday May 12 13:30 ET)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **MU** 🚀🚀 | 3 | $541.11 | $725.85 | +$554 | **+34.1%** 🎯 | $700 | -3.7% (locks +$478) |
| **UNH** | 0.69 | $290.00 | $393.27 | +$71 | **+35.6%** | — frac | n/a |
| **CVS** 🎯 | 27 | $75.83 | $94.68 | +$506 | **+24.7%** | $82 | -13.4% (consider 3R trim) |
| **BTC** | 0.0034 | $70,867 | $79,995 | +$31 | **+12.9%** | — crypto | n/a |
| **CCI** | 20 | $84.31 | $91.34 | +$140 | **+8.3%** | $84.31 | -7.7% (breakeven lock) |
| **TXN** | 5 | $272.83 | $289.99 | +$86 | **+6.3%** | $252.58 | -12.9% |
| **MRVL** | 9 | $159.54 | $159.46 | -$1 | **-0.05%** | $145 | -9.1% |
| **BILL** | 64 | $40.17 | $40.75 | +$37 | **+1.4%** | $36 | -13.3% |
| **NUE** | 9 | $223.00 | $230.86 | +$71 | +3.5% | $210 | -9.0% |
| **BLK** | 2 | $1,057.92 | $1,084.90 | +$54 | +2.6% | $990 | -8.7% |
| **MRK** | 18 | $112.47 | $113.42 | +$17 | +0.8% | $103.50 | -8.7% |
| **AVGO** | 1 | $431.40 | $410.63 | -$21 | -4.8% | $407 | **-0.9%** YELLOW (stress-tested 0.45% min) |
| **AMAT** | 1 | $441.47 | $419.94 | -$22 | -4.9% | $416 | **-0.9%** YELLOW (stress-tested 0.22% min) |

**Total open unrealized P&L: ~$1,495** (intraday). **Realized today: +$138.97** (INTC stop).

⚠ **Stop stress test summary (semi sleeve):**
- AMAT: cushion path 2.1% AM → **0.22% (~$0.90 above stop)** 13:03 → 0.95% recovered
- AVGO: cushion path 4.3% AM → **0.45%** 12:42 → 0.89% recovered
- MU: cushion path 4.98% AM → **1.29%** 12:42 → 3.69% recovered

All 3 stops held through the worst intraday pressure. **MU down -8.7% intraday but $478 still locked via $700 stop.** Discipline > urgency.

🎯 **Catalysts being faded today (catalyst rejection pattern):**
- AFRM Google BNPL +0.4% morning → -1.14% mid (-2.04% idio alpha) **INVALIDATED**
- ORCL Samsung Java -4.3%
- AMD Mizuho $515 -4.95%
- GS record GBM -1.04%
- AVGO Citi $500 PT -4.07%
- AKAM upgrade -4.0%
- MNDY record Q1 beat -5.3%
- CRCL Q1 beat -6.36%
- TRI × Anthropic Claude -2.08%
- AI Siebel CEO + prelim Q4 -6.4%

🚪 **Closed today:** INTC stopped at $120.01 (6 sh, +$138.97). [Trade journal](trades/2026-05-12-INTC-stop-trigger)

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $6,550 (25%) | $6,830 (26.1%) | **104% of soft target** | MU $2,178 + MRVL $1,435 + TXN $1,450 + AVGO $411 + AMAT $420 |

Sleeve regime: **HOT** but **TECH CONCENTRATION CEILING BINDING.** Total tech = semi $6,830 + BILL $2,608 (SaaS, tech-adjacent) = **$9,438 = 36.0%, over 35% hard ceiling.** No tech adds today regardless of catalyst quality. Sleeve refresh requires harvest of a winner (MU candidate at +34% with 5R lock).

---

## Allocation (Intraday May 12 13:30 ET)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI** (MU, MRVL, TXN, AVGO, AMAT) | $6,830 | 26.1% |
| **SaaS (BILL)** | $2,608 | 10.0% |
| **TECH TOTAL** | **$9,438** | **36.0%** ⚠ OVER 35% CEILING |
| Healthcare (MRK, CVS, UNH) | $4,839 | 18.5% |
| Financials (BLK) | $2,170 | 8.3% |
| Materials (NUE) | $2,077 | 7.9% |
| Real Estate (CCI) | $1,826 | 7.0% |
| Crypto (BTC) | $276 | 1.1% |
| **Cash** | $6,476 | **24.7%** |

---

## Open Orders (12 active GTC stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 3 | **$700.00** | GTC | Entry+5R lock — stress-tested 1.29% cushion 12:42, held |
| Stop | CVS | 27 | $82.00 | GTC | +24.7% / +$506; 3R milestone reached, consider ratchet |
| Stop | BILL | 64 | $36.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $252.58 | GTC | |
| Stop | NUE | 9 | $210.00 | GTC | |
| Stop | **AVGO** | 1 | **$407.00** | GTC | YELLOW 0.9% buffer (stress-tested 0.45%) |
| Stop | **AMAT** | 1 | **$416.00** | GTC | YELLOW 0.9% buffer (stress-tested 0.22%) |

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-12** 🎯 | **INTC** | Stop fired @ $120.01 (6 sh) 10:31 ET | **+$138.97 / +23.93%** | Entry+5R lock did its job; total INTC trade +$256.12 / +44% across lifecycle. [Journal](trades/2026-05-12-INTC-stop-trigger) |
| 2026-05-11 | CEG | Stop fired @ $289.52 (7 sh) | +$66.64 / +3.4% | Q1 mega-beat sold-the-news |
| 2026-05-11 | NKE | Stop fired @ $42.50 (44 sh) | −$122.62 / −6.2% | Consumer-disc sector pressure |
| 2026-05-08 🎯 | INTC | Target trim 6 sh @ $116.37 | +$117.15 / +20.1% | Apple-Intel deal day |
| 2026-05-07 | CVX | Stop fired @ $181.50 | -$104.20 / -5.4% | Energy zero-weight |
| 2026-05-06 | MU | 3R trim 1 sh @ $653.32 | +$112.21 / +20.7% | |

---

## Today's Mercury Catalyst Stack (30+ alerts since 04:02 ET)

### Tape REWARDED (positive idio alpha) — BUT all 3 blocked by tech concentration
- **CSCO** analyst upgrade pushes 1-yr high (+3.21% idio vs XLK)
- **META** DESRI 850MW PPA / 2.5GW partnership (+2.75% idio vs XLK)
- **FTNT** NVDA AI security partner (+1.77% idio vs XLK)

### Tape REJECTED (catalyst faded)
- AFRM Google Pay Gemini BNPL (-2.04% idio) **INVALIDATED**
- AMD Mizuho $515 PT (-1.93% idio)
- ORCL Samsung Java SE (-2.73% idio)
- GS record GBM (-1.94% idio)
- AKAM upgrade 12-mo high (-2.43% idio)
- TRI × Anthropic Claude legal AI (-2.08% absolute)
- MNDY record Q1 beat + AI ramp (-5.3% absolute)
- CRCL Q1 beat + Arc Token upside carved out (-6.36% absolute)
- AI Siebel CEO + prelim Q4 (-6.4% absolute)

### Macro signals
- **QCOM -11% on $20B buyback** = sell-the-news mega-event; explains broader semi profit-taking
- **PYPL $30M DOJ DEI settlement** — paired with CVS TX AG threat; DEI enforcement wave
- **CVS TX AG Medicaid fraud threat** (HELD POSITION — tape ignored)

### Healthcare cluster (XLV +2.32% best sector)
- NVO Wegovy premenopausal 22.6% loss
- AZN CALYPSO Phase 3 hit primary endpoint
- ARVN/PFE/RIGL $405M VEPPANU licensing
- JNJ Shockwave C2 Aero launch

### M&A/Partnership
- CRBG + EQH leadership team merger step
- GOOGL × SpaceX orbital data centers (WSJ exclusive)
- AFRM/KLAR × Google Pay BNPL cluster
- VIST JPM PT $93 on M&A

---

## Watchlist (8 tickers from today)

| Ticker | Setup | Re-entry trigger |
|--------|-------|-----------------|
| **CSCO** | +3.21% idio strong; blocked by tech concentration | Harvest MU/AVGO winner first, OR pivot to financials |
| **META** | DESRI 2.5GW + Google product slate, blocked by concentration | Same — sector cap binding |
| **FTNT** | NVDA AI security cluster (with PANW Idira) | Sector cap binding |
| AFRM | **INVALIDATED** by tape rejection | Wait for $63-64 bounce + tape recovery |
| AZN | CALYPSO Phase 3 hit (no idio edge today) | 2nd shop / BLA timeline confirmation |
| MNDY | Record Q1 + AI ramp but tape selling | Watch $70 bounce |
| CRCL | Q1 beat sold | Watch $115 stabilization |
| TRI | Anthropic Claude legal AI | AI-infra tape recovery |

---

*Generated by autopilot_midday (26 min late). Next scheduled fire: autopilot_close at 15:53 ET.*
