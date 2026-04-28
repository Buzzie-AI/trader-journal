---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-04-28 4:46 PM ET (Tuesday EOD)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$24,909.59** |
| Cash | $7,424 (29.8%) |
| Invested | $17,486 (70.2%) |
| Positions | 10 equity + BTC + UNH fractional |
| Today's activity | **🚨 3 STOPS TRIGGERED** — INTC $82→$81.50 (+$204) · LRCX $246→$245.94 (-$86) · BA $228→$227.87 (+$44) = **+$162.04 net realized**. TXN $254 stop placed AM (T+1 PDT clear). 0 discretionary trades. |
| Stop coverage | ✅ All 9 active equity positions stopped |
| 🎯 Best held | CVS +3.3% to $80.98 (CNC peer-cohort bull working) · CCI +3.7% to $86.50 (AMT+WELL REIT cohort bull) |
| 🎯 Sleeve compression | After INTC + LRCX stops: sleeve 78% of target ($4,857/$6,230); ~$1,373 dry powder for post-Fed Wed redeploy |

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
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59],
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
          handoverLine: {
            type: 'line',
            xMin: 'Mar 28',
            xMax: 'Mar 28',
            borderColor: '#f59e0b',
            borderWidth: 2,
            borderDash: [6, 4]
          },
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
| **Since Agents (Mar 28) — agent P&L only** | $20,489 | **~$22,069** | **+$1,580 (+7.7%)** | Excludes $3,000 Apr 23 deposit |
| 1 Month — agent P&L only | $23,448 | ~$22,069 | -5.9% | Excludes deposit; broader market context |
| Total equity (incl deposit) | $20,489 | $25,069 | +22.4% | Inflated by $3K Apr 23 deposit |
| Today (Apr 27) | $25,097 (Fri close) | $25,069 | **-0.11% (-$28)** | +$66.48 realized (NVDA trim) |
| Low | $20,408 (Mar 31) | | | |
| High | $25,105 (Apr 24 close) | | | (incl deposit) |

**Honest framing:** Agent-driven trading P&L since Mar 28 = **+$1,580 (+7.7% in 31 days)**, annualized ~78%. The total-equity chart includes a $3,000 deposit on Apr 23 — without that deposit, the underlying portfolio would be ~$22,069 today. The Apr 23→24 jump on the equity chart is mostly the deposit (~$3K) plus a smaller trading gain.

Orange dashed line = agents took control (Mar 28). Blue dashed line = sector-sleeve infrastructure deployed (Apr 23). Purple dot = $3K capital injection (Apr 23).

---

## Current Positions (post-close)

| Ticker | Shares | Entry | Last | P&L | P&L % | Weight | Stop |
|--------|--------|-------|------|-----|-------|--------|------|
| **NVDA** | **10** (was 12) | $177.28 | **$217.24** | **+$400** | **+22.5%** 🎯 | 8.7% | **$195 ✅ (trail-up post-trim)** |
| **INTC** | 14 | $66.94 | **$84.69** | **+$248** | **+26.5%** 🎯 | 4.7% | **$82 ✅ (re-placed today after anomaly)** |
| **CEG** | 7 | $280.00 | $315.89 | **+$251** | **+12.8%** 🎯 | 8.8% | **$290 ✅ (re-placed today after anomaly)** |
| **TXN 🆕** | 5 | $272.83 | $269.68 | -$16 | -1.2% | 5.4% | $254 PENDING T+1 |
| BA | 9 | $222.99 | $231.04 | +$72 | +3.6% | 8.3% | **$228 ✅ (trailed today)** |
| MRVL | 9 | $159.54 | $158.00 | -$14 | -1.0% | 5.7% | **$145 ✅ (placed today T+1 cleared)** |
| LRCX | 4 | $267.37 | $259.04 | -$33 | -3.1% | 4.1% | $246 ✅ |
| MRK | 18 | $112.47 | $112.45 | flat | flat | 8.1% | $103.50 ✅ |
| CVS | 27 | $75.83 | $78.09 | +$61 | **+3.0%** | 8.4% | $72.08 ✅ |
| CCI | 20 | $84.31 | $83.44 | -$17 | -1.0% | 6.7% | $80 ✅ |
| BLK | 2 | $1,057.92 | $1,049.00 | -$17 | -0.8% | 8.4% | $990 ✅ |
| NKE | 44 | $45.29 | $45.29 | flat | flat | 7.9% | $42.50 ✅ |
| BTC | 0.0034 | $70,867 | $77,693 | +$24 | **+9.6%** | 1.1% | — |
| UNH | 0.69 | $290.00 | $351.49 | +$42 | **+21.2%** | 1.0% | — |

**Total Open P&L: +$1,001** (mixed day; INTC + NVDA + CEG drive most of unrealized basket).

---

## ⭐ Sector Sleeve Status (Day 3 of deployment)

| Sleeve | Regime | Target | Current Fill | Status | Members Held |
|--------|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | 🔥 HOT | $6,267 (25%) | $7,164 (114%) | OVER TARGET (within 80-110% band stretched by appreciation) | NVDA, LRCX, INTC, MRVL, **TXN 🆕** |

**Day 3 sleeve activity:**
- TXN sleeve add filled @ $272.83 (5 sh, 5.4% of portfolio — within 6% per-name cap)
- NVDA Harvest trim 2 sh @ $210.52 = +$66.48 realized; remaining 10 sh at +22.5% unrealized; stop trailed to $195

**Cumulative sleeve P&L (Days 1-3):**
- INTC: +$401 realized + $248 unrealized = **$649**
- NVDA: +$66 realized + $400 unrealized = **$466**
- LRCX: -$33 unrealized
- MRVL: -$14 unrealized
- TXN: -$16 unrealized (Day 1)
- **Total sleeve P&L: +$1,052 over 3 days**

**Sleeve weight:** 28.6% portfolio (target 25%, ceiling 35%) — within band.

---

## Allocation (post-close)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI sleeve** (NVDA, INTC, LRCX, MRVL, TXN) | $7,164 | 28.6% |
| Aerospace (BA) | $2,079 | 8.3% |
| Healthcare (MRK, CVS, UNH) | $4,367 | 17.4% |
| Financials (BLK) | $2,098 | 8.4% |
| Consumer (NKE) | $1,993 | 7.9% |
| Utility/Nuclear (CEG) | $2,211 | 8.8% |
| Real Estate (CCI) | $1,669 | 6.7% |
| Crypto (BTC) | $264 | 1.1% |
| **Cash** | **$3,248** | **13.0%** |

Eight sectors. Highest concentration: semi_ai sleeve at 28.6% (target 25%, max 35% with forced Harvest trim above).

---

## Open Orders

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| **Stop** | **NVDA** | **10** | **$195.00** | GTC | **Trailed up from $185 post-trim** |
| Stop | BLK | 2 | $990.00 | GTC | |
| **Stop** | **CEG** | **7** | **$290.00** | GTC | **Re-placed today (overnight cancel anomaly)** |
| Stop | CVS | 27 | $72.08 | GTC | |
| Stop | NKE | 44 | $42.50 | GTC | |
| Stop | CCI | 20 | $80.00 | GTC | |
| Stop | MRK | 18 | $103.50 | GTC | |
| **Stop** | **BA** | **9** | **$228** | GTC | **Trailed today from $223** |
| Stop | LRCX | 4 | $246 | GTC | |
| **Stop** | **INTC** | **14** | **$82** | GTC | **Re-placed today (overnight cancel anomaly)** |
| **Stop** | **MRVL** | **9** | **$145** | GTC | **Placed today (T+1 PDT clear)** |
| (pending) | **TXN** | **5** | **$254** | GTC | **To place Tuesday morning (PDT same-day block)** |

---

## Recently Closed (last 7 days)

| Ticker | Entry | Exit | Return | Reason |
|--------|-------|------|--------|--------|
| **NVDA (partial)** | $177.28 | $210.52 | **+$66.48 (+18.7%)** | **Harvest trim Apr 27 — 2 sh; remaining 10 sh +22.5%** |
| **INTC (partial)** | $66.94 | $83.00 | +$401 (+24.0%) | Harvest trim Apr 24 — 5 sh; remaining 14 sh |
| AEM | $215.20 | $199.96 | -$152 (-7.1%) | Stop trigger Apr 23 open |
| NFLX | $97.00 | $93.89 | -$68 (-3.2%) | Reaper sell Apr 21 (Hastings exit) |
| MU | $375.00 | ~$438 | +$315 (+16.8%) | Stop trigger after Samsung-strike |
| PANW | $160.15 | $164.97 | +$58 (+3.0%) | Stop discipline WIN |
| DDOG | $119.00 | $104.95 | -$225 (-11.8%) | Stop discipline LOSS CUT |

---

## Today's Trades (2/2 daily cap used)

1. **NVDA TRIM** 2 sh @ limit $209.50 (filled $210.52) — Harvest +15-25% trim window; locks +$66.48 realized
2. **TXN BUY** 5 sh @ limit $275 (filled $272.83) — Sleeve catalyst-buy: 4-catalyst stack (17 PT hikes + data center +90% + Q1 +22.6% EPS + Q2 guide above consensus) post 5-agent debate

## Tuesday (Apr 28) priority stack

1. **Place TXN stop $254 GTC** (T+1 PDT clear)
2. **Verify INTC + CEG + all 11 stops still active** — recurrence check after Apr 27 anomaly
3. **INTC Reaper agent debate**: Gawel-reframe means INTC bull stack now UNCHALLENGED. Consider extending stop higher to $84-85 OR 2nd Harvest trim if INTC gaps higher
4. **NVDA position**: possibly trim 1 more sh if extends past +25%; Gawel hire is mild bullish offset to Burry SOXX puts + CDNS beat-punished bears
5. Sleeve cohort considerations: AVGO + QCOM remain candidates (CDNS removed from add-list)
6. Healthcare cluster (12 catalysts/10 names this week): AZN, JNJ, ABBV, GSK
7. LMT defense (Golden Dome + F-35 + Peru F-16 stack)

---

## Architecture note

Cron-delivery delays persisted throughout Apr 27 (morning +30 min, midday +26, close +32). The Apr 24 schedule fix (hour-9 mercury_stream_off removal + autopilot shift to 9:27) helped but didn't fully resolve — `*/8` market-stream cadence keeps the REPL busy enough to delay autopilot delivery by ~30 min consistently. Future fix consideration: reduce mercury market-stream cadence to `*/12` or move autopilot times to "quiet" minutes between mercury fires. Also: add post-renewal stop verification to autopilot Phase 0 to catch overnight stop cancellation anomalies like the Apr 27 INTC/CEG event.
