---
title: "MRVL Harvest Pre-ER Trim — 2026-05-27"
date: 2026-05-27
---

# MRVL Harvest Pre-ER Trim — 2026-05-27 12:18 ET

**Action:** TRIM 25% (sell 1 of 5 sh, limit, GTC day)
**Limit price:** $199
**Filled price:** **$200.18** (price improvement)
**Order ID:** `9309d242-8437-4393-a7af-30be8025db0e`
**Entry:** $189.11
**Realized:** **+$11.07** (1 sh × $11.07)

## Trigger

Harvest playbook rule: "Pre-earnings trim within 7 days → Trim 25%". MRVL Q1 earnings AH today (Wed 5/27, ~16:30 ET).

## Setup justification

- Bull stack at 15+ data points (Citi/Wells/Stifel/HSBC + Wedbush PANW/CRWD/OKTA cluster + GS liquid cooling + DRAM ETF + MU $1T + SK Hynix $1T + Jensen $150B Taiwan)
- Bear-tail framing 4 data points ("can MRVL justify 130% rally?", "high bar", high-expectations baked in)
- Stop $195 cushion only 2.6% at trim time (intraday low was 1.4% at 11:18 ET)
- ZS template demonstrated same morning: $172 stop filled at $136.64 = -$133 actual vs my predicted -$26 (5x slippage)

## Risk asymmetry preserved

- 4 sh × upside exposure to bull print
- $195 stop floor on remaining 4 sh = +$23.56 floor (4 × $5.89/sh)
- 1 sh × +$11.07 locked NOW = max-downside protection
- Total realized + floor = +$34.63 minimum

## Stop adjustment

Previous stop (qty 5) replaced with qty 4 @ $195 — order ID `f3520c7b-efb6-4d25-a7a8-12c8ebc1c55f`

## Notes

Executed autonomously per autopilot midday Harvest authority. Operator did not respond to morning Tier-1 urgent ping recommending this exact trim. Pipeline discipline non-issue (Harvest trims don't require 5-agent fast-track, only new BUYs do).
