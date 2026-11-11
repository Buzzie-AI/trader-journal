# Portfolio Snapshot — 2026-11-11 16:20 ET (Wed EOD — 0 trades, DELL/GOOGL blocked at volume gate)

**Equity:** $30,122.34 (+$90 / +0.30% vs Tue close $30,032.80)
**Cash:** $26,854.74 (89.2%)
**Long value:** $3,267.60 (10.8%)
**Trades today:** 0/4 | **Spend:** $0/$5K
**Blocked today:** GOOGL 7sh @ $291.50 (09:59, volume 0.49x) · DELL 4sh @ $383.25 (13:04, volume ~1.45x vs 20d avg, need 1.5x — borderline)

## Current Positions

| Ticker | Qty | Basis | Price (16:20 ET) | Day% | Unrl P&L | Stop | Status |
|--------|-----|-------|------------------|------|----------|------|--------|
| **REGN** | 2 | $737.32 | $959.41 | +4.7% | +$444 (+30.1%) | $793.30 GTC | GREEN — 5.3R |
| **ABBV** | 3 | $273.24 | $294.03 | +0.0% | +$62 (+7.6%) | $253.27 GTC | GREEN — closed above $293.21 1R trigger; breakeven check next run |
| **UNH** | 0.52 | $290 | $402.80 | -0.6% | +$59 (+38.9%) | none (fractional) | GREEN |
| BTCUSD | 0.00345 | $70,867 | $74,603 | +1.4% | +$13 (+5.3%) | 66,661 / 66,500 stop-limit | hold |
| 737CVR019 | 4.06 | $0 | n/a | n/a | n/a | n/a | CVR |

## Allocation

- Healthcare: REGN $1,870 + ABBV $877 + UNH $208 = **$2,955 = 9.8%**
- Crypto: BTCUSD $257 = 0.9%
- Cash: 89.3%
- **Semi/AI sleeve:** $0 / $9,020 target (0%) — UNDER-FILLED, regime COLD (auto)

## Open Orders (all GTC)

- REGN stop $793.30 (order 43c3de82)
- ABBV stop $253.27 (order 67710004)
- BTC/USD stop-limit 66,661 / 66,500 (order a9807b29)
- UNH — no stop (fractional, not stop-eligible)

## Recently Closed

- HPE 14sh — stop $67 filled 10/14 @ $64.52
- MRVL 3sh — stop $259.94 filled 10/13 @ $254.65
- AVGO 3sh — stop $360 filled 10/08 @ $359.97
- (NVDA, MU, SYM, SYY, DLR closed between 10/08 and 11/10 — see cron-health log)

## Equity Curve (1M, daily close)

```
{
  "labels": ["Mon 10/12", "Tue 10/13", "Wed 10/14", "Thu 10/15", "Fri 10/16", "Mon 10/19", "Tue 10/20", "Wed 10/21", "Thu 10/22", "Fri 10/23", "Mon 10/26", "Tue 10/27", "Wed 10/28", "Thu 10/29", "Fri 10/30", "Mon 11/2", "Tue 11/3", "Wed 11/4", "Thu 11/5", "Fri 11/6", "Mon 11/9", "Tue 11/10"],
  "values": [30232.47, 30169, 30022.35, 30020.31, 29949.38, 29972, 30060.72, 30153.35, 30020.92, 29943.88, 30004.53, 30069.17, 30017.74, 29987.07, 30160.68, 30187.04, 30170.95, 30130.05, 29993.57, 30004.13, 30039.37, 30032.8]
}
```

Base value $30,352.81 as of 2026-10-09. Intraday Wed 11/11 13:19 ET: $30,066.18.

## Safety Gate Status

- Max 4 trades/day: 0/4 ✅
- Max $5K daily spend: $0 ✅
- Min $2K cash reserve: $26.9K ✅
- Max 10% per position: REGN 6.2% ✅
- Semi sleeve 0% < 50% ceiling ✅
- Circuit breaker: +0.30% ✅
- Stops: 3/3 stop-eligible positions covered ✅ (UNH fractional exempt)
- Limit orders only ✅
- Volume gate (1.5x): blocked GOOGL (0.49x) and DELL (~1.45x) today — both Diana BUYs held back
