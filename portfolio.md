---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-04 11:30 AM ET (Monday intraday — post-NVDA stopout)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$25,279.01** |
| Cash | $3,281.71 (13.0%) ✅ above $2K min-reserve |
| Invested | $21,997.30 (87.0%) |
| Positions | 12 equity + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **2 actions**: (1) MU stop $510 GTC placed AM (T+3 catch-up). (2) **NVDA stop fired 11:21 ET** — 10 sh @ $194.885 = +$179.55 realized / +10.1%. Cash freed $1,949 (binding constraint cleared). 0 BUYs (pipeline discipline — fresh autopilot fire required for any add). |
| Stop coverage | ✅ 11 active stops (BLK/CCI/CEG/CVS/CVX/MRK/MRVL/MU/NKE/NUE/TXN). Exempt: UNH (fractional), 737CVR019 (CVR), BTC (no Alpaca crypto stop). |
| 🎯 Best held | **CEG +14.6%** 🎯 (AI-power thesis, +4.20% intraday) · **BTC +12.5%** ($80K crossed Sun via Project Freedom + ETF inflows) · **CVS +8.8%** · **MU +6.9%** (HBM4 demand surge, +6.67% intraday) · **CCI +7.3%** · **UNH +27.1%** (fractional) |
| Day P&L | **+$185.58 / +0.74%** vs Friday close $25,093.43 |
| **Realized today** | **+$179.55** from NVDA stop (entry 3/9 @ $176.93, exit 5/4 @ $194.885, hold ~57d) |

---

## Equity Curve (1 Month)

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25279.01],
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
        min: 19000, max: 26000
      }
    }
  }
});
</script>

| Period | Start | End | Change | Notes |
|--------|-------|-----|--------|-------|
| **Today (May 4 intraday)** | $25,093 (Fri close) | $25,279 | **+0.74% (+$186)** | NVDA stop fired (+$180 realized); CEG +4.2%, MU +6.7% leading; cash binding cleared |
| 1 Week | $24,880 (Apr 30) | $25,279 | +1.6% | CVX/NUE stops + MU sleeve add (5/1); NVDA stopout (5/4) |
| **Since Agents (Mar 28)** | $20,489 | $25,279 | **+$4,790 (+23.4%)** | Excludes $3,000 Apr 23 deposit; agent P&L only ~+$1,790 (+8.7%) |
| Total equity (incl deposit) | $20,489 | $25,279 | +23.4% | |
| High | $25,379 (May 4 11:01 ET pre-stopout) | | | |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$1,790 (+8.7% in 37 days)**. The total-equity chart includes a $3,000 deposit on Apr 23 (purple dot).

Blue dashed line = sector-sleeve infrastructure deployed (Apr 23). Purple dot = $3K capital injection (Apr 23).

---

## Current Positions (intraday)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **CEG** | 7 | $280.00 | $320.75 | **+$285** | **+14.6%** 🎯 | 8.9% | $290 ✅ (above entry) |
| **CVS** 🎯 | 27 | $75.83 | $82.53 | +$181 | **+8.8%** | 8.8% | $75.83 ✅ (breakeven-lock) |
| **MU** 🆕 | 4 | $541.11 | $578.36 | +$149 | **+6.9%** | 9.2% | **$510 ✅ (placed today T+3)** |
| **CCI** | 20 | $84.31 | $90.49 | +$124 | +7.3% | 7.2% | $84.31 ✅ (breakeven-lock) |
| UNH | 0.69 | $290.00 | $368.60 | +$54 | **+27.1%** | 1.0% | — fractional exempt |
| **TXN** | 5 | $272.83 | $280.00 | +$36 | +2.6% | 5.5% | $254 ✅ |
| **BTC** | 0.0034 | $70,867 | $79,708 | +$31 | **+12.5%** | 1.1% | — crypto exempt |
| **MRVL** | 9 | $159.54 | $162.71 | +$29 | +2.0% | 5.8% | $145 ✅ |
| **MRK** | 18 | $112.47 | $113.82 | +$24 | +1.2% | 8.1% | $103.50 ✅ |
| **NUE** | 9 | $223.00 | $223.86 | +$8 | +0.4% | 8.0% | $210 ✅ |
| **CVX** | 10 | $191.92 | $192.57 | +$7 | +0.3% | 7.6% | $182 ✅ |
| BLK | 2 | $1,057.92 | $1,053.34 | -$9 | -0.4% | 8.3% | $990 ✅ |
| NKE | 44 | $45.29 | $43.44 | -$81 | -4.1% | 7.6% | $42.50 ✅ TIGHT |

**Total Open P&L: +$836 unrealized.** Today's intraday drivers: CEG +$91, MU +$145, CCI +$25, MRK +$30, CVX +$19; offset by NKE -$42, MRVL -$20, NUE -$20, BLK -$17.

**🚪 Closed today (realized):** NVDA 10 sh @ $194.885 = **+$179.55 / +10.1%** (stop fired 11:21 ET; entry 2026-03-09 @ $176.93).

---

## ⭐ Sector Sleeve Status (semi_ai)

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $6,320 (25%) | $5,178 (82%) | **UNDER target — priority queue ON** | MRVL, TXN, MU |

**Sleeve concentration:** 20.5% of equity (vs 25% target / 35% hard ceiling). NVDA exit dropped sleeve from 113% over to 82% under. Sleeve members: MRVL $1,464 / TXN $1,400 / MU $2,313. Dry powder: ~$1,142 toward target. **Priority queue active** — next autopilot will surface semi/AI candidates first (QCOM, INTC top scorers from this morning's Mercury cluster).

---

## Allocation (intraday)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (MRVL, TXN, MU) | $5,178 | 20.5% (under target) |
| Healthcare (MRK, CVS, UNH) | $4,531 | 17.9% |
| Utility/Nuclear (CEG) | $2,245 | 8.9% |
| Financials (BLK) | $2,107 | 8.3% |
| Materials (NUE) | $2,015 | 8.0% |
| Energy (CVX) | $1,926 | 7.6% |
| Consumer (NKE) | $1,911 | 7.6% |
| Real Estate (CCI) | $1,810 | 7.2% |
| Crypto (BTC) | $275 | 1.1% |
| **Cash** | **$3,282** | **13.0%** ✅ above $2K reserve |

Cash binding cleared by NVDA stopout. Semi/AI sleeve under-filled — high-conviction adds (QCOM, INTC) now executable through pipeline at next autopilot run, with sleeve priority routing favoring semi candidates over general.

---

## Open Orders (11 active stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 4 | $510 | GTC | 🆕 placed today AM (T+3 catch-up from 5/1 PDT-block) |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CVS | 27 | $75.83 | GTC | Breakeven-lock |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | TIGHT buffer ~$0.94 |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $254.00 | GTC | |
| Stop | CVX | 10 | $182.00 | GTC | Placed 5/1 (T+1 catch-up) |
| Stop | NUE | 9 | $210.00 | GTC | Placed 5/1 (T+1 catch-up) |

🚪 **Filled today:** NVDA 10 sh stop @ $195 → fill $194.885 (order `96e50d4c`). Position closed.

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| **2026-05-04** | **NVDA** | Stop fired @ $194.885 (10 sh) | **+$179.55 / +10.1%** | Entry 2026-03-09 @ $176.93. Stop placed 4/27 post-harvest-trim ($210.52 trim of 2 sh). Breakeven-lock above entry held; ~57d hold. |
| 2026-04-28 | INTC | Stop fired @ $81.50 (gap-down) | +$204 | Q1 blowout +29× then sleeve compression |
| 2026-04-28 | LRCX | Stop fired @ $245.94 | -$86 | US Commerce Hua Hong tool-ban cohort |
| 2026-04-28 | BA | Stop fired @ $227.87 | +$44 | Airbus Q1 mixed peer-cohort |
| 2026-04-23 | AEM | Stop fired @ $199.96 (open) | -$152 | Reversal of Apr 20 catalyst-buy |
| 2026-04-21 | NFLX | Reaper SELL | -$68 | Reed Hastings exit + weak guide |

---

## Mon premarket Mercury catalyst cluster (40+ alerts in last 4h)

**Tier-1 (autopilot_score ≥ 70 — now executable with cash freed):** QCOM (mystery chip deal +20% ~85), INTC (SambaNova antitrust clear + Sat dual-upgrade + 52-wk-high + perm CTO + Physical AI Group ~82), AMZN (6-deep multi-axis: Anthropic + OpenAI + JPM + supply chain + HUMAIN + DoW CMMC ~85), AMAT (NEXX AI packaging ~75), LMT/BA ($119B Israel ~78), PARA (MS double upgrade ~72), LLY (Q1 GLP-1 blockbuster ~74), JNJ (STELARA + CAPLYTA ~70), EBAY (board confirms $56B GME ~75), BTC ($80K cross + ETF inflows ~92, HELD)

**Tier-2 (60–69):** GS/BX (Anthropic JV), NOC (F-16), GOOGL/MSFT (data-center power constraint), CRM ($25B buyback), DHR/MASI merger, ABBV/AMGN (pharma cohort), CAT (analyst pivot), TSLA (DZ Bank capitulation), UBER (Ahold grocery)

**Bear-qualifiers:** AZN (FDA panel reject), NCLH (FY26 guidance cut), META (China Manus block + capex digest)

**Constraint update:** cash freed by NVDA stopout ($1,949 added to cash, total $3,282). All Tier-1 candidates now pass the Marcus min_reserve gate. **Sleeve priority routing favors semi candidates (QCOM, INTC) over general candidates** at next autopilot pipeline fire — sleeve regime HOT + fill 82% (under target).

---

## Recent autopilot debriefs

- [2026-05-04 09:18 ET (midday — streamlined)](debriefs/2026-05-04-0918.html) — 12 new alerts since morning, cash binding (now cleared by 11:21 stopout)
- [2026-05-04 05:58 ET (morning)](debriefs/2026-05-04-0558.html) — Full Mon-morning context, 22 Mercury alerts scored, MU stop placed
- [2026-05-01 16:23 ET (close)](debriefs/2026-05-01-1623.html)
- [2026-05-01 13:17 ET (midday)](debriefs/2026-05-01-1317.html)
- [2026-05-01 09:50 ET (morning)](debriefs/2026-05-01-0950.html)

---

## Architecture / Cron note

**Cron timezone bug active:** all configured ET cron expressions firing in UTC interpretation (4h early). Examples:
- `27 9 * * 1-5` (configured 9:27 ET) → fired at 5:58 ET premarket
- `47 12 * * 1-5` (configured 12:47 ET) → fired at 9:18 ET (12 min before market open)
- `3 8 * * *` renewal → fires at 4:33 ET

Net impact: autopilot_morning runs premarket without live mover data; midday runs near-open. The 06:00 ET autopilot is essentially redundant with 09:18 ET — wasting an analytical pass and not getting the 9:27 ET market-open scan that would surface real movers. Worth investigating before next trading session.
