---
title: Portfolio
layout: default
---

# Portfolio Snapshot

*Last updated: 2026-05-20 16:25 ET (Wed EOD CLOSE — **5 actions / 0 realized / equity $31,059 (+$169 / +0.55%)**). **Day story = TAPE-CONFIRMING DISCIPLINE THROUGH NVDA EARNINGS**: AM 3 BUYs (MRVL/TJX/BA re-entry, $2,243 spend) selected by catalyst+tape alignment; PASSED on top-scored MU (-2.6%) and TGT (-7.7% sell-the-news despite beat-and-raise). Midday CRWD ratchet $600→$620 (+$10.52 above entry on 11-leg sell-side cluster + ATH $646). MSFT add on OpenAI $1T IPO blocked by wash trade. Close: 2 RATCHETS (DXCM $60→$66 / TXN $285→$293 locks +$100.88). **NVDA Q1 BEAT $1.87/$81.6B/+139% YoY EPS BUT AH selling -2.3% sell-the-news (4th AMAT lesson reapplied today)**. 4th cap slot HELD RESERVED for Thu tape-confirm.*

## Account Summary

| Metric | Value |
|--------|-------|
| **Portfolio Value** | **$31,059.40 EOD** (Wed close) |
| Cash | **$9,102** (29.3%) — ample dry powder |
| Invested | $21,957 (70.7%) across **25 equity positions** |
| Positions | **25 equity** (+MRVL/TJX/BA AM = full deck) + BTC + UNH frac + CVR |
| Today's activity | **5 actions: 3 BUYs (AM) + 2 RATCHETS (Close) + 1 MIDDAY RATCHET** |
| Realized today | **$0** (no stops fired) |
| Day P&L | **+$169 / +0.55%** vs SPX/Nasdaq mixed |
| 🚫 Saved by Tape-Confirming PASS | MU sell-the-news -2.6% AM / TGT BEAT-AND-RAISE rejected -7.7% / NVDA AH -2.3% sell-the-news despite +139% YoY EPS |
| 🔧 Ratchets locked today | CRWD $600→$620 (+$10.52 above entry) · DXCM $60→$66 (+$4.60) · TXN $285→$293 (+$100.88 lock) |
| 🔥 CRWD compounding | **11 sell-side legs over 5 days** + ATH break $646.62; **+6.3% lifecycle, AH close $650.34** |
| 🔥 NVDA Q1 print | EPS $1.87 vs $1.76 (+6.25%) / Sales $81.62B vs $78.80B / **+139.74% YoY EPS** — BUT AH tape -2.3% |
| 🚨 Thu open watch | MRVL chip-cluster reaction to NVDA AH / NFLX 5.0% cushion / WBD $30B LBO bond signal AH |

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
    labels: ["Apr 1","Apr 2","Apr 3","Apr 6","Apr 7","Apr 8","Apr 9","Apr 10","Apr 13","Apr 14","Apr 15","Apr 16","Apr 17","Apr 20","Apr 21","Apr 22","Apr 23 (+$3K deposit)","Apr 24","Apr 27","Apr 28","Apr 29","Apr 30","May 1","May 4","May 5","May 6","May 7","May 8","May 11","May 12","May 13","May 14 (+$5K deposit)","May 15","May 18","May 19 EOD","May 20 EOD"],
    datasets: [{
      label: 'Equity',
      data: [20886.27,21055.12,20969.30,20958.95,20991.67,21341.87,21247.72,21213.72,21327.63,21679.31,21654.58,21723.91,21872.97,21653.15,21376.01,21581.07,24602.55,25096.64,25080.73,24887.84,24880.66,25129.32,25093.43,25259.53,25699.52,26167.40,25767.88,26455.49,26575.95,26439.85,26735.75,31124.35,30878.74,31100.67,30890.49,31059.40],
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

**Wed May 20 EOD:** $31,059.40 (+$169 / +0.55% vs Tue close $30,890.49). Day featured 3 tape-confirming BUYs (MRVL/TJX/BA re-entry) + 3 ratchets (CRWD midday $620 / DXCM close $66 / TXN close $293). **NVDA Q1 mega-beat BUT AH selling -2.3% = AMAT/MU/TGT sell-the-news pattern reapplied** — 4th cap slot held reserved heading into Thu open.

---

## Current Positions (25 equity + 1 frac + 1 crypto, EOD May 20)

| Ticker | Shares | Entry | Last | P&L | P&L % | Stop | Buffer |
|--------|--------|-------|------|-----|-------|------|--------|
| **UNH** | 0.69 | $290.00 | $383.30 | +$64 | **+32.2%** | — frac | n/a |
| **CVS** 🎯 | 27 | $75.83 | $94.01 | +$491 | **+23.9%** | $87 | 8.0% |
| **TXN** 🔧 | 5 | $272.83 | $304.88 | +$160 | **+11.7%** | **$293 (ratched today)** | 3.9% (locks +$101) |
| **DXCM** 🔧🆕 | 4 | $64.85 | $71.44 | +$26 | **+10.2%** | **$66 (ratched today)** | 7.6% (locks +$4.60) |
| **CCI** | 20 | $84.31 | $92.64 | +$167 | +9.9% | $84.31 | 9.0% (breakeven) |
| **BTC** | 0.0034 | $70,867 | $77,470 | +$23 | +9.3% | — crypto | n/a |
| **CRWD** 🚀🔧 | 1 | $609.48 | $647.76 (AH $650.34) | +$38 | **+6.3%** | **$620 (ratched today)** | 4.5% (locks +$10.52) |
| **GE** 🆕 | 2 | $285.99 | $298.32 | +$25 | +4.3% | $263 | 13.4% |
| **SYY** | 5 | $73.21 | $75.46 | +$11 | +3.1% | $68 | 11.0% |
| **BSX** | 5 | $55.14 | $56.67 | +$8 | +2.8% | $51 | 11.1% |
| **PANW** 🆕 | 1 | $243.21 | $246.45 | +$3 | +1.3% | $225 | 9.5% |
| **NUE** | 9 | $223.00 | $225.67 | +$24 | +1.2% | $210 | 7.5% |
| **MSFT** | 1 | $415.53 | $419.91 | +$4 | +1.1% | $395 | 6.3% |
| **MRK** | 18 | $112.47 | $113.25 | +$14 | +0.7% | $107 | 5.8% YELLOW |
| **BA** 🔄re-entry | 3 | $220.33 | $221.20 | +$3 | +0.4% | $202 | 9.5% |
| **TJX** 🆕 | 4 | $159.00 | $159.21 | +$1 | +0.1% | $146 | 9.0% |
| **OKTA** 🆕 | 5 | $89.36 | $88.95 | -$2 | -0.5% | $82 | 8.5% |
| **BLK** | 2 | $1,057.92 | $1,051.57 | -$13 | -0.6% | $990 | 6.2% (SpaceX IPO catalyst) |
| **MRVL** 🆕 | 5 | $189.11 | $186.50 | -$13 | -1.4% | $174 | 7.2% (NVDA AH risk Thu) |
| **D** | 4 | $68.82 | $67.49 | -$5 | -1.9% | $63 | 7.1% |
| **CSCO** | 1 | $117.34 | $114.34 | -$3 | -2.6% | $108 | 5.9% YELLOW |
| **NFLX** 🆕 | 5 | $91.12 | $88.20 | -$15 | -3.2% | $84 | 5.0% YELLOW |
| **ZS** 🆕 | 3 | $180.83 | $174.45 | -$19 | -3.5% | $165 | 5.7% YELLOW |
| **BILL** | 64 | $40.17 | $38.34 | -$117 | -4.6% | $36 | 6.5% |

**Total open unrealized P&L: ~$865 EOD**. **Realized today: $0** (no stops fired).

🔥 **Today's Catalyst Highlights:**
- **NVDA Q1 print**: EPS $1.87 BEAT $1.76 (+6.25%) / Sales $81.62B BEAT $78.80B / **+139.74% YoY EPS growth** — BUT AH selling -2.3% ($223→$218) = sell-the-news
- **CRWD 11-leg sell-side cluster** completed (Cantor $700 + MS $610 + Stifel + earlier 8 from Mon-Tue) + ATH break $646.62 today → ratchet $600→$620
- **SpaceX $75B IPO June timeline** + BLK 13% stake target (held position direct beneficiary)
- **GOOG $15B Missouri AI infra** + Ameren 500MW capacity (hyperscaler capex confirms AI thesis)
- **WBD $30B LBO bond signal** (M&A imminent, not held)

---

## ⭐ Sector Sleeve Status

| Sleeve | Target | Current Fill | Status | Members Held |
|--------|-------:|-------------:|--------|--------------|
| **semi_ai** | $9,318 (30%) | ~$2,457 (7.9%) | **26% of target** | MRVL $933 + TXN $1,524 |
| **cyber** | (sub-tech) | ~$1,862 (6.0%) | 11-leg cluster active | CRWD $648 + ZS $523 + OKTA $445 + PANW $246 |

Sleeve regime: **HOT** semi_ai (NVDA catalyst persistent despite AH sell-the-news) + **HOT** cyber (CRWD 11-leg + S/AWS competitive note). Tech total = semi $2,457 + SaaS BILL $2,454 + cyber $1,862 = **~$6,773 / 21.8%** of $31,059 — well under raised 50% ceiling.

---

## Allocation (EOD May 20)

| Category | Value | Weight |
|----------|-------|--------|
| **Tech / Semi-AI** (MRVL, TXN, MSFT) | $2,877 | 9.3% |
| **Cyber** (CRWD, ZS, OKTA, PANW) | $1,862 | 6.0% |
| **SaaS** (BILL, CSCO) | $2,568 | 8.3% |
| **TECH TOTAL** | **$7,307** | **23.5%** (well under raised 50% ceiling) |
| Healthcare (MRK, CVS, UNH, BSX, DXCM) | $5,394 | 17.4% |
| Financials (BLK) | $2,103 | 6.8% |
| Materials (NUE) | $2,031 | 6.5% |
| Consumer Discretionary (TJX, NFLX) | $1,078 | 3.5% |
| Real Estate (CCI) | $1,853 | 6.0% |
| Consumer Staples (SYY) | $377 | 1.2% |
| Industrials (GE, BA) | $1,260 | 4.1% |
| Utilities (D) | $270 | 0.9% |
| Crypto (BTC) | $267 | 0.9% |
| **Cash** | $9,102 | **29.3%** |

---

## Open Orders (22 active GTC stops)

| Type | Ticker | Qty | Trigger | TIF | Notes |
|------|--------|-----|---------|-----|-------|
| Stop | **CRWD** 🚀 | 1 | **$620.00** | GTC | Ratcheted today (locks +$10.52 above entry on 11-leg cluster + ATH) |
| Stop | **TXN** 🔧 | 5 | **$293.00** | GTC | Ratcheted today close (locks +$100.88 / +11.7% lifecycle) |
| Stop | **DXCM** 🔧 | 4 | **$66.00** | GTC | Ratcheted today close (locks +$4.60 above entry) |
| Stop | CVS 🎯 | 27 | $87.00 | GTC | +23.9% lifecycle protected |
| Stop | **BA** 🆕 | 3 | $202.00 | GTC | New AM (re-entry catalyst-buy 09:58 ET) |
| Stop | **TJX** 🆕 | 4 | $146.00 | GTC | New AM (beat-and-raise catalyst-buy 09:58 ET) |
| Stop | **MRVL** 🆕 | 5 | $174.00 | GTC | New AM (chip-cluster catalyst-buy 09:58 ET); NVDA AH risk Thu |
| Stop | MRK | 18 | $107.00 | GTC | Phase 3 trofuse ratchet 5/18 |
| Stop | BILL | 64 | $36.00 | GTC | |
| Stop | BLK | 2 | $990.00 | GTC | SpaceX IPO catalyst building |
| Stop | CCI | 20 | $84.31 | GTC | Breakeven-lock |
| Stop | NUE | 9 | $210.00 | GTC | |
| Stop | GE | 2 | $263.00 | GTC | Set 5/19 |
| Stop | NFLX | 5 | $84.00 | GTC | YELLOW 5.0% cushion |
| Stop | OKTA | 5 | $82.00 | GTC | Set 5/19 |
| Stop | ZS | 3 | $165.00 | GTC | YELLOW 5.7% cushion |
| Stop | DXCM | 4 | (above) | GTC | (listed above with ratchet) |
| Stop | BSX | 5 | $51.00 | GTC | |
| Stop | D | 4 | $63.00 | GTC | |
| Stop | PANW | 1 | $225.00 | GTC | Set 5/15 |
| Stop | CSCO | 1 | $108.00 | GTC | YELLOW 5.9% cushion |
| Stop | MSFT | 1 | $395.00 | GTC | Blocks wash-trade adds |
| Stop | SYY | 5 | $68.00 | GTC | |

---

## Recently Closed

| Date | Ticker | Action | Realized | Notes |
|------|--------|--------|---------:|-------|
| 2026-05-19 | **BA** | Stop fired @ $216 (3 sh) | **-$46.85 / -1R** | Tue stop — India regulatory + macro rates compound (re-entered Wed 5/20 @ $220.33 on Beijing order confirmation) |
| 2026-05-13 | **AVGO** | Stop fired @ $407 (1 sh) | -$24.40 / -5.66% | 1R bounded loss |
| 2026-05-12 🎯 | **INTC** | Stop fired @ $120.01 (6 sh) | **+$138.97 / +23.93%** | Entry+5R lock; lifecycle +$256 / +44% |
| 2026-05-11 | CEG | Stop fired @ $289.52 (7 sh) | +$66.64 / +3.4% | Q1 mega-beat sold-the-news |
| 2026-05-11 | NKE | Stop fired @ $42.50 (44 sh) | -$122.62 / -6.2% | Consumer-disc pressure |
| 2026-05-08 🎯 | INTC | Target trim 6 sh @ $116.37 | +$117.15 / +20.1% | Apple-Intel deal day |
| 2026-05-07 | CVX | Stop fired @ $181.50 | -$104.20 / -5.4% | |

---

## Today's Catalyst Highlights (Wed 5/20)

### 🚀 Pipeline-Executed Catalyst-Buys (3, all tape-confirming)
- **MRVL** 5 sh @ $189.11 — Wells PT $135→$195 (+44%, above our Mon $169.94 exit); MU JPM bullish + Melius $1,100 PT confirm chip-cluster bull (+7.9% intraday)
- **TJX** 4 sh @ $159 — Q1 18% EPS BEAT + FY27 guide RAISE + buyback $2.75-3B; off-price differentiating from HD/LOW housing weakness (+5.6% intraday)
- **BA** 3 sh @ $220.33 (re-entry) — Beijing CONFIRMS Boeing order + Xi $30B tariff de-escalation framework; reverses Tue $216 stop's regulatory thesis (+2.4% intraday)

### 🛡️ Tape-Confirming PASS Decisions (saved capital)
- **MU** — top-scored catalyst (JPM bullish + Melius $1,100 PT) BUT tape -2.6% sell-the-news; **PASSED**
- **TGT** — BEAT-AND-RAISE (17% EPS beat + FY raise + buyback) BUT tape -7.7% sell-the-news; **PASSED** (validated 1.5h later when CFO said "consumer sentiment slipping")
- **NVDA** — Q1 BEAT $1.87/$81.6B/+139% YoY EPS BUT **AH tape -2.3%** sell-the-news; **PASSED on 4th cap deployment** (held reserve for Thu tape-confirm)

### 🔧 Ratchets Executed (3, all locking profit above entry)
- **CRWD** midday $600→$620 — locks +$10.52 above entry on 11-leg sell-side cluster + ATH break $646.62
- **DXCM** close $60→$66 — locks +$4.60 above entry (+10.2% lifecycle position)
- **TXN** close $285→$293 — locks +$100.88 lifecycle profit (+11.7% lifecycle)

### Thu 5/21 AM Watchlist
- **MRVL** — NVDA AH reaction Thu open; if -2.3% AH reverses or chip cluster green = HOLD/possible add; if NVDA continues down = expect MRVL sympathy decline
- **NVDA itself (not held)** — would need explicit tape-confirmation to re-enter chip sleeve at parent level
- **WBD** — $30B LBO bond signal AH; M&A spike monitoring
- **BLK** — SpaceX IPO June timeline follow-on PR possible Thu
- **NFLX/ZS/MRK/CSCO YELLOW positions** — cushion improvement or stop-out risk
- **CCI** breakeven $84.31 → push to $88 if no overnight macro shock

---

## Today's Mercury Catalyst Stack (24+ alerts; tape-confirming framework filter applied)

### 🔥 Headline Catalysts (Wed 5/20)
- **NVDA** 16:21 ET Q1 BEAT $1.87/$81.6B/+139% YoY — **MOST MATERIAL ALERT OF DAY** (AH tape rejecting -2.3%)
- **WBD** 16:21 ET — Banks Eye $30B Bonds for LBO (Bloomberg)
- **BLK/SpaceX** 16:04 ET — SpaceX $75B IPO as soon as June; BLK wants 13% stake
- **GOOG/AEE** 15:40 ET — $15B Missouri AI infra + 500MW Ameren capacity
- **CRWD** 12:43 ET — Morgan Stanley $610 + Cantor $700 + Stifel = completes 11-leg cluster

### Earlier Day Stack
- TJX BEAT-AND-RAISE Q1 (executed BUY)
- MU JPM "outlook strengthened" + Melius $1,100 PT (PASSED, tape rejected)
- TGT Q1 BEAT-AND-RAISE (PASSED, tape -7.7%)
- BA Beijing CONFIRMS order + Xi $30B tariff (executed BUY re-entry)
- MRVL Wells $135→$195 + Oppenheimer $200 + Wolfe Hold→Buy (executed BUY)
- ARM Bernstein $300 PT + $2B agentic AI chip demand (not held)
- Managed care 5-firm cluster (Deutsche ELV/CNC/HUM + Mizuho ELV/HUM) — UNH held implicit
- BMY×Anthropic enterprise + INCY×Genesis Molecular (pharma×AI)
- Singapore AI cluster 4-mega-cap (NVDA hub + OpenAI + GOOG)

---

## Process Notes (this week)

1. **Pipeline discipline 2026-05-20 (Wed): 100%** — Every BUY went through 5-agent fast-track. Zero process violations through 3 days (Mon/Tue/Wed) and 11 catalyst-buys.
2. **Tape-confirming framework validated 4 times today** — MU, TGT, NVDA AH (all PASSED despite top catalyst scores when tape rejected); MRVL/TJX/BA (all EXECUTED when catalyst+tape aligned). AMAT 13-catalyst lesson reapplied.
3. **Wash-trade architectural lesson** — MSFT add on OpenAI $1T IPO blocked by existing $395 stop; held 4th cap slot reserved vs 3-step cancel-buy-replace choreography.
4. **NVDA AH price discovery** — Massive beat (+139% YoY EPS) + AH selling is the year's clearest sell-the-news case study; tape-confirming framework saved 4th cap slot for Thu tape-confirm rather than chasing the catalyst.
5. **PDT same-day stops continue OK above $25K** (equity $31,059 well above floor).
