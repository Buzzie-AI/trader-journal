# INTC Stop Trigger — 2026-05-12

**Order ID:** 3b177ec3-c977-4386-b233-700a69be79d0
**Client order ID:** harvest_20260508_INTC_stop_ratchet_120_eod
**Stop:** $120.00 GTC (ratcheted Fri 5/8 EOD from $118 after WSJ Apple-Intel deal day)
**Fill:** 6 shares @ $120.01 avg
**Fill time:** 2026-05-12 10:31:18 ET (14:31:18 UTC)

## P&L

| Metric | Value |
|--------|-------|
| Entry (5/4 sleeve catalyst-buy) | 12 sh @ $96.8499 |
| Trim 5/8 (50% target) | -6 sh @ $116.3745 → +$117.15 realized |
| Stop trigger today | -6 sh @ $120.01 → **+$138.97 realized** |
| **Total realized** | **+$256.12 / +44.1% on 12-share basis** |

## Context

- INTC traded $124.37 open → $116.00 day low → $117.43 last (at time of detection)
- Stop $120 GTC trailing from Fri 5/8 (AAPL foundry deal) caught the breach precisely
- Sector was risk-off all morning (XLK -1.57% intraday) → semi sleeve under pressure
- Reaper flagged INTC at YELLOW++ in 09:58 autopilot (3.3% cushion) — stop did its job

## Detection Gap (Process Issue)

**Stop fired 10:31 ET; I did not detect the absent position until 11:42 ET while checking AVGO/AMAT pressure** — 1h11min latency. Same monitoring lapse pattern as 5/11 CEG/NKE stops.

**Remediation:** Add an explicit position-diff check (snapshot positions, compare to last-known list) to the mercury_stream_market cron. If a previously held ticker disappears from `get_all_positions`, immediately log + alert via Tier-1 ping. This is a free check on each fire and would have caught this in minutes, not hours.

## Lessons

- Stop ratchet from $118→$120 on 5/8 was the right call — locked +24% on the back half after AAPL deal had already paid +20% on the front half (target trim @ $116.37)
- Total INTC trade across the lifecycle: +$256.12 realized = +44% on initial $581 cost basis. Textbook 5/4 catalyst-buy → 5/8 target trim → 5/12 stop close.
- Position monitoring at the cron level needs to look at both queue AND position state — not just news flow.
