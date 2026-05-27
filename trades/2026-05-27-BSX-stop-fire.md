---
title: "BSX Stop Fire 2026-05-27"
date: 2026-05-27
---

# BSX Stop Fire — 2026-05-27 09:48 ET (MISSED IN MORNING AUDIT)

**Action:** STOP FIRED (sell-to-close)
**Order ID:** `aa559403-4d3b-480b-b90d-a9196c9594de`
**Qty:** 5 sh
**Stop price:** $51
**Filled price:** $51 (clean, no slippage)
**Entry:** $55.14
**Realized:** **-$20.72** (5 × ($55.14 - $51))

## Why missed in morning audit

Checked `get_orders` at 09:45 ET autopilot but apparently filtered window didn't catch BSX (fired at 09:48 ET = 3 min after autopilot completed). Lesson: morning autopilot Phase 0 stop check should use a wider window OR re-check stop status mid-morning if intraday volatility appears.

## Why did BSX move -12% intraday?

BSX dropped from $57.66 → $50.42 (intraday low $50.045). Not investigated in real-time — already exited. Possible causes: medtech sector pullback contagion from cyber sleeve sell-the-news pattern, DXCM stolen-sensor narrative spread, or BSX-specific news not captured in Mercury queue (worth investigating tomorrow).

## Updated day realized

| Position | Stop | Filled | Realized |
|----------|------|--------|----------|
| ZS | $172 | $136.64 | -$132.57 |
| CRWD | $640 | $637.36 | +$27.88 |
| PANW | $245 | $243.67 | +$0.46 |
| **BSX** | **$51** | **$51** | **-$20.72** |
| MRVL trim | limit $199 | $200.18 | +$11.07 |
| **TOTAL** | | | **-$113.88** |
