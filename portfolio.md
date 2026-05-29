---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-29 16:23 ET (Fri CLOSE / WEEK WRAP — equity **$31,348.61 (+$144 / +0.46% day; +$300 / +0.96% week)**; **OKTA BREAKOUT +30.0% on day** ($94.72→$123.16) with **11 ANALYST RAISES** (bull avg $120.78); MDB recovered from -1.5% midday to +5.0% close on Citi $455 + 5 other raises; MSFT +5.1% on OpenAI IPO bank lineup news (5th catalyst week); **2 missed stops fired ~10:43 ET** (TXN +$185.20 / CBRS -$28.33 = net **+$156.87 realized**); **8 stop ratchets across day** locking momentum gains; AI blitz day-2 **+$54.22 / +1.90%** on $2,859 deployed (MU +6.2% runner pays for CBRS -10.8% exit); 1/4 daily cap used (MDB AM only); 3 sessions of mid-morning stop fires observed — **proposing 10:30 ET autopilot cron** to operator)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$31,348.61 EOD** (Fri close) |
| Cash | **$12,535.83** (40.0%) |
| Invested | $18,812.78 (60.0%) across **22 equity positions** |
| Today's activity | **1 BUY (MDB) + 8 RATCHETS + 2 stop fires** |
| Realized today | **+$156.87** (TXN +$185.20 / CBRS -$28.33) |
| Day P&L | **+$144 / +0.46%** vs Thu $31,204.52 |
| Week P&L | **+$300 / +0.96%** (3 sessions Wed-Fri) |
| Week realized | **+$66.55** (net of ZS -$132.57 slippage) |
| 🚀 Friday winners (held) | OKTA +30.0% / MSFT +5.1% / MU +4.5% / AVGO +4.2% / MDB +5.0% / DXCM +1.9% / GE +1.1% / CSCO +1.8% / CCI +0.5% / BA +1.0% |
| 🔧 Friday ratchets (8 total) | OKTA $89→$100→$110→$115 / MU $850→$900→$920 / MRK $115→$117 / MSFT $394→$410 / AVGO $395→$410 |
| 🏆 Lifecycle highs | OKTA **+37.8%** / UNH +31.1% / CVS +20.0% / DXCM +13.6% / GE +13.4% / NUE +12.1% / CCI +8.5% / MSFT +7.9% / MU +6.2% / MRK +5.6% / AVGO +5.8% / MDB +5.0% |
| 📊 AI Blitz 48hr | NVDA -0.09% / **MU +6.23%** / **AVGO +5.78%** / TSM +0.60% / CBRS exited; **NET +$54.22 / +1.90%** on $2,859 |
| 🎯 Mon 6/1 pipeline | MDB add (if <$345) / CRWD (cyber 2nd) / AMAT (re-test $440) / INTC fresh catalyst needed |
| ⚠️ Mid-morning stop pattern | **3 consecutive sessions** — proposing autopilot_midmorning 10:30 ET cron |

---

## Equity Curve (Apr 1 → May 29 close)

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23 (+$3K deposit)","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12","May 13","May 14 (+$5K deposit)","May 15","May 18","May 19","May 20","May 21","May 22","May 26","May 27","May 28","May 29"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26439.85,26735.75,31124.35,30878.74,31100.67,30890.49,31059.40,30992.43,31273.88,31048.78,31155.80,31204.52,31348.61],
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

**Fri May 29 close:** $31,348.61 (+$144 / +0.46% day; +$300 / +0.96% 3-session week). **Story of the week:** OKTA breakout +37.8% lifecycle as 11 analyst raises Friday alone confirm the bull stack. AI blitz 48hr validated +1.90%. Mid-morning stop fire pattern documented for operator decision.

---

## Current Positions (22 equity + BTCUSD + CVR, EOD Fri 5/29 CLOSE)

| Ticker | Shares | Entry | Close | Day % | Lifecycle | Stop | Buffer | Notes |
|--------|--------|-------|-------|-------|-----------|------|--------|-------|
| **OKTA** 🚀🚀🚀 | 5 | $89.36 | **$123.16** | **+30.0%** | **+37.8%** | **$115 ↑↑↑** | 6.6% | **11 analyst raises today**; bull avg $120.78 |
| MSFT 🚀 | 1 | $415.53 | $448.56 | +5.05% | +7.95% | **$410 ↑** | 8.6% | OpenAI IPO bank lineup (5th catalyst wk) |
| MU 🚀 | 1 | $908.44 | $965.00 | +4.49% | +6.22% | **$920 ↑** | 4.7% | DELL surge + Mizuho $1150 |
| AVGO 🆕🚀 | 1 | $420.33 | $444.61 | +4.23% | +5.78% | **$410 ↑** | 7.8% | Susquehanna $490 |
| MDB 🆕 | 1 | $317.56 | $333.58 | +2.43% | +5.04% | $290 | 12.9% | Citi $455 + 5 raises (avg $418) |
| NVDA 🆕 | 4 | $212.69 | $212.49 | -0.82% | -0.09% | $190 | 10.6% | Day 2 flat |
| TSM 🆕 | 1 | $416.43 | $418.94 | -1.39% | +0.60% | $390 | 6.9% | Foundry leverage |
| **UNH** 🏆 | 0.69 | $290.00 | $380.31 | -0.58% | **+31.1%** | — | n/a | All-time win |
| **CVS** 🏆 | 27 | $75.83 | $90.98 | -2.14% | **+20.0%** | $87 | 4.4% | Cushion eroding |
| **GE** | 2 | $285.99 | $324.25 | +1.07% | **+13.4%** | $263 | 18.9% | Industrial |
| **DXCM** | 4 | $64.85 | $73.69 | +1.87% | **+13.6%** | $66 | 10.4% | Glucose momentum |
| **NUE** | 9 | $223.00 | $250.00 | +0.28% | **+12.1%** | $210 | 16.0% | Steel rally |
| **CCI** | 20 | $84.31 | $91.50 | +0.45% | +8.5% | $84.31 | 7.9% | REIT breakeven |
| **MRK** | 18 | $112.47 | $118.72 | -0.98% | +5.6% | **$117 ↑** | 1.4% TIGHT | Calderasib mod |
| **BA** | 3 | $220.33 | $231.00 | +0.97% | +4.9% | $202 | 12.5% | Solid |
| **CSCO** | 1 | $117.34 | $120.80 | +1.82% | +2.9% | $108 | 10.6% | Steady |
| **SYY** | 5 | $73.21 | $75.81 | -0.14% | +3.5% | $72 | 5.0% | Stable |
| **BLK** | 2 | $1,057.92 | $1,046.88 | +0.04% | -1.0% | $990 | 5.4% | Range |
| **D** | 4 | $68.82 | $66.94 | -0.65% | -2.7% | $62.33 | 6.9% | Utility |
| **TJX** | 4 | $159.00 | $154.75 | -0.09% | -2.7% | $146 | 5.6% | Soft |
| **NFLX** | 5 | $91.12 | $86.04 | -0.37% | -5.6% | $84 | 2.4% TIGHT | Drift |
| **BTCUSD** | 0.0034 | $70,867 | $73,564 | +0.08% | +3.8% | n/a | n/a | Frozen |
| **737CVR019** | 4.06 | $0 | n/a | — | — | n/a | n/a | CVR |

---

## Today's Stop Fires (2 — both missed AM audit ~10:43 ET)

| Time | Ticker | Stop | Fill | Realized | Notes |
|------|--------|------|------|----------|-------|
| 10:42 ET | CBRS | $235 | $235 (clean) | **-$28.33** | Day-2 blitz volatility; small bet |
| 10:43 ET | TXN | $310 | $309.87 (-13¢) | **+$185.20** | Trend exhaustion; +13.6% lifecycle locked |
| **NET** | | | | **+$156.87** | BSX/MRVL pattern day 3 |

## Today's Stop Ratchets (8 across day — locking momentum gains)

| Time | Ticker | Old | New | Notes |
|------|--------|-----|-----|-------|
| 09:58 AM | OKTA | $89 | $100 | AM phase 5-analyst raise stack |
| 09:58 AM | MU | $850 | $900 | Mizuho $1150 paying |
| 09:58 AM | MRK | $115 | $117 | Calderasib breakthrough |
| 13:19 mid | OKTA | $100 | $110 | 9 raises confirmed |
| 13:19 mid | MU | $900 | $920 | Above-entry breakeven+ |
| 13:19 mid | MSFT | $394 | $410 | 6.8% lifecycle lock |
| **16:23 close** | **OKTA** | $110 | **$115** | **11 raises avg $120.78; locks $130 floor** |
| 16:23 close | AVGO | $395 | $410 | 5.8% lifecycle lock |

## Today's Buys (1 — daily cap)

| Time | Ticker | Qty | Filled | Limit | Slippage |
|------|--------|-----|--------|-------|----------|
| 09:58 | MDB | 1 | $317.56 | $320 | $2.44 favorable |

---

## Open Stop-Loss Orders (22 active GTC at close)

| Ticker | Qty | Stop | Cushion |
|--------|-----|------|---------|
| **OKTA** | 5 | **$115** ↑↑↑ | 6.6% |
| **MU** | 1 | **$920** ↑ | 4.7% |
| **MSFT** | 1 | **$410** ↑ | 8.6% |
| **AVGO** | 1 | **$410** ↑ | 7.8% |
| **MRK** | 18 | **$117** ↑ | 1.4% TIGHT |
| MDB | 1 | $290 | 12.9% |
| NVDA | 4 | $190 | 10.6% |
| TSM | 1 | $390 | 6.9% |
| CVS | 27 | $87 | 4.4% |
| CCI | 20 | $84.31 | 7.9% |
| GE | 2 | $263 | 18.9% |
| DXCM | 4 | $66 | 10.4% |
| NUE | 9 | $210 | 16.0% |
| BLK | 2 | $990 | 5.4% |
| BA | 3 | $202 | 12.5% |
| CSCO | 1 | $108 | 10.6% |
| SYY | 5 | $72 | 5.0% |
| TJX | 4 | $146 | 5.6% |
| NFLX | 5 | $84 | 2.4% TIGHT |
| D | 4 | $62.33 | 6.9% |

---

## Week Trajectory (Wed 5/27 → Fri 5/29)

| Date | Close | Day $ | Cum Week |
|------|-------|-------|----------|
| Tue 5/26 EOD | $31,048.78 | — | start |
| Wed 5/27 | $31,155.80 | +$107 | +0.34% |
| Thu 5/28 | $31,204.52 | +$48.72 | +0.50% |
| **Fri 5/29** | **$31,348.61** | **+$144.09** | **+0.96%** |

3-session week: **+$300 total / +0.96%** | Net realized: **+$66.55** (despite ZS -$132.57 slippage)

---

## Sector Allocation (EOD close)

| Sleeve | Members | Value | % |
|--------|---------|-------|---|
| **semi_ai** | NVDA + MU + AVGO + TSM | $2,678 | 8.5% |
| **hyperscaler+sw** | MSFT + MDB + OKTA + CSCO | $1,519 | 4.8% |
| Healthcare | UNH + CVS + DXCM + MRK | $5,150 | 16.4% |
| Industrials | BA + GE + NUE | $3,591 | 11.5% |
| Financials | BLK | $2,094 | 6.7% |
| Consumer | TJX + SYY + NFLX | $1,428 | 4.6% |
| REITs | CCI | $1,830 | 5.8% |
| Utility | D | $268 | 0.9% |
| Crypto (frozen) | BTCUSD | $254 | 0.8% |
| CVR | 737CVR019 | nominal | — |
| **Cash** | — | **$12,536** | **40.0%** |

**Direct AI exposure:** ~$4,200 = **13.4%** of book (up from 4.3% pre-blitz Wed).

---

## Mid-Morning Stop Fire Pattern — 3 Sessions

| Date | Ticker(s) | AM autopilot | Stop fire | Lag |
|------|-----------|--------------|-----------|-----|
| 5/27 | BSX | 09:57 | ~10:30 | ~33 min |
| 5/28 | MRVL | 09:57 | 10:47 | ~50 min |
| **5/29** | **TXN + CBRS** | **09:57** | **10:42-43** | **~46 min** |

**Cumulative cost: ~$50 over 3 sessions.** Will propose `autopilot_midmorning` cron at 10:30 ET to operator.

---

## Monday 6/1 Setup

**Priority pipeline:**
1. MDB add (if opens <$345 — bull stack avg $418 vs $317 entry)
2. CRWD (Jefferies $775; cyber sleeve 2nd to OKTA)
3. AMAT (re-test entry at $440 if pulls back)

**Tight stop watch:**
- MRK $117 (1.4% cushion — likely fires Mon)
- NFLX $84 (2.4%)
- CVS $87 (4.4% deteriorating)
