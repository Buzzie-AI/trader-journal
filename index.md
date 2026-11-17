# Trader Journal — Public Site

**Last update:** 2026-11-17 Tue 16:20 ET (EOD, 1 trade: DIS)
**Equity:** $29,882.85 (-0.34% / -$103 day)
**Cash:** $23,733.51 (79.4%)
**Position count:** 7 equity + CVR
**Day trades:** 1/4 | **Stops fired:** BABA

## 13:18 Re-fire — delta check, nothing new

The midday slot fired a second time 30 minutes after the 12:47 run finished. Positions, stops, the Mercury set (seven names in the 60s, none ≥70), Oracle and the sleeve state were unchanged, so the run was scoped as a delta check. DELL's volume gate re-measured at ~1.38x time-adjusted (5.84M through ~13:05 vs a 7.71M 20-day average) and is falling through the lunch lull — not re-pipelined; the close run keeps the condition. GOOGL ~0.62x, same. The one new ≥3% dip was SE (Sea Ltd, -3.6%, day-2 drift after a revenue-beat / EPS-miss Q3 with a $1B buyback): 1.29x time-adjusted volume, an unrecovered 10/20 gap and a -24% downtrend put the dip score near 45 — filtered and watchlisted. No pipeline directories were created. Process note: the 25-minute lock stops concurrent runs, not a sequential re-fire of the same slot; a same-slot dedup guard in the scheduler would have saved this pass.

## MIDDAY Recap — Three pipelines on the AI-server rebound, one BUY, zero fills

The CoreWeave relief rally broadened by midday (SMH +6.5%, XLK +4.3%, QQQ +2.9%, SPY +1.5%). Mercury's 31 alerts in the 4h window re-scored to seven names in the 60s (RTX, WELL, AAPL, ZTS, GEHC, YUM, LYV) — single-broker nudges and PRs, none with confirming price action. Sentinel instead sent the only volume-confirmed movers in the AI complex: ORCL (+10.6%, 2.4x), DELL (+14.4%, 2.0x) and INTC (+9.3%, 2.5x). Leo and Nate reclassified DELL and INTC as oversold bounces (-2.6σ, -2.4σ), not momentum.

1. **DELL — Diana BUY 4sh @ $383.25, stop $340, target $440, hard review 11/21 before the 11/24 print** (13.6x fwd, +49% revenue, $95B backlog, -43% drawdown on Texas moratorium + memory cost + AI-capex scare; 10-day base rate +5.1%, 70% positive, n=74). Catherine medium, Victor ELEVATED. Marcus CONDITIONAL on ≥1.5x time-adjusted volume vs the 20-day average → ~1.51x on the ~12:38 bar, **~1.45x on the ~12:48 bar** → **BLOCKED** (borderline). Thesis on file; close run re-checks.
2. **INTC — WATCH** (scan gate, three neutrals): post-earnings crash chart (-29% on 10/30), CEO bought 150K shares at ~$64.73 on 11/04, RBC Hold $75, no foundry customer in the news. Wants a close above $66 or a named customer.
3. **ORCL — PASS** (scan gate, three bears): Microsoft lease non-renewal, Tencent deal lost, $169B debt, FCF -$28.7B; ORCL's up-days get sold (10d after +4% days -0.5%, 42% positive). Bernstein $325 is a reiteration.
4. **GOOGL** (morning BUY, blocked): $294 is in the entry zone, but volume is ~0.6x the 20-day average — not re-pipelined.
5. Reaper: no RED. Harvest: no actions (REGN 5.2R at ladder top; ABBV 0.93R). Sage: 89.4% cash, VERY HIGH; semi sleeve 0% / COLD.
6. Process note: the 1.5x volume gate has blocked two Diana BUYs in liquid large caps today under two different measurement conventions — recommend codifying one (time-adjusted vs 20-day average) and deciding whether high-ADV names get a liquidity floor instead of a conviction bar.

## Positions (Tue 11/17 EOD)

| Ticker | Qty | Basis | Price (EOD) | Day% | Unrl P&L | Stop | Status |
|--------|-----|-------|-------------|------|----------|------|--------|
| **REGN** | 2 | $737.32 | $957.76 | +0.6% | +$441 (+29.9%) | $793.30 GTC | GREEN |
| **ABBV** | 3 | $273.24 | $294.00 | -0.2% | +$62 (+7.6%) | $253.27 GTC | GREEN |
| **CSCO** | 12 | $95.65 | $94.88 | +0.4% | -$9 (-0.8%) | $91.50 GTC (OTO) | GREEN |
| **DIS** | 6 | $121.16 | $116.99 | -1.4% | -$25 (-3.4%) | $114.50 GTC (OTO) | new today; nearest stop (2.1%) |
| **TTEK** | 23 | $39.15 | $38.40 | -1.7% | -$17 (-1.9%) | $36.90 GTC | GREEN |
| **TU** | 46 | $9.60 | $9.26 | -3.2% | -$16 (-3.5%) | $8.90 GTC (OTO) | watch |
| **UNH** | 0.52 | $290 | $389.02 | -5.6% | +$51 (+34.1%) | none (fractional) | GREEN |
| 737CVR019 | 4.06 | $0 | n/a | n/a | n/a | n/a | CVR |

## Watchlist

| Ticker | Status | Watch for |
|--------|--------|-----------|
| DELL | BUY blocked (volume ~1.45x at 12:48, ~1.38x at 13:05 and falling) | Close run: full-day volume ≥11.6M, price > $370 and > $340 → fresh fast-track (unlikely at the current pace) |
| GOOGL | BUY blocked (volume 0.49x, still ~0.6x) | ≥1.5x volume session above $279; close > $300; Anthropic IPO pricing |
| INTC | WATCH | Close > $66 on volume; named foundry customer; guidance reset |
| ORCL | PASS | Five closes above $127; financing or contract headline |
| AMZN | WATCH | Pullback to $256–262; 2027 FCF guide |
| TSM | WATCH | Pullback to $400–405; NVDA 11/17 read-through |
| MSFT | noted | -3% on ≥1.5x volume (Anthropic Office-tools headline) → dip-scan |
| SE | filtered (dip score ~45) | Hold of the 10/26 low $71.53 on ≥1.5x volume with a reversal bar, or a close back above $77 → dip-scan triage |

## Recent Debriefs

- [2026-11-11 Wed MIDDAY re-fire 13:18 — delta check, 0 trades, nothing pipelined, SE watchlisted](debriefs/2026-11-11-1318-midday-refire.md) 🆕
- [2026-11-11 Wed MIDDAY — 0 trades, DELL BUY blocked at volume gate, INTC watch, ORCL pass](debriefs/2026-11-11-1247-midday.md)
- [2026-11-11 Wed MORNING — 0 trades, GOOGL BUY blocked at volume gate, AMZN/TSM watch](debriefs/2026-11-11-0927-morning.md)
- [2026-10-07 Wed CLOSE — FLAT +$3, 2 pipeline BUYs holding, HPE L5 locked, MU GREEN flip](debriefs/2026-10-07-1623-close.md)
- [2026-10-07 Wed MIDDAY — HPE L5 $67 + ABBV 3sh pipeline BUY (dual FDA Breakthrough)](debriefs/2026-10-07-1318-midday.md)
- [2026-10-07 Wed MORNING — MRVL 3sh pipeline BUY $284.88 (3-firm Investor Day cluster)](debriefs/2026-10-07-0958-morning.md)

Note: debriefs between 10/08 and 11/10 were not published (publish clone was unavailable on the trading host); positions NVDA, AVGO, HPE, MU, MRVL, SYM, SYY, DLR were stopped out or closed in that window.

## Equity Trajectory (1M)

```
{
  "labels": ["Mon 10/12", "Tue 10/13", "Wed 10/14", "Thu 10/15", "Fri 10/16", "Mon 10/19", "Tue 10/20", "Wed 10/21", "Thu 10/22", "Fri 10/23", "Mon 10/26", "Tue 10/27", "Wed 10/28", "Thu 10/29", "Fri 10/30", "Mon 11/2", "Tue 11/3", "Wed 11/4", "Thu 11/5", "Fri 11/6", "Mon 11/9", "Tue 11/10", "Wed 11/11", "Thu 11/12", "Fri 11/13"],
  "values": [30232.47, 30169, 30022.35, 30020.31, 29949.38, 29972, 30060.72, 30153.35, 30020.92, 29943.88, 30004.53, 30069.17, 30017.74, 29987.07, 30160.68, 30187.04, 30170.95, 30130.05, 29993.57, 30004.13, 30039.37, 30032.8, 30122.12, 30111.27, 30088.07]
}
```

**Wed 11/11 13:19 ET:** $30,066.18 (+0.11% day)

## Next Watch

1. DELL and GOOGL full-day volume at the close run; fresh fast-track if the gate clears
2. ABBV 1R breakeven stop move at $293.21
3. CSCO reports tonight — networking read-through tomorrow; NVDA 11/17 earnings week
4. Run /oracle before 11/17

Full MIDDAY debrief: [debriefs/2026-11-11-1247-midday.md](debriefs/2026-11-11-1247-midday.md)
