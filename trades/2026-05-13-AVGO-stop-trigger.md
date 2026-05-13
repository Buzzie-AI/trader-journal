# AVGO Stop Trigger — 2026-05-13

**Order ID:** 4fc21eca-db04-4307-b2e2-8493c13287b4
**Client order ID:** autopilot_20260511_AVGO_stop_loss_gtc_407
**Stop:** $407.00 GTC (placed Mon 5/11 EOD as bracket-replacement; survived 0.45% cushion stress test Tue 12:42 ET)
**Fill:** 1 share @ $407.00 exact
**Fill time:** 2026-05-13 09:46:40 ET (13:46:40 UTC)

## P&L

| Metric | Value |
|--------|-------|
| Entry (5/11 catalyst-buy AM) | 1 sh @ $431.40 |
| Stop trigger today | -1 sh @ $407.00 = **-$24.40 / -5.66% realized loss** |
| Hold duration | ~2 trading days (5/11 fill 09:57 ET → 5/13 stop 09:46 ET) |

## Context

- **Catalyst-buy** entered Mon 5/11 09:57 ET on Mercury alert: AVGO record $35B private credit (Apollo+Blackstone) — Mercury score 91, top of 23 alerts
- Tue 5/12 stress test: cushion hit 0.45% intraday low at 12:42 ET, recovered to 2.43% close
- Wed 5/13 open: stop $407 triggered ~16 min after market open on weak semi-sector tape (despite MRVL/MU/TXN exploding on memory thesis — AVGO underperformed)
- AVGO closing $417.15 yesterday → $407 today = sub-$10 gap-down + intraday weakness through stop
- Citi $500 PT raise yesterday (Tue 11:35 ET poll alert) FAILED to lift tape — broader catalyst-rejection pattern continues

## Detection Latency — Remediation Working ✓

- AVGO stop fired 09:46:40 ET
- Position-diff check at 09:51 ET detected missing position (~5 min latency)
- Compared to yesterday's INTC: 1h11min latency
- **Position-diff check in mercury cron is materially reducing detection lag**

## Sleeve State Post-AVGO

Tech concentration drop:
- Before: 36% (over 35% ceiling)
- After AVGO exit: tech bucket drops by ~$417 → ~35.0% (right at ceiling)
- Some room may open for tech adds depending on intraday valuation moves

Semi sleeve survivors:
- MU: $788.91, +45.8% cumulative ($743 unrealized); stop $700, cushion 11.3%
- MRVL: $175.90, +10.3% cumulative ($147 unrealized); stop $145, cushion 17.6%
- TXN: $306.20, +12.2% cumulative ($167 unrealized); stop $252.58, cushion 17.5%
- AMAT: $426.59, -3.4% cumulative ($-14.88 unrealized); stop $416, cushion **2.5%** (still YELLOW)

## Lessons

- 2nd catalyst-buy loss from Mon's mass-entry day (NKE also stopped Mon at -$122; AVGO today -$24)
- AVGO entry timed at mid-day after AVGO had already moved on $35B credit news — entered into momentum that didn't sustain
- Mon's daily-cap-2 entries (AVGO + AMAT) both went on to stop pressure within 48h
- AMAT still alive but only 2.5% cushion — same setup risk profile as AVGO

**Process update:** position-diff check is now mandatory in every mercury cron, validated through 2 fills (INTC yesterday, AVGO today). Detection latency cut from hours to single-digit minutes.
