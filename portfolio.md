---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-29 13:17 ET (Fri MIDDAY autopilot — equity **$31,337 (+$132 / +0.42% day)**; **2 MISSED STOPS** TXN $310 +$185.20 & CBRS $235 -$28.33 fired ~10:43 ET (BSX/MRVL pattern day 3); 3 stop ratchets **OKTA $100→$110 / MU $900→$920 / MSFT $394→$410**; net realized **+$156.87**; **OKTA +28% intraday** ($121.21) on 9 analyst raises stack; blitz day-2 +$61 net; 1/4 daily cap used (MDB 09:58 ET); no new pipeline this fire; proposing 10:30 ET autopilot at close to fix mid-morning blind spot)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$31,337** (Fri midday intraday) |
| Cash | **$12,535.83** (40.0%) |
| Invested | $18,801.17 (60.0%) across **22 equity positions** |
| Today's activity | **3 RATCHETS + 1 BUY (MDB AM) + 2 stop fires + 0 new pipeline** |
| Realized today | **+$156.87** (TXN +$185.20, CBRS -$28.33) |
| Day P&L | **+$132 / +0.42%** vs Thu $31,204.52 |
| Week-to-date | Strong: equity holding +$130+ ground after week of AI blitz |
| 🚀 Friday intraday winners | OKTA +28.0% / MSFT +3.9% / MU +3.9% / AVGO +3.0% / BLK +1.1% / NVDA +1.2% / DXCM +1.7% / GE +1.3% |
| 🔧 Friday ratchets | OKTA $100→$110 (locks $105 floor) / MU $900→$920 (above entry) / MSFT $394→$410 (near breakeven) |
| 🏆 Lifecycle highs | OKTA +35.7% / UNH +30.9% / CVS +20.3% / GE +13.6% / DXCM +13.4% / NUE +12.1% / CCI +7.8% |
| 📊 AI Blitz Day 2 | NVDA +1.97% / MU +5.53% / AVGO +4.53% / TSM +0.83% / CBRS exited; **+$61 net** (89 unrealized − 28 realized) |
| 🎯 Pipeline candidates | None pipelined; AMAT priced (+0.22% only), INTC fading, META has Reuters bear catalyst, MOD post-catalyst-day |
| ⚠️ BSX pattern recurrence | **3 consecutive sessions** missed stops fire ~10:30-10:47 ET window |

---

## Equity Curve (Apr 1 → May 29 intraday)

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23 (+$3K deposit)","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12","May 13","May 14 (+$5K deposit)","May 15","May 18","May 19","May 20","May 21","May 22","May 26","May 27","May 28","May 29 midday"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26439.85,26735.75,31124.35,30878.74,31100.67,30890.49,31059.40,30992.43,31273.88,31048.78,31155.80,31204.52,31337.00],
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

**Fri May 29 midday:** $31,337 (+$132 / +0.42% vs Thu $31,204.52). Story: OKTA ripping +28% intraday on 9-analyst raise stack pays for MDB sold-the-news drift + CVS pullback. 2 missed stops at 10:43 ET (BSX pattern day 3) — TXN profit-take +$185 partially offset by CBRS exit -$28. Stop ratchet trio executed on momentum positions.

---

## Current Positions (22 equity + BTCUSD + CVR, Fri 5/29 midday intraday)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer | Notes |
|--------|--------|-------|------|-----|-------|------|--------|-------|
| **OKTA** 🚀🚀🚀 | 5 | $89.36 | **$121.21** | **+$160** | **+35.7%** | **$110 ↑ (locks $105 floor)** | 9.3% | 9 analyst raises today; bull avg $120.13 |
| **UNH** 🏆 | 0.69 | $290.00 | $379.50 | +$62 | **+30.9%** | n/a | n/a | All-time win frac |
| **CVS** 🏆 | 27 | $75.83 | $91.19 | +$415 | **+20.3%** | $87 | 4.6% | Zepbound + CRM AI fading; tight |
| **GE** | 2 | $285.99 | $324.99 | +$78 | **+13.6%** | $263 | 19.1% | Steady industrial |
| **DXCM** | 4 | $64.85 | $73.55 | +$35 | **+13.4%** | $66 | 10.3% | Glucose tech momentum |
| **NUE** | 9 | $223.00 | $250.08 | +$244 | **+12.1%** | $210 | 16.0% | Steel rally intact |
| **CCI** | 20 | $84.31 | $90.88 | +$131 | **+7.8%** | $84.31 (breakeven) | 7.2% | Tower REIT |
| **MSFT** 🚀🔧 | 1 | $415.53 | $443.79 | +$28 | **+6.8%** | **$410 ↑ (near breakeven)** | 7.6% | 3-catalyst run; ratchet today |
| **MU** 🚀🔧 | 1 | $908.44 | $958.62 | +$50 | **+5.5%** | **$920 ↑ (above entry)** | 4.0% | Mizuho $1150 paying through |
| **MRK** 🚀 | 18 | $112.47 | $118.82 | +$114 | **+5.6%** | $117 | 1.5% | TIGHT — Calderasib breakthrough |
| **BA** | 3 | $220.33 | $231.03 | +$32 | **+4.9%** | $202 | 12.6% | Solid recovery |
| **AVGO** 🚀🆕 | 1 | $420.33 | $439.37 | +$19 | **+4.5%** | $395 | 10.1% | Day 2 blitz; Susquehanna $490 |
| **BLK** | 2 | $1,057.92 | $1,058.16 | +$0 | +0.02% | $990 | 6.4% | Steady recovery; was -2% mid-week |
| **NVDA** 🆕 | 4 | $212.69 | $216.89 | +$17 | **+1.97%** | $190 | 12.4% | Day 2 blitz; +28% / cumulative |
| **TSM** 🆕 | 1 | $416.43 | $419.89 | +$3 | +0.83% | $390 | 7.1% | Day 2 blitz; foundry leverage |
| **CSCO** | 1 | $117.34 | $119.75 | +$2 | +2.05% | $108 | 9.8% | Steady |
| **SYY** | 5 | $73.21 | $75.45 | +$11 | +3.05% | $72 | 4.6% | Stable |
| **MDB** 🆕 | 1 | $317.56 | $312.95 | -$5 | -1.45% | $290 | 7.3% | Fresh AM buy; SOLD THE NEWS day |
| **D** | 4 | $68.82 | $66.86 | -$8 | -2.85% | $62.33 | 6.8% | Utility drift |
| **TJX** | 4 | $159.00 | $154.36 | -$19 | -2.92% | $146 | 5.4% | Soft consumer |
| **NFLX** | 5 | $91.12 | $85.99 | -$26 | -5.6% | $84 | 2.3% | TIGHT; continuing slow drift |
| **BTCUSD** | 0.0034 | $70,867 | $74,183 | +$11 | +4.7% | n/a | n/a | Frozen position |
| **737CVR019** | 4.06 | $0 | n/a | — | — | n/a | n/a | CVR |

---

## Today's Stop Fires (2)

| Time | Ticker | Stop | Fill | Realized | Notes |
|------|--------|------|------|----------|-------|
| 10:42 ET | CBRS | $235 | $235 (clean) | **-$28.33** | Day-2 blitz volatility; 1 sh small bet |
| 10:43 ET | TXN | $310 | $309.87 | **+$185.20** | Trend exhaustion exit; +13.6% lifecycle gain locked |
| **NET** | | | | **+$156.87** | Both missed in AM autopilot (10-day pattern) |

## Today's Stop Ratchets (3)

| Ticker | Old | New | Trigger | Floor Locked |
|--------|-----|-----|---------|--------------|
| OKTA | $100 | **$110** | 9 analyst raises today; bull avg $120.13 | $11/sh × 5 = $105 |
| MU | $900 | **$920** | Mizuho $1150 paying through +5.5% day | $11.56/sh above entry |
| MSFT | $394.09 | **$410** | 3-catalyst run + 6.8% lifecycle | $5.53/sh max loss capped |

## Today's Buys (1)

| Time | Ticker | Qty | Filled | Limit | Slippage |
|------|--------|-----|--------|-------|----------|
| 09:58 | MDB | 1 | $317.56 | $320 | $2.44 favorable |

---

## Open Stop-Loss Orders (21 active GTC + MDB just placed)

All equity positions except UNH (frac) and BTCUSD (crypto) and the CVR have GTC stops in place. Updated stops as of midday:

| Ticker | Qty | Stop |
|--------|-----|------|
| **OKTA** | 5 | **$110** ↑ |
| **MU** | 1 | **$920** ↑ |
| **MSFT** | 1 | **$410** ↑ |
| **MRK** | 18 | $117 (AM ratchet) |
| MDB | 1 | $290 |
| NVDA | 4 | $190 |
| AVGO | 1 | $395 |
| TSM | 1 | $390 |
| CVS | 27 | $87 |
| CCI | 20 | $84.31 (breakeven) |
| GE | 2 | $263 |
| DXCM | 4 | $66 |
| NUE | 9 | $210 |
| BLK | 2 | $990 |
| BA | 3 | $202 |
| CSCO | 1 | $108 |
| SYY | 5 | $72 |
| TJX | 4 | $146 |
| NFLX | 5 | $84 |
| D | 4 | $62.33 |

(TXN $310 and CBRS $235 stops both filled this AM — see "Stop Fires" above.)

---

## Sector Allocation (intraday)

| Sleeve | Members | Value | % of Portfolio |
|--------|---------|-------|----------------|
| **semi_ai** | NVDA + MU + AVGO + TSM | $2,686 | 8.6% |
| **hyperscaler+sw** | MSFT + MDB + OKTA + CSCO | $1,483 | 4.7% |
| Healthcare | UNH + CVS + DXCM + MRK | $5,157 | 16.5% |
| Industrials | BA + GE + NUE | $3,594 | 11.5% |
| Financials | BLK | $2,116 | 6.8% |
| Cyber (held) | OKTA included above | — | — |
| Consumer | TJX + SYY + NFLX | $1,425 | 4.5% |
| REITs | CCI | $1,818 | 5.8% |
| Utility | D | $267 | 0.9% |
| Crypto (frozen) | BTCUSD | $256 | 0.8% |
| CVR | 737CVR019 | nominal | — |
| **Cash** | — | $12,536 | **40.0%** |

Total AI-direct exposure: ~$4,400 = **14.0% of book** (up from 4.3% pre-blitz; sleeve fill ~47% of target).

---

## Mid-Morning Stop Fire Pattern — 3 Sessions in a Row

| Date | Ticker(s) | AM autopilot | Stop fire | Lag |
|------|-----------|--------------|-----------|-----|
| 5/27 | BSX | 09:57 | ~10:30 | ~33 min |
| 5/28 | MRVL | 09:57 | 10:47 | ~50 min |
| **5/29** | **TXN + CBRS** | **09:57** | **10:42-43** | **~46 min** |

**Proposing:** add `autopilot_midmorning` cron at 10:30 ET weekdays to catch this window. Decision deferred to operator at close debrief.
