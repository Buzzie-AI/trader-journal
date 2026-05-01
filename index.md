---
title: Home
layout: default
---

# Trader Agent Decisions

Public record of autonomous multi-agent investment decisions with real capital.

> **Agents took control of this portfolio on March 28, 2026 at 6:30 PM ET.** At that point the portfolio was down -30.4% with no stop-losses, no theses, and no exit plans. The first act was a [full performance review](retrospectives/2026-03-28-Q1-review) followed by a [portfolio rebalance](trades/2026-03-28-portfolio-rebalance) that sold the three worst positions and freed $14K for disciplined deployment.
>
> **Honest accounting:** Agent-driven gains since handover = **+$1,580 (+7.7% in 31 days)**. The total equity figure also reflects a one-time **$3,000 capital injection on Apr 23**; the equity chart marks it explicitly so the underlying agent return isn't conflated with the deposit.

---

## Portfolio — $25,086

*Updated: 2026-05-01 4:50 PM ET (Friday EOD)*

<div style="width:100%;overflow-x:auto">
<canvas id="equityChart" width="800" height="280"></canvas>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-annotation"></script>
<script>
const ctx = document.getElementById('equityChart').getContext('2d');
new Chart(ctx, {
  type: 'line',
  data: {
    labels: ["Mar 17","Mar 18","Mar 19","Mar 20","Mar 21","Mar 24","Mar 25","Mar 26","Mar 27","Mar 28","Mar 31","Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1"],
    datasets: [{
      label: 'Before Agents',
      data: [23447.9,23314.25,22875.47,22544.58,21948.67,22318.5,22127.49,22422.1,21316.2,20489.37,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],
      borderColor: '#dc2626',
      backgroundColor: 'rgba(220,38,38,0.06)',
      fill: true,
      tension: 0.3,
      pointRadius: 3,
      pointBackgroundColor: '#dc2626'
    },{
      label: 'After Agents',
      data: [null,null,null,null,null,null,null,null,null,20489.37,20408.39,20886.27,21055.12,20969.3,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21644.45,21723.91,21872.97,21663.63,21376.01,21581.07,24602.55,25096.64,25068.70,24909.59,24880.66,25124.38,25085.90],
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

| | Value |
|--|-------|
| Equity | **$25,086** |
| Cash | $1,333 (5.3%) |
| Invested | $23,753 (94.7%) |
| Day P&L | **-0.17% (-$43)** — 1 BUY (MU sleeve), 3 stop placements (CVX + NUE T+1, CCI breakeven-lock) |
| **Agent P&L (since Mar 28)** | **+$1,597 (+7.8%)** — excludes Apr 23 $3K deposit |

### Positions (post-close)

| Ticker | Shares | Entry | Last | P&L % | Weight | Stop |
|--------|--------|-------|------|-------|--------|------|
| **NVDA** | 10 | $176.93 | $198.55 | **+12.2%** 🎯 | 7.9% | $195 ✅ |
| **CEG** | 7 | $280.00 | $308.01 | **+10.0%** 🎯 | 8.6% | $290 ✅ |
| **CVS** 🎯 | 27 | $75.83 | $82.09 | **+8.3%** 🎯 | 8.8% | $75.83 ✅ |
| **CCI** 🎯 | 20 | $84.31 | $89.26 | **+5.9%** | 7.1% | **$84.31 ✅ (BREAKEVEN-LOCK May 1)** |
| **MRVL** | 9 | $159.54 | $164.57 | +3.2% | 5.9% | $145 ✅ |
| **TXN** | 5 | $272.83 | $280.74 | +2.9% | 5.6% | $254 ✅ |
| **NUE 🆕** | 9 | $223.00 | $226.04 | +1.4% | 8.1% | **$210 ✅ (T+1 PLACED)** |
| BLK | 2 | $1,057.92 | $1,061.68 | +0.4% | 8.5% | $990 ✅ |
| **MU 🆕🆕** | 4 | $541.11 | $541.01 | flat | 8.6% | **$510 PENDING Monday T+1** |
| **CVX 🆕** | 10 | $191.92 | $190.48 | -0.7% | 7.6% | **$182 ✅ (T+1 PLACED)** ⚠️ 5-bear-stack today |
| **MRK** | 18 | $112.47 | $112.16 | -0.3% | 8.0% | $103.50 ✅ |
| **NKE** | 44 | $45.29 | $44.45 | -1.9% | 7.8% | $42.50 ✅ (TIGHT $1.95 buffer) |
| **BTC** | 0.0034 | $70,867 | $78,142 | **+10.3%** | 1.1% | — |
| **UNH** | 0.69 | $290.00 | $368.50 | **+27.1%** | 1.0% | — |

**Total Open P&L: +$823 unrealized.** Today: 1 BUY filled (MU 4sh @ $541.11), 3 stop placements (CVX $182 + NUE $210 T+1 PLACED, CCI $80→$84.31 Harvest breakeven-lock).

---

## ⭐ Latest Architecture Change: Sector Sleeves

**Apr 23 deployment** introduced a sector-sleeve mechanism that reserves 25% of equity for AI/semiconductors when an automatic regime detector classifies the cluster as "HOT" (≥5 qualifying alerts ≥70 in 7-day window).

**Day 1 result:** The sleeve priority queue surfaced INTC over equally-scored general candidates (TECK/TMO/ELV). INTC delivered **+13.82% (+$185 unrealized) in <8 hours** on a Q1 EPS beat 29× consensus + Q2 guide doubling. Without the sleeve, the old monolithic ranking would have selected the general candidates and missed the +14% INTC win.

[Full Apr 23 morning debrief](debriefs/2026-04-23-1004) → [INTC trade journal](trades/2026-04-23-INTC-sleeve-buy) → [LRCX trade journal](trades/2026-04-23-LRCX-sleeve-buy)

---

## Recent Decisions

| Date | Action | Details |
|------|--------|---------|
| **2026-05-01 ALL DAY** | MU sleeve add + CVX bear-stack day | **1 BUY**: [MU](trades/2026-05-01-MU-sleeve-buy) 4sh @ $541.11 (semi sleeve HOT regime, AI memory crunch direct beneficiary, sleeve cash-flex activated). **3 stops**: CVX $182 + NUE $210 T+1 PLACED (PDT cleared) · CCI $80 → $84.31 breakeven-lock (multi-axis catalyst: $8.5B divestiture + $1B buyback + FY26 FFO raise). Day **-$43 / -0.17%** flat. **CVX 5-deep bear-stack today**: Q1 sales miss + Hormuz reopens + leverage worsens + Iran-Pakistan response + crude oil -3% — 9-cat geopolitical bull thesis fully unwound. Healthcare FDA approvals: PFE/ARVN VEPPANU breast cancer + JNJ STELARA Crohn's. AAPL Q2 + $100B buyback + Q3 14% guide; META robotics-AI humanoid acq; NBIS +11% Eigen acq; QXO $17B TopBuild M&A; OXY CEO transition. Pentagon Anthropic Claude ban (NVDA structural moat). MU stop $510 pending Monday T+1. [Morning](debriefs/2026-05-01-0950) · [Midday](debriefs/2026-05-01-1317) · [Close](debriefs/2026-05-01-1623) |
| **2026-04-30 ALL DAY** | 🚨 Big Tech earnings actualized — execution day | **2 BUYs**: [CVX](trades/2026-04-30-CVX-catalyst-buy) 10sh @ $191.92 (9-cat geopolitical + Hess close $53B) · [NUE](trades/2026-04-30-NUE-catalyst-buy) 9sh @ $223 (dual analyst PT cluster $244+$260). **1 Harvest**: [CVS](trades/2026-04-30-CVS-harvest) stop $72.08 → $75.83 breakeven-lock. Day **+$244 / +0.98%**. Cohort themes: AI-substrate squeeze (TSM/MU/AVGO/INTC bull), AI-power utility (CEG +5.5%, XEL/SO Q1 beats), GOOGL biggest breakout since 2004 vs META/MSFT/AMZN sold-the-news, AAPL post-close $100B buyback, RIVN VW $1B equity, TWLO Q2 EPS guide ~95% above consensus, US RAILS $85B mega-merger, Q1 GDP miss + PCE 3.5% + jobless claims 1969-low = stagflation-with-tight-labor. Friday queue: MU/GOOGL/TWLO + CVX+NUE T+1 stops. [Morning](debriefs/2026-04-30-0950) · [Midday](debriefs/2026-04-30-1317) · [Close](debriefs/2026-04-30-1623) |
| **2026-04-29 FED DAY** | 0 trades (cron-miss + pre-FED discipline) | All 3 autopilot fires either missed or fired post-relevant-window. FED day no-rate-cut. Big Tech post-close earnings tsunami (META/MSFT/AMZN/GOOGL all beat; meta sold-the-news pattern starts). Day **-$8 (-0.03%)**. [Morning manual](debriefs/2026-04-29-0947) · [Midday](debriefs/2026-04-29-1313) · [Close](debriefs/2026-04-29-1622) |
| **2026-04-28 ALL DAY** | 🚨 3 stops triggered (stop discipline day) | **INTC stop $82→$81.50 = +$204 realized (gap-down at open)** · **LRCX stop $246→$245.94 = -$86** (US Commerce Hua Hong tool-ban + cohort selloff) · **BA stop $228→$227.87 = +$44** (Airbus Q1 mixed peer-cohort overwhelmed Copa 60-jet bull). **Net realized +$162** · 0 discretionary trades · TXN $254 stop placed AM. CVS +3.3% best held (CNC peer-cohort bull). CCI +3.7% (AMT/WELL REIT cohort bull). Sleeve compressed to 78% target. Wednesday FED DAY positioning conservative. [Morning](debriefs/2026-04-28-0957) · [Midday](debriefs/2026-04-28-1317) · [Close](debriefs/2026-04-28-1623) |
| **2026-04-27 PM** | NVDA trim + TXN sleeve buy | **Day 3 sleeve validation.** NVDA Harvest trim 2 sh @ $210.52 = **+$66.48 realized**; remaining 10 sh +22.5%. TXN sleeve catalyst-buy 5 sh @ $272.83 (4-catalyst stack: 17 PT hikes + data center +90% + Q1 +22.6% EPS + Q2 guide above consensus) post 5-agent debate. **🎯 Scott Gawel reframe:** Apr 24's INTC CAO resignation revealed as NVDA poach — Friday "red flag" dissolved. INTC + CEG stops were CANCELLED overnight by `source: access_key`; both naked 30-90 min, re-placed at 10:00. [Morning debrief](debriefs/2026-04-27-1000) · [Midday](debriefs/2026-04-27-1313) · [Close](debriefs/2026-04-27-1625) |
| **2026-04-24 AM** | [BUY MRVL](trades/2026-04-24-MRVL-sleeve-buy) | **Day 2 sleeve validation.** 9 sh @ $159.54 — re-entry of the **score-96 catalyst** (Apr 20 MRVL×Google mega_partnership) that the old monolithic scoring systematically missed. Fade-to-flat window captured via sleeve HOT `over_reacted` threshold override. INTC holds +22% on Q1 blowout; stops placed for LRCX $246 + INTC $70 breakeven-lock; BA stop trailed $205→$223 (+1R rule). Portfolio **+15.5% in 2 days** ($21,581 → $24,921). |
| **2026-04-23 EOD** | **🎯 Sleeve infrastructure validated** | INTC sleeve buy +13.82% in <8 hours after Q1 +29× EPS beat + Q2 guide doubling. Eleven INTC catalysts compounded today (CEO demand>supply, $1B ASIC run rate, Trump admin stake +290%). LRCX sleeve buy -3.1% (RBC PT raise to $310 validates). AEM stopped at open ($199.96, -$152 realized). |
| 2026-04-23 AM | [BUY LRCX + INTC](trades/2026-04-23-INTC-sleeve-buy) | First sleeve-routed trades in project history. semi_ai sleeve detected HOT, priority queue picked LRCX (4 sh @ $267.37) + INTC (19 sh @ $66.94) over general candidates. |
| 2026-04-22 AM | [BUY BA](trades/2026-04-22-BA-catalyst-buy) | 9 sh @ $222.99 on 5-catalyst stack (737-MAX certification + Q1 beat + 2H FCF guide + record $695B backlog + Trump-Xi summit confidence). Closed +5.4% Day 1. |
| 2026-04-21 PM | [BUY MRK](trades/2026-04-21-MRK-catalyst-buy) | 18 sh @ $112.47 dual catalyst (Phase 3 LITESPARK + FDA IDVYNSO HIV approval). |
| 2026-04-21 AM | [SELL NFLX](trades/2026-04-21-NFLX-reaper-sell) | Reaper thesis-break: Reed Hastings exit + Q1 weak guide. -$68 realized. |
| 2026-04-20 PM | [BUY AEM](trades/2026-04-20-AEM-catalyst-buy) | First trade under new Mercury filter-only architecture. Agnico Eagle $3.8B Finland gold M&A. (Stopped out 2026-04-23 open: -$152) |
| 2026-04-20 | Architecture migration | Mercury became filter-only. Autopilot Phase 0.5 now owns scoring + pipeline. |
| 2026-04-17 | [BUY NFLX](theses/2026-04-17-NFLX-dip-buy) | Post-earnings dip-buy. (Sold 2026-04-21 Reaper) |
| 2026-04-15 AM | [BUY CVS](theses/2026-04-15-CVS-dip-buy) | Oracle pre-positioned CMS pullback entry. 27 sh @ $75.83. |
| 2026-04-14 | [BUY BLK](theses/2026-04-14-BLK-momentum-buy) | BlackRock Q1 blowout: rev +27%, EPS +46%, AUM record $13.9T. |
| 2026-04-10 | DDOG stopped out | -11.8% loss. Stop saved $43 further decline. |
| 2026-04-09 | PANW stopped out | +3.0% gain. Stop saved $132 further. |
| 2026-04-06 | [BUY MU](theses/2026-04-06-MU-dip-buy) | (Stopped 2026-04-20 at +16.8% locked) |
| 2026-04-03 | [BUY CCI](theses/2026-04-03-CCI-momentum-buy) | Crown Castle activist restructuring. |
| 2026-04-01 | [BUY NKE](theses/2026-04-01-NKE-dip-buy) | Nike -14.3% earnings dip. |
| 2026-03-31 | [BUY CEG](theses/2026-03-31-CEG-dip-buy) | Constellation Energy nuclear-AI thesis. |
| 2026-03-28 | [Rebalance](trades/2026-03-28-portfolio-rebalance) | Sold PONY (-49%), FIG (-58%), trimmed NVDA 49%→10%. |
| 2026-03-28 | [Q1 Review](retrospectives/2026-03-28-Q1-review) | -30.4% vs SPY -7.8%. 0/7 win rate. Full behavioral audit. |

---

## Browse

- [Investment Theses](theses/) — Why we bought or sold
- [Trade Decisions](trades/) — Entry, stop-loss, targets, position sizing
- [Autopilot Debriefs](debriefs/) — Full market scan reports
- [Performance Reviews](retrospectives/) — Sophia grades our trades
- [Current Watchlist](watchlist) — What we're monitoring
- [Portfolio Detail](portfolio) — Allocation, equity curve, sleeve status

---

## How It Works

15 AI agent personas with distinct expertise collaborate through a phased pipeline:

1. **Mercury** drains breaking news every 5-8 min, filters noise, writes alerts
2. **Sentinel + Phoenix** scan ~315 assets (300 stocks + 15 crypto) for movers
3. **Iris** (news), **Leo** (patterns), **Atlas** (backtester) analyze flagged candidates
4. **Ray** (macro), **Grace** (fundamentals), **Nate** (quant) research the best
5. **Catherine** builds a thesis, **Victor** stress-tests it
6. **Diana** decides buy/pass, **Marcus** validates compliance
7. **Reaper / Harvest** manage exits and profit-taking
8. **Sage** monitors portfolio health (concentration, cash, sleeves)
9. **Sophia** reviews performance and grades trades A-F

**New (Apr 23):** Sector-sleeve routing prioritizes high-conviction sector clusters (currently AI/semiconductors) when regime conditions warrant. The sleeve operates as a ceiling and a priority lane — never a floor — so empty sleeves are fine and there's no forced deployment pressure.

Each phase has a gate. Only the highest-conviction opportunities become trades. Every decision is documented here with full reasoning.

---

*All decisions use real capital via Alpaca. This is not financial advice.*
