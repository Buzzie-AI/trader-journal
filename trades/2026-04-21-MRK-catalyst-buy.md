# Trade: MRK Buy — Autopilot Midday 2026-04-21

**Strategy:** catalyst-buy (dual-catalyst under-reaction)
**Source:** autopilot_midday cron fire at 13:17 ET

## Catalyst

Two confirmed positive catalysts on MRK in a single pre-market + market-open window:

1. **06:52 ET:** Merck Phase 3 LITESPARK-012 trial results — belzutifan combination regimen in renal cell carcinoma (oncology pipeline advance)
2. **11:56 ET:** FDA approves Merck's IDVYNSO for HIV-1 infection treatment in adults (new revenue-generating approval)

## Price Action — the under-reaction

- Yesterday close: $117.07
- At autopilot run (13:17 ET): $112.46 = **-3.94% intraday**
- Expected category impact (dual FDA/Phase-3 on mega-cap pharma): +2 to +5% combined
- **Under-reaction gap: ~6-9%** = strong dip-buy setup

Price drop possibly driven by broader pharma profit-taking (vaccine-panel ruling was politically complicating, GLP-1 competitive-threat weighing on the sector). MRK itself has no bearish news today.

## Pipeline (abbreviated)

- **Iris (news):** 2 concrete positive catalysts, no negative MRK-specific news
- **Grace (fundamental):** MRK mega-cap ~$280B, diversified franchise, Keytruda still dominant, HIV addition extends the bench beyond late-decade Keytruda patent cliff
- **Atlas (event study):** Mega-pharma typical reaction to dual FDA/Phase-3 day: +2-5% same-day. MRK -4% = atypical under-reaction
- **Victor (risk):** Risk = broader pharma rotation continues overnight. Stop $103.50 = -8% from entry = ~$160 max loss. Position 9.5% of portfolio — at concentration limit
- **Diana (decision):** BUY 18 sh @ $112.50 limit, stop $103.50, target $125 (+11.1%, +1.4R)

## Safety gates

| Gate | Value | Status |
|------|-------|--------|
| Daily trade cap (2) | 2 used (NFLX sell + MRK buy) | ✓ at limit |
| Daily spend ($4K) | $2,024 | ✓ |
| Max position (10%) | $2,024 / $21,404 = 9.45% | ✓ |
| Min cash reserve ($2K) | $4,561 after | ✓ |
| Circuit breaker (-8%) | -1.15% day | ✓ |
| Limit order | Yes ($112.50) | ✓ |
| Stop-loss | **PDT blocked** same-day, deferred to tomorrow morning | ⚠ deferred |

## Execution

- Order ID: `95e352a0-de9c-4a08-b088-d27777cb0389`
- Client ID: `autopilot_20260421_MRK_catalyst_buy`
- Type: limit buy 18 sh @ $112.50 day-TIF
- **FILLED instantly at $112.4669** (total cost $2,024.40, under limit)
- Stop order rejected by Alpaca with 403 code 40310000: "no day trades permitted based on your previous day account equity being under $25,000"
- Same PDT pattern as AEM yesterday — stop will be placed by tomorrow's 9:23 AM autopilot Phase 0 (AEM stop was placed today successfully using that pattern)

## Plan

- Entry: $112.4669 (filled)
- Stop: **$103.50 (pending tomorrow)** — ~-8% from entry
- Target: $125 (+11.1% from entry, +1.4R)
- Horizon: 20-60 days (pharma catalyst absorption + HIV franchise ramp)
- Exit triggers: stop hit, target hit, broader pharma sector rotation, or MRK-specific thesis-break (FDA reversal, efficacy concerns)

## Tomorrow's Autopilot Action

1. Place MRK stop $103.50 GTC (mirror AEM pattern)
2. Confirm stop on AEM still at $200 GTC
3. Re-evaluate MRK if price moves >±5% overnight

## Post-Trade Portfolio

- Cash: $6,585 → $4,561
- Positions: 10 (was 11 yesterday, +AEM -NFLX -MU, net same), MRK new
- Current MRK P&L at 13:19 ET: position +/- within a few cents of fill
