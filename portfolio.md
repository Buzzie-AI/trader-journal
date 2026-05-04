---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-04 11:01 AM ET (Monday intraday)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$25,378.57** |
| Cash | $1,333 (5.3%) ⚠️ below $2K min-reserve |
| Invested | $24,046 (94.7%) |
| Positions | 13 equity + BTC + UNH fractional + 737CVR019 (CVR) |
| Today's activity | **1 risk-mgmt action**: MU stop $510 GTC placed (T+3 catch-up, PDT-blocked at 5/1 buy time). 0 BUYs (cash binding < $2K reserve). 22+ Mercury alerts scored across 06:00 ET + 09:18 ET autopilot runs — Phase B pipeline deferred. |
| Stop coverage | ✅ 11 active stops (BLK/CCI/CEG/CVS/CVX/MRK/MRVL/MU/NKE/NUE/NVDA/TXN). Exempt: UNH (fractional), 737CVR019 (CVR), BTC (no Alpaca crypto stop). |
| 🎯 Best held | **CEG +15.4%** 🎯 (AI-power thesis, +4.97% intraday, Denmark data-center halt narrative bull-incremental) · **BTC +13.0%** ($80K crossed Sun overnight via Project Freedom + ETF inflows) · **NVDA +11.5%** (multi-axis bull holds despite China=$0 / Cerebras IPO bear-qualifiers) · **MU +8.0%** (HBM4 demand surge + QCOM mystery chip read-through, +7.82% intraday) · **CVS +8.8%** · **UNH +27.3%** (fractional) |
| Day P&L | **+$285 / +1.14%** vs Friday close $25,093.43 |

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
      data: [20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25129.32,25093.43,25378.57],
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
| **Today (May 4 intraday)** | $25,093 (Fri close) | $25,379 | **+1.14% (+$285)** | 0 BUYs (cash binding); 1 stop placement (MU $510); CEG +5%, MU +7.8% leading |
| 1 Week | $24,880 (Apr 30) | $25,379 | +2.0% | Friday: CVX/NUE stop placement; MU sleeve add. Weekend regime cluster (Project Freedom, CLARITY Act, AI partnership tectonic). |
| **Since Agents (Mar 28)** | $20,489 | $25,379 | **+$4,890 (+23.9%)** | Excludes $3,000 Apr 23 deposit; agent P&L only ~+$1,890 (+9.2%) |
| Total equity (incl deposit) | $20,489 | $25,379 | +23.9% | |
| High | $25,379 (May 4 intraday) | | | New all-time |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$1,890 (+9.2% in 37 days)**, annualized ~91%. The total-equity chart includes a $3,000 deposit on Apr 23 (purple dot).

Blue dashed line = sector-sleeve infrastructure deployed (Apr 23). Purple dot = $3K capital injection (Apr 23).

---

## Current Positions (intraday)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **CEG** | 7 | $280.00 | $323.13 | **+$302** | **+15.4%** 🎯 | 8.9% | $290 ✅ (above entry) |
| **NVDA** | 10 | $176.93 | $197.34 | +$204 | **+11.5%** | 7.8% | $195 ✅ (above entry) |
| **CVS** 🎯 | 27 | $75.83 | $82.51 | +$180 | **+8.8%** | 8.8% | $75.83 ✅ (breakeven-lock) |
| **MU** 🆕 | 4 | $541.11 | $584.61 | +$174 | **+8.0%** | 9.2% | **$510 ✅ NEW (T+3 catch-up)** |
| **CCI** | 20 | $84.31 | $90.17 | +$117 | +6.9% | 7.1% | $84.31 ✅ (breakeven-lock) |
| UNH | 0.69 | $290.00 | $369.05 | +$55 | **+27.3%** | 1.0% | — fractional exempt |
| **MRVL** | 9 | $159.54 | $164.88 | +$48 | +3.4% | 5.8% | $145 ✅ |
| **TXN** | 5 | $272.83 | $280.58 | +$39 | +2.8% | 5.5% | $254 ✅ |
| **BTC** | 0.0034 | $70,867 | $80,092 | +$32 | **+13.0%** | 1.1% | — crypto exempt |
| **NUE** | 9 | $223.00 | $225.60 | +$23 | +1.0% | 8.0% | $210 ✅ |
| MRK | 18 | $112.47 | $113.17 | +$13 | +0.6% | 8.0% | $103.50 ✅ |
| BLK | 2 | $1,057.92 | $1,060.53 | +$5 | +0.2% | 8.4% | $990 ✅ |
| CVX | 10 | $191.92 | $190.46 | -$15 | -0.8% | 7.5% | $182 ✅ |
| NKE | 44 | $45.29 | $43.86 | -$63 | -3.2% | 7.6% | $42.50 ✅ TIGHT |

**Total Open P&L: +$1,114 unrealized.** Today's intraday drivers (post-open): MU +$170, CEG +$107, MRK +$18, CCI +$18, CVS +$11; offset by NKE -$24, NVDA -$11.

---

## ⭐ Sector Sleeve Status (semi_ai)

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $6,345 (25%) | $7,199 (113%) | **OVER target, under 35% ceiling** | NVDA, MRVL, TXN, MU |

**Sleeve concentration:** 28.4% of equity (vs 25% target / 35% hard ceiling). Headroom for sleeve adds is restricted by hard ceiling, not target. Sleeve members: NVDA $1,973 / MRVL $1,484 / TXN $1,403 / MU $2,338. NVDA single-name 7.8% (under 12% NVDA-exception cap).

---

## Allocation (intraday)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (NVDA, MRVL, TXN, MU) | $7,199 | 28.4% ⚠️ |
| Healthcare (MRK, CVS, UNH) | $4,519 | 17.8% |
| Utility/Nuclear (CEG) | $2,262 | 8.9% |
| Financials (BLK) | $2,121 | 8.4% |
| Materials (NUE) | $2,030 | 8.0% |
| Consumer (NKE) | $1,930 | 7.6% |
| Energy (CVX) | $1,905 | 7.5% |
| Real Estate (CCI) | $1,803 | 7.1% |
| Crypto (BTC) | $276 | 1.1% |
| **Cash** | **$1,333** | **5.3%** ⚠️ below $2K reserve |

Highest concentration: semi_ai sleeve at 28.4% (over target but within ceiling). Cash below $2K min-reserve constrains all new BUYs.

---

## Open Orders (12 active stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **MU** | 4 | $510 | GTC | 🆕 placed today (T+3 catch-up from 5/1 PDT-block) |
| Stop | NVDA | 10 | $195.00 | GTC | Above entry; trail-up post-trim 04-27 |
| Stop | BLK | 2 | $990.00 | GTC | |
| Stop | CEG | 7 | $290.00 | GTC | Above entry |
| Stop | CVS | 27 | $75.83 | GTC | Breakeven-lock |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NKE | 44 | $42.50 | GTC | TIGHT buffer ~$1.36 |
| Stop | MRK | 18 | $103.50 | GTC | |
| Stop | MRVL | 9 | $145.00 | GTC | |
| Stop | TXN | 5 | $254.00 | GTC | |
| Stop | CVX | 10 | $182.00 | GTC | Placed 5/1 (T+1 catch-up) |
| Stop | NUE | 9 | $210.00 | GTC | Placed 5/1 (T+1 catch-up) |

---

## Mon premarket Mercury catalyst cluster (40+ alerts in last 4h)

**Tier-1 (autopilot_score ≥ 70):** BTC ($80K cross + ETF inflows ~92), AMZN (6-deep multi-axis: Anthropic + OpenAI + JPM + supply chain + HUMAIN + DoW CMMC ~85), QCOM (mystery chip deal +20% ~85), INTC (SambaNova antitrust clear + Sat dual-upgrade + 52-wk-high + perm CTO + Physical AI Group ~82), AMAT (NEXX AI packaging ~75), LMT/BA ($119B Israel ~78), PARA (MS double upgrade ~72), LLY (Q1 GLP-1 blockbuster ~74), JNJ (STELARA + CAPLYTA ~70), NVDA HELD (China=0 + Cerebras IPO mixed ~71), EBAY (board confirms $56B GME ~75)

**Tier-2 (60–69):** GS/BX (Anthropic JV), NOC (F-16), GOOGL/MSFT (data-center power constraint), CRM ($25B buyback), DHR/MASI merger, ABBV/AMGN (pharma cohort), CAT (analyst pivot), TSLA (DZ Bank capitulation), UBER (Ahold grocery)

**Bear-qualifiers:** AZN (FDA panel reject), NCLH (FY26 guidance cut), META (China Manus block + capex digest)

**Cash constraint binding:** every Tier-1 candidate blocks at Marcus due to $1,333 cash < $2,000 min-reserve. Operator decision: free $1-2K via winner trim (CEG +15%, BTC +13%, NVDA +11.5%, CVS +9%) to enable 1 high-conviction add (top: QCOM mystery chip / INTC SambaNova / LMT defense).

---

## Recent autopilot debriefs

- [2026-05-04 09:18 ET (midday — streamlined)](debriefs/2026-05-04-0918.html) — 12 new alerts since morning, cash binding, Phase B deferred
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

Net impact: autopilot_morning runs premarket without live mover data; midday runs near-open. Worth investigating before next trading session — the 06:00 ET autopilot is essentially redundant with 09:18 ET, so we're wasting an analytical pass and not getting the 9:27 ET market-open scan that would surface real movers.
