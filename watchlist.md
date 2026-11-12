# Watchlist — Last update 2026-11-12 16:20 ET (eod_summary)

## EOD snapshot — 2026-11-12

- **Equity:** $30,113 (-0.03% day) · **Cash:** $24,199 (80.4%) · **Trades:** 3/4 (SMCI 34 @ $26.545, TTEK 23 @ $39.145, BABA 9 @ $94.773; all OTO/stop attached) · **Blocked/unfilled:** NVDA BUY limit unfilled and cancelled (10:12); NVDA 12:35 WATCH · **Stops fired:** 0
- Movers: top gainers/losers all sub-$10 microcaps/warrants (POAS, GP, CDNL, SMX...) — outside universe, ignored.
- Positions: REGN 2 @ $948 (+28.6%, stop $793.30) · ABBV 3 @ $294.45 (+7.8%, stop $253.27) · SMCI 34 @ $27.16 (+2.3%, stop $24.30) · TTEK 23 @ $39.24 (+0.2%, stop $36.90) · BABA 9 @ $94.67 (-0.1%, stop $89) · UNH 0.52 @ $404.75 (+39.6%, no stop, fractional) · BTCUSD @ $71,440 (+0.8%, stop-limit 66,661/66,500) · 737CVR019 CVR.
- Open stops intact on all whole-share/BTC positions; none within 5% of price (BABA stop 6.0% below).

---

## Dip scan — 2026-11-12 11:12 ET (stock_dip_scan)
| **BABA** | WATCH | $94.83 (-6.6%) | Score 71, legal_regulatory/geopolitical: Megaspeed/Nvidia spy-probe link ($4.1B Singapore prepayments). Pipeline `2026-11-12-1112-BABA`. Atlas: 18 similar drops, 30d win 28%, avg -6.8%. Unresolved event risk. Re-check on probe resolution or a flush toward $89. |
| NVDA | pipelined 10:12 (BUY, limit not filled, cancelled) | | CEO ouster; see pipeline `2026-11-12-1012-NVDA` |

## EOD snapshot — 2026-11-11

- **Equity:** $30,122 (+0.30% day) · **Cash:** $26,855 (89.2%) · **Trades:** 0/4 · **Blocked:** 2 (DELL, GOOGL volume gate) · **Stops fired:** 0
- Movers: top gainers/losers all sub-$10 microcaps/warrants (NXXT, WHLR, ENGS, BMGL…) — outside universe, ignored.
- Positions: REGN 2 @ $959.41 (+30.1%, stop $793.30) · ABBV 3 @ $294.03 (+7.6%, stop $253.27; closed just above the $293.21 1R trigger — close-based breakeven check due tomorrow) · UNH 0.52 @ $402.80 (+38.9%, no stop, fractional) · BTCUSD @ $74,603 (+5.3%, stop-limit 66,661/66,500) · 737CVR019 CVR.
- Open orders: REGN, ABBV, BTC stops intact. No stop within 5% of price.

---

## Delta check — 2026-11-11 13:18 ET (autopilot_midday re-fire, no pipeline)

Second invocation of the midday slot, 30 min after the 12:47 run. Positions, stops, Mercury set (7 flagged, none ≥70), Oracle and sleeve state unchanged. Re-measured the two open conditions and triaged one new dip; nothing entered the pipeline. Debrief: `journal/autopilot-runs/2026-11-11-1318-midday-refire.md`.

| Ticker | Status | Price (13:19) | Re-check | Watch for |
|--------|--------|---------------|----------|-----------|
| **DELL** | still BUY BLOCKED | $382.81 | SIP 5.84M through ~13:05 vs 20d avg 7.71M → ~1.38x time-adjusted, falling (1.51x → 1.45x → 1.38x). Price in the $378–388 zone. Not re-pipelined. | Close run: full-day ≥11.6M and price > $370 / > $340 → fresh fast-track. Unlikely at the current pace (~9–10M projected). |
| **GOOGL** | still BUY BLOCKED | $294.84 | 13.72M through ~13:05 vs 40.3M 20d avg → ~0.62x. Not re-pipelined. | ≥1.5x volume session with price > $279 |
| **SE** | filtered (dip score ~45), new | $74.05 (-3.6%) | Q3 11/10: revenue +43% beat, EPS miss, $1B buyback; day-1 full reversal (high $85.16 → close $76.80), day-2 drift. Volume 6.38M vs 8.87M 20d avg = ~1.29x time-adj / 0.33x raw vs the 19.5M earnings bar. 10/20 -9% gap never recovered; -24% from 10/15 high. ~$45B cap. | Hold of the 10/26 low $71.53 on ≥1.5x volume with a reversal bar, or a close back above $77 → dip-scan triage with fresh event study |
| PEPE | deferred | -8.2% | Memecoin tier 35 — crypto_dip_scan (13:29) owns it | — |

- **Equity:** $30,066 · **Cash:** $26,855 (89.3%) · **Trades today:** 0/4 · **Spend:** $0/$5K
- **ABBV** $292.46, day high $292.58 — still below the $293.21 1R breakeven trigger (close-based)

---

## Wed 11/11 Position Book (12:48 ET, live Alpaca)

| Ticker | Qty | Basis | Price | Unrl P&L | Stop | Status |
|--------|-----|-------|-------|----------|------|--------|
| **REGN** | 2 | $737.32 | $931.48 | +26.2% | $793.30 GTC (entry+1.5R) | GREEN — hold; 5.2R; CIDEB siRNA liver-fat data 11/10 positive; no thesis file (legacy flag) |
| **ABBV** | 3 | $273.24 | $291.85 | +6.8% | $253.27 GTC | GREEN — 0.93R, still below the 1R breakeven trigger ($293.21); raised guidance per coverage |
| **UNH** | 0.52 | $290 | $398.21 | +37.3% | none (fractional) | GREEN — unprotected by design; third guidance raise this year; Medicare exits in 140 counties noted |
| BTCUSD | 0.00345 | $70,867 | $74,500 | +5.1% | 66,661/66,500 stop-limit | hold |
| 737CVR019 | 4.06 | $0 | n/a | n/a | n/a | CVR, no market |

- **Equity:** $30,055 · **Cash:** $26,855 (89.4%) · **Trades today:** 0/4 · **Spend:** $0/$5K (GOOGL and DELL both Diana BUYs blocked by the volume gate — not counted)
- **Sleeve semi_ai:** $0 / $9,017 target (0%) — UNDER-FILLED, regime COLD (auto, 0 qualifying alerts ≥70 in 7d)

## Watch — pipeline outcomes 2026-11-11 midday (autopilot_midday 12:47)

| Ticker | Status | Price | Why | Watch for |
|--------|--------|-------|-----|-----------|
| **DELL** | BUY BLOCKED (volume gate ~1.45x) | $382.45 | Full pipeline passed: Iris/Leo/Atlas bull (50–52), Grace bull 60, Nate bull 55, Ray neutral, Catherine medium, Victor ELEVATED, Diana BUY 4sh @ $383.25, stop $340, target $440, hard review 11/21 before the 11/24 print. Marcus CONDITIONAL on ≥1.5x time-adjusted volume vs 20d avg; measured ~1.51x on the ~12:38 bar, ~1.45x on the ~12:48 bar → blocked (borderline). | Close run (15:53): full-day volume ≥11.6M and price > $370 and > 200-day ($340) → re-run fast-track for a fresh Diana call. Thesis: `journal/theses/2026-11-11-DELL-buy.md`. Pipeline: `journal/pipeline/2026-11-11-1255-DELL/` |
| **INTC** | WATCH (scan gate, 3 neutrals) | $63.46 | +9.3% on CoreWeave relief, 2.5x adj volume; post-earnings crash chart (-29% on 10/30, -59% from high); CEO bought 150K sh ~$64.73 (11/04), RBC Hold PT $75; no foundry customer, no dated catalyst; base rates are pre-crash artefacts. Sleeve member, regime COLD. | Close above $66 (crash-day gap area) on volume, a named foundry customer, or a guidance reset. Pipeline: `journal/pipeline/2026-11-11-1255-INTC/` |
| **ORCL** | PASS (scan gate, 3 bears) | $130.54 | +10.6% on 2.4x adj volume, but structural narrative: Microsoft lease non-renewal, Tencent $7B deal lost/walked, $169B debt, FCF -$28.7B TTM, record CDS; up-days get sold (10d after +4% days: -0.5%, 42% positive, n=43). Bernstein $325 Buy maintained. Earnings 12/09. | Five closes above $127 (20-day SMA) on declining volume, or a financing/contract headline. Pipeline: `journal/pipeline/2026-11-11-1255-ORCL/` |
| **GOOGL** | still BUY BLOCKED (morning) | $293.99 | Price above $279 and inside the $288–294 entry zone, but SIP volume 12.4M by 12:47 ≈ 0.6x the 20-day average (40.3M). Not re-pipelined. | ≥1.5x volume session with price > $279; close > $300 on volume; Anthropic IPO pricing |
| MSFT | noted, not pipelined | $521.42 | -2.2% on Anthropic Office/Excel tools competition headline while XLK +4.3% — idiosyncratic quality dip but below the 3% threshold; CFO plan sale 11/10; RBC bullish into Ignite. | -3% or more on ≥1.5x volume → dip-scan candidate; Ignite headlines |
| FIS | filtered | $30.12 | +6.4% on 2.6x adj volume is a dead-cat bounce: guidance cut, six red days, -30%, new 1-year low today; guidance_cut overreaction 0.2. | No action |

---

## (previous) Dip scan — 2026-11-11 12:11 ET (no fast-track)

Movers feed again micro-cap/warrant only. Full 298-name universe snapshot (282 live, 16 stale — same hygiene list as 10:14 plus ABC): only two live ≥3% dips, both fail the volume gate 2.7h into the session.

| Ticker | Move | Vol (raw / time-adj) | News | Note |
|--------|------|----------------------|------|------|
| ABNB | -3.09% @ $181.16 | 0.66x / ~1.58x | Unchanged from 10:14 — post-earnings digestion + CSO $21.9M insider sale; no new catalyst | Dedup: move within 2pp of 10:14 alert, raw vol still < 1.5x. Price holds > $178. Fresh 3-yr event study (45 prior ≥3% drops): T+5 win 47% avg -0.46%, T+20 win 58% avg -0.09% — mixed-to-unfavorable, weaker than the 70-event read this morning. Not a dip-buy at this volume. |
| LULU | -3.69% @ $106.29 | 0.37x / ~0.90x | Names Ben Hallam / Emily Sunderland to top roles (management change, ~0.5); "securities notice" items are law-firm ads | ~$12.5B cap, barely inside $10B floor. Volume gate fails outright. Filtered. |

CI recovered to < 2.5% down — no longer a candidate.

**Context for autopilot_midday (12:47):** broad semi/AI rally on CoreWeave results easing AI-demand worries — MU +13.2%, ARM +12.8%, MRVL +12.0%, SMCI +10.9%, ORCL +9.4%, INTC +9.1%, AMAT/LRCX/AMD +7.4-7.7%, AVGO +6.7%, KLAC +6.5%, QCOM +3.7%. Only INTC (1.15x raw), ORCL (1.06x), FIS (1.01x) and ROK (1.06x) show raw vol ≥ 1x at midday. This is sector_tailwind (0.7 overreaction) — chasing risk; Phoenix should weigh under-reaction ratios, not magnitude. None held (position book: REGN, ABBV, UNH, BTC) — no take-profit signals.

---

## (previous) Dip scan — 2026-11-11 10:11 ET (no fast-track)

Movers feed was micro-cap/warrant only (nothing ≥ $10B). Full 298-name universe snapshot: two real ≥3% dips, both failed the raw 1.5x volume gate 41 min into the session (same convention that blocked GOOGL at 10:06).

| Ticker | Move | Vol (raw / time-adj) | News | Score (if vol passed) | Note |
|--------|------|----------------------|------|-----------------------|------|
| ABNB | -3.19% @ $180.96 | 0.23x / ~2.2x | Day-2 post-earnings slide; CSO Blecharczyk sold $21.9M (insider_sale, ~0.5); $12B buyback + guidance already out | ~62 (+10 news) | Not held. 70 prior ≥3% drops: T+20 win 56%, avg +0.75% — mixed. Re-check at 11:11 if raw vol ≥ 1.5x and price holds > $178 |
| CI | -3.12% @ $293.71 | 0.34x / ~3.2x | Investor-day: $45 EPS by 2030 target, Bernstein PT → $390; ACA exit in 11 states. Drop reads as guidance digestion, not a miss | ~60 | Not held (UNH is; insurer overlap). 33 prior ≥3% drops: T+20 win 64%, avg +1.95%. Re-check at 11:11 |

**Stale-ticker hygiene (universe.yaml):** EQR flagged as -3.5% on 1.66x but its snapshot is from 2026-08-17 (prev bar 08-14) — not a live move. AVB (08-14) same; headlines show AvalonBay now trades as VMRK (Vivmark Residential). 15 universe names returned non-today snapshots: AVB, CFLT, DFS, EQR, EXAS, HBI, HES, LBRDK, MMC, PXD, SQ, WBA, WBD, X, ZI. PARA prints $0.07. Recommend pruning / remapping before these generate another false dip.

---

# (previous) Watchlist — 2026-11-11 10:05 ET (autopilot_morning)

## Wed 11/11 Position Book (10:00 ET, live Alpaca)

| Ticker | Qty | Basis | Price | Unrl P&L | Stop | Status |
|--------|-----|-------|-------|----------|------|--------|
| **REGN** | 2 | $737.32 | $902.50 | +22.4% | $793.30 GTC (entry+1.5R) | GREEN — hold; 4.4R; no thesis file, target-trim logic skipped; 3R trim = 0 sh on 2-share lot |
| **ABBV** | 3 | $273.24 | $291.20 | +6.6% | $253.27 GTC | GREEN — 0.90R, below 1R breakeven trigger ($293.21); watch |
| **UNH** | 0.52 | $290 | $402.45 | +38.8% | none (fractional) | GREEN — unprotected by design; known limitation |
| BTCUSD | 0.00345 | $70,867 | $73,533 | +3.8% | 66,661/66,500 stop-limit | hold |
| 737CVR019 | 4.06 | $0 | n/a | n/a | n/a | CVR, no market |

- **Equity:** $30,005 · **Cash:** $26,855 (89.5%) · **Trades today:** 0/4 · **Spend:** $0/$5K
- **Sleeve semi_ai:** $0 / $9,002 target (0%) — UNDER-FILLED, regime COLD (auto, 0 qualifying alerts ≥70 in 7d)

## Watch — pipeline outcomes 2026-11-11 AM

| Ticker | Status | Price | Why | Watch for |
|--------|--------|-------|-----|-----------|
| **GOOGL** | BUY BLOCKED (volume gate 0.49x) | $290.90 | Full pipeline passed: Diana BUY 7sh @ $291.50, stop $268, target $330 (medium conviction, Victor ELEVATED). Marcus condition on Mercury 1.5x volume failed. | Session with ≥1.5x volume and price > $279; Anthropic IPO pricing; close > $300 on volume. Thesis: `journal/theses/2026-11-11-GOOGL-buy.md` |
| **AMZN** | WATCH (research gate 1/3) | $273.33 | Mercury 77.5 (Anthropic stake mark ~$258B, unverified). Grace neutral (FCF -$47B, fwd P/E > trailing), Ray neutral, Nate bull. | Pullback to $256–262 (SMA20) that holds; FCF guidance for 2027; IPO pricing |
| **TSM** | WATCH (scan gate) | $412.12 | Board $1B Anthropic/OpenAI + NT$9 dividend; +4.3% but zero idiosyncratic (SMH +4.4%); Leo/Atlas: chasing +4% days is negative-expectancy; Taiwan stabilization fund = stress signal. Not in `config/universe.yaml` despite sleeve membership. | Pullback to $400–405 holding; NVDA 11/17 read-through |
| CRWV | noted, not pipelined | $55.53 | +14% on Q3 beat/raised outlook, $133B backlog; unprofitable, GPU-backed debt at ~16% yields, Chanos short; not in universe | Pullback after breakout; only as momentum play with tight stop |

---

# (history) Watchlist — 2026-10-07 16:30 ET (Wed EOD) — position book below is STALE; see top of file

## Wed 10/7 Position Book (CLOSE)

| Ticker | Qty | Basis | Close | Day% | LC% | Stop | Cushion |
|--------|-----|-------|-------|------|-----|------|---------|
| **NVDA** 🔥 | 15 | $229.00 | $237.42 | -0.75% | +3.68% | $205 GTC | 13.7% |
| **AVGO** 🔥 | 3 | $353.38 | $376.51 | +0.16% | **+6.55%** | $360 L4 | 4.4% |
| **HPE** 🔥 | 14 | $64.00 | $72.12 | **+2.21%** | **+12.68%** | **$67 L5** | 7.1% |
| **MU** ✅ | 1 | $1,061.09 | $1,085.83 | **+3.86%** | **+2.33% GREEN** | $1,000 | 7.9% |
| **REGN** ✅ | 2 | $737.32 | $742.42 | +0.50% | +0.65% | $700 | 5.7% |
| **MRVL** 🆕 | 3 | $284.88 | $284.72 | -0.80% | -0.05% | $260 | 8.7% |
| **ABBV** 🆕 | 3 | $273.24 | $271.41 | +1.74% | -0.63% | $255 | 6.0% |
| **SYM** | 15 | $41.00 | $43.33 | -1.90% | +5.68% | $35 | 19.2% |
| **SYY** ⚠️ | 5 | $73.21 | $76.79 | -0.85% | +4.89% | $74.45 | 3.0% |
| **UNH** | 0.52 | $290 | $375.50 | -0.22% | +29.5% | frac | n/a |
| **DLR** ⚠️ | 4 | $198.87 | $180.43 | **-2.29%** | -9.27% | $167.78 | 7.0% |
| BTCUSD | 0.003 | $70,867 | $83,517 | -1.01% | +17.9% | frozen | n/a |

- **Equity:** $30,577.93
- **Cash:** $18,400.61 (60.2%)
- **Wed trades:** 2 (MRVL AM + ABBV MID) · 2/4 slots · $1,675/$5K
- **Cycle P&L Wed→Wed 7 days:** **+$419 / +1.39%**

## Session Cumulative (Wed→Wed, 7 trading days)

- **6 pipeline BUYs HELD:** HPE/REGN/AVGO/MU/MRVL/ABBV
- **4 GREEN + 2 flat/down; zero stop-fires** 7 days
- Session cycle spend: $5,312 deployed

## Wed close key events

1. **MU +3.86% GREEN flip** — NLST $600M 2nd settlement ABSORBED; held bull thesis validated
2. **HPE L5 ratchet $66→$67 (1.56R)** — 5-level cycle COMPLETE, max reserve, +$42 locked
3. **MRVL 3sh pipeline BUY $284.88** — 3-firm Investor Day cluster (Needham $400/Susq $340/Evercore $433)
4. **ABBV 3sh pipeline BUY $273.24** — dual FDA Breakthrough Therapy Designations (Telisotuzumab Adizutecan ADC)
5. **AVGO** +6.55% LC Day 4 FT $60B holding ($7.44 from L5 trigger)
6. **DLR** -2.29% despite Japan 24MW catalyst (digestion); cushion 7.0% watch

## Thu 10/8 Setup Priorities

1. **AVGO L5** at $383.95+ (1.5R) → $7.44 away
2. **MU breakeven** at 1R $1,122 → $36 away
3. **REGN breakeven** at 1R $775 → $33 away
4. **MRVL Day 3** continuation (Investor Day sustain)
5. **ABBV FDA Day 2** continuation
6. **DLR** cushion monitor (-9.27% LC)
7. **HPE L5 max reserve** Day 7 continuation
8. Session cap 2/4 Wed → fresh Thu 4+$5K

---

# EOD Snapshot — 2026-11-10 (eod_summary)

- **Equity:** $30,028.75 (prev close $30,039.37, -$10.62 / -0.04%) · **Cash:** $26,854.74 (89.4%)
- **Trades today:** 0 buys/sells filled. Stop maintenance only: REGN stop replaced to $793.30 (14:37Z), BTC/USD stop-limit placed 66,661/66,500 (14:43Z)
- **Blocked trades:** none recorded in Alpaca orders
- **Movers (EOD):** top gainers/losers all micro/penny names (PGRW, SMX, NXXT, LICN...) — below quality filter, no dip/jump candidates

| Position | Qty | Price | Unrl P&L | Stop |
|---|---|---|---|---|
| REGN | 2 | 913.63 | +$352.62 (+23.9%) | $793.30 |
| ABBV | 3 | 293.89 | +$61.96 (+7.6%) | $253.27 |
| BTCUSD | 0.00345 | 73,852 | +$10.30 (+4.2%) | 66,661/66,500 |
| UNH | 0.5197 | 404.69 | +$59.60 (+39.5%) | **NONE (fractional)** |
| 737CVR019 | 4.06 | n/a | n/a | n/a (CVR, zero basis) |

- **Stop-loss hits:** none. All priced positions well above stops.
- **Flag:** UNH has no active stop order.

- 2026-11-12 BABA HELD: 9 @ 94.773, stop 89.00 (18e10420), target 104. dip-buy on US remote AI-chip curb report. Exit early on a final rule; time-box ~5 sessions. Pipeline journal/pipeline/2026-11-12-1311-BABA/
- 2026-11-12 NVDA (-4.9%, CEO transition, score ~66), GPN (-10%, PE takeover interest dropped, ~58), FIS (earnings), MSTR (MSCI deletion): not fast-tracked this run (one pipeline per scan).
