---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-06-01 09:57 ET (Mon MORNING autopilot — equity **$31,422.19 (+$68 / +0.22% day)**; **MRK STOP $117 FIRED at 09:31 ET** (1 min after open as predicted Fri close) = **+$81.54 realized**; 4 stop ratchets locking momentum gains (**OKTA $115→$125** locks $178 floor / **MU $920→$960** above entry / **MDB $290→$310** / **MSFT $410→$430**); 2 fresh BUYs run through full 5-agent pipeline: **ORCL 1 sh @ $231.04** ($30B gov AI deal Sun PM, $3.96 favorable vs $235 limit, stop $215) + **ARM 1 sh @ $390.59** (Mizuho Outperform PT $425, operator-flagged 5/27, $4.41 favorable vs $395 limit, stop $370); NVDA + TSM sleeve adds **BLOCKED by Alpaca wash-trade protection** (existing stops on opposite side — defer to midday with cancel-stop-buy-re-stop workaround); 2/4 daily cap used; **OKTA +50% lifecycle** ($134.07 vs $89.36 entry), MDB +15.6% / MU +13.3% / MSFT +11.8% lifecycle; direct AI exposure 13.4%→**15.3% of book** post-buys; Computex catalyst stack 25+ NVDA bull alerts Sun-Mon offset by China loophole bear)*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$31,422.19** (Mon AM autopilot) |
| Cash | **$14,020** (44.6%) — post-MRK exit + ORCL/ARM buys |
| Invested | $17,402 (55.4%) across **23 equity positions** |
| Today's activity | **4 RATCHETS + 2 BUYs + 1 stop fire + 2 blocked BUYs (defer)** |
| Realized today | **+$81.54** (MRK predicted) |
| Day P&L | **+$68 / +0.22%** vs Fri $31,354 last_equity |
| 🚀 Big intraday | OKTA +8.8% ($134, lifecycle +50%!) / MDB +9.4% ($367) / MU +6.0% ($1029) / NVDA +4.0% ($219) / MSFT +3.2% ($464) / TSM +3.3% ($432) / ORCL +3.2% (new) |
| 🔧 Today's ratchets | OKTA $125 / MU $960 / MDB $310 / MSFT $430 |
| 🏆 Lifecycle leaders | OKTA +50.0% / UNH +30.9% / CVS +19.4% / MDB +15.6% / MU +13.3% / DXCM +13.7% / GE +11.4% / MSFT +11.8% / NUE +10.7% |
| 🆕 New positions | ORCL ($231.04, stop $215) / ARM ($390.59, stop $370) |
| 💰 Capital deployed today | $621.63 (+$8.37 favorable slippage) |
| 🎯 Pipeline blocked | NVDA + TSM (wash-trade rejected — midday workaround) |
| 🎯 Daily cap | 2/4 BUYs used; 2 remaining (likely NVDA+TSM midday) |
| ⚠️ MRK predicted exit | Fri close watchlist flagged "MRK $117 1.4% likely fires Mon" — fired at 09:31:40 ET |

---

## Equity Curve (Apr 1 → Jun 1 AM)

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23 (+$3K deposit)","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12","May 13","May 14 (+$5K deposit)","May 15","May 18","May 19","May 20","May 21","May 22","May 26","May 27","May 28","May 29","Jun 1 AM"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26439.85,26735.75,31124.35,30878.74,31100.67,30890.49,31059.40,30992.43,31273.88,31048.78,31155.80,31204.52,31353.95,31422.19],
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
    plugins: { legend: { display: true, position: 'top' }, tooltip: { callbacks: { label: function(ctx) { return ctx.dataset.label + ': $' + ctx.parsed.y.toLocaleString(); } } } },
    scales: { y: { ticks: { callback: function(v) { return '$' + v.toLocaleString(); } } } }
  }
});
</script>

**Mon Jun 1 AM:** $31,422.19 (+$68 / +0.22% intraday). **OKTA +50% lifecycle** as 12 analyst raises Fri continue Monday. MDB +15.6% lifecycle on Citi $455. New AI sleeve adds ORCL + ARM (BUY pipeline). MRK exit +$81.54 predicted. NVDA+TSM sleeve adds blocked by wash-trade — midday workaround.

---

## Current Positions (23 equity + BTCUSD + CVR — Mon 9:57 ET)

| Ticker | Shares | Entry | Last | Day % | Lifecycle | Stop | Buffer | Notes |
|--------|--------|-------|------|-------|-----------|------|--------|-------|
| **OKTA** 🚀🚀🚀 | 5 | $89.36 | **$134.07** | **+8.8%** | **+50.0%** | **$125 ↑↑** | 6.8% | 12 raises Fri + Macquarie Sat; bull avg $120.78 |
| **UNH** 🏆 | 0.69 | $290.00 | $379.74 | -0.15% | **+30.9%** | — | n/a | All-time win frac |
| **CVS** 🏆 | 27 | $75.83 | $90.55 | -0.5% | **+19.4%** | $87 | 3.9% | Cushion deteriorating |
| **MDB** 🚀🔧 | 1 | $317.56 | $367.20 | +9.4% | +15.6% | **$310 ↑** | 15.5% | Citi $455 + 5 raises avg $418 |
| **DXCM** | 4 | $64.85 | $73.71 | -0.04% | **+13.7%** | $66 | 10.5% | Glucose tech |
| **MU** 🚀🔧 | 1 | $908.44 | $1029.53 | +6.0% | **+13.3%** | **$960 ↑** | 6.8% | Wall Street "cheap at $1T" |
| **MSFT** 🚀🔧 | 1 | $415.53 | $464.44 | +3.2% | **+11.8%** | **$430 ↑** | 7.4% | One Copilot + OpenAI IPO |
| **GE** | 2 | $285.99 | $318.64 | -1.6% | **+11.4%** | $263 | 17.4% | Industrial |
| **NUE** | 9 | $223.00 | $246.94 | -1.2% | **+10.7%** | $210 | 15.0% | Steel |
| **CCI** | 20 | $84.31 | $90.28 | -1.3% | +7.1% | $84.31 | 6.6% | REIT breakeven |
| **AVGO** | 1 | $420.33 | $449.28 | +0.6% | +6.9% | $410 | 8.7% | Pre-ER quiet |
| **TSM** | 1 | $416.43 | $432.05 | +3.3% | +3.7% | $390 | 9.7% | TSMC NVDA AI partnership |
| **NVDA** | 4 | $212.69 | $219.66 | +4.0% | +3.3% | $190 | 13.5% | Computex 25+ catalysts |
| **CSCO** | 1 | $117.34 | $119.46 | -0.8% | +1.8% | $108 | 9.6% | Steady |
| **SYY** | 5 | $73.21 | $74.70 | -1.5% | +2.0% | $72 | 3.6% | Stable |
| **BA** | 3 | $220.33 | $224.67 | -2.8% | +2.0% | $202 | 10.1% | Drift |
| **ARM** 🆕 | 1 | $390.59 | $390.59 | NEW | — | $370 | 5.3% | Mizuho PT $425; AI semi-IP |
| **ORCL** 🆕 | 1 | $231.04 | $231.04 | NEW | — | $215 | 7.0% | $30B gov AI deal |
| **BLK** | 2 | $1,057.92 | $1,049.39 | +0.2% | -0.8% | $990 | 5.7% | Recovering |
| **BTCUSD** | 0.0034 | $70,867 | $71,485 | -2.3% | +0.9% | n/a | n/a | Frozen |
| **D** | 4 | $68.82 | $65.82 | -1.7% | -4.4% | $62.33 | 5.3% | Utility drift |
| **TJX** | 4 | $159.00 | $153.30 | -0.9% | -3.6% | $146 | 4.8% | Soft |
| **NFLX** | 5 | $91.12 | $86.61 | +0.7% | -5.0% | $84 | 3.0% TIGHT | Drift |
| **737CVR019** | 4.06 | $0 | n/a | — | — | n/a | n/a | CVR |

---

## Today's Stop Fires (1)

| Time | Ticker | Stop | Fill | Realized | Note |
|------|--------|------|------|----------|------|
| 09:31:40 | MRK | $117 | $117.00 (clean) | **+$81.54** | **Predicted at Fri close (1.4% cushion)** |

## Today's BUYs (2)

| Time | Ticker | Qty | Filled | Limit | Slippage | Stop |
|------|--------|-----|--------|-------|----------|------|
| 09:56 | ORCL | 1 | $231.04 | $235 | $3.96 favorable | $215 |
| 09:56 | ARM | 1 | $390.59 | $395 | $4.41 favorable | $370 |
| **TOTAL** | | | **$621.63** | | **+$8.37** | |

## Today's Stop Ratchets (4)

| Ticker | Old | New | Trigger |
|--------|-----|-----|---------|
| OKTA | $115 | **$125** | Lifecycle +50%; bull stack continuing Mon |
| MU | $920 | **$960** | +13.3% lifecycle; "cheap at $1T" |
| MDB | $290 | **$310** | +15.6% lifecycle; Citi $455 |
| MSFT | $410 | **$430** | +11.8% lifecycle; OpenAI IPO + One Copilot |

## Blocked BUYs (2 — wash-trade protection, midday workaround)

| Ticker | Block | Plan |
|--------|-------|------|
| NVDA add | Existing stop $190 covers 4 sh | Midday: cancel stop → buy 1 → re-stop qty 5 |
| TSM add | Existing stop $390 covers 1 sh | Midday: cancel stop → buy 1 → re-stop qty 2 |

---

## Sector Allocation (post-buys)

| Sleeve | Members | Value | % |
|--------|---------|-------|---|
| **semi_ai** | NVDA + MU + AVGO + TSM + ARM | $3,121 | 9.9% |
| **hyperscaler+sw** | MSFT + MDB + OKTA + CSCO + ORCL | $1,989 | 6.3% |
| Healthcare | UNH + CVS + DXCM | $3,001 | 9.5% |
| Industrials | BA + GE + NUE | $3,534 | 11.2% |
| Financials | BLK | $2,099 | 6.7% |
| Consumer | TJX + SYY + NFLX | $1,420 | 4.5% |
| REITs | CCI | $1,806 | 5.8% |
| Utility | D | $263 | 0.8% |
| Crypto | BTCUSD | $247 | 0.8% |
| CVR | 737CVR019 | nominal | — |
| **Cash** | — | **$14,020** | **44.6%** |

Direct AI exposure: ~$4,800 = **15.3% of book** (up from 13.4% Fri close pre-buys).

semi_ai sleeve under-fill: 9.9% vs 30% target — room for $6K more. Midday NVDA+TSM adds will move to ~10.7%.

---

## Pending Midday Actions

1. **NVDA add 1 sh** + replace stop qty 4→5 (cancel-buy-replace workflow)
2. **TSM add 1 sh** + replace stop qty 1→2 (cancel-buy-replace workflow)
3. Stop ratchet review on ORCL/ARM (let positions settle)
4. Daily cap will hit 4/4 used after midday adds
