# Chapter 15: Stop Loss Placement

## Core Idea
Stop Loss always goes BEHIND a barrier (Price Action, VWAP, or Volume Profile) — a zone price shouldn't cross without signaling the trade thesis is wrong — with the strongest, most reliable placements combining two or more barrier types at once, and ATR-based sizing as the fallback when no clean barrier exists.

## Frameworks Introduced
- **The universal Stop Loss rule**: position Stop Loss behind a barrier (a Support/Resistance zone from Price Action, VWAP, or Volume Profile analysis) — if the barrier is breached, the trend/setup thesis is likely wrong and it's time to exit.
  - When to use: every trade, as the starting principle before choosing which specific barrier type to use.
  - How: identify the nearest structurally significant barrier just beyond your entry, opposite your trade direction → place SL just past it, treating a breach as a safety-net trigger, not just a probability shift.
- **Price Action based Stop Loss placement**: SL at a swing point or significant high/low.
  - When to use: whenever a clear swing point/prior high-low sits just beyond your entry.
  - How: identify the nearest swing point or significant high/low against your position → place SL beyond it → in multi-entry VWAP Trend setups, each successive short/long can get its own SL at its own nearest prior high/low.
- **VWAP based Stop Loss placement**: SL behind the VWAP line, a deviation, or another anchored VWAP, adjusted as price advances.
  - When to use: whenever VWAP or its deviations are acting as the relevant barrier — includes progressively moving SL to a "closer" VWAP-family level as a trade develops.
  - How: place initial SL below/above the VWAP line or a deviation → as price moves favorably and the original VWAP grows too far away to be a useful barrier, migrate SL forward to whichever VWAP-family level (a different deviation, a different anchored VWAP) is now closest and still valid → in a VWAP Trend setup, anchor a fresh VWAP at the start of the new trend and use it as an ongoing barrier — if price crosses back through this fresh anchor, exit, since it signals the driving pressure has subsided.
- **Volume Profile based Stop Loss placement**: SL behind a heavy volume zone.
  - When to use: whenever a heavy volume zone (identified via Volume Profile) sits just beyond your entry.
  - How: identify the nearest heavy volume zone against your position → place SL just beyond it → treat a breach of the zone as a sign the opposing side has taken control.
- **Stop Loss placement — combined barriers**: place SL behind two or more overlapping barrier types (e.g., heavy volume zone + swing point, or heavy volume zone + VWAP) for the strongest possible protection.
  - When to use: whenever multiple barrier types align near the same area — the author's preferred SL placement when available.
  - How: identify overlapping barriers (e.g., a heavy volume zone with a swing point positioned just past it) → place SL beyond the combined zone → balance strength against distance: don't place SL unreasonably far away chasing a "super strong" combined barrier if it would sacrifice too much of a trailed trade's open profit — a weaker but closer barrier is preferable in that case.
- **ATR based Stop Loss**: a fixed SL sized as a percentage of average daily volatility, reusing the Ch14 ATR calculation method.
  - When to use: as an alternative to barrier-based placement generally, or specifically when no Price-Action, VWAP, or Volume-Profile barrier is available nearby.
  - How: reuse the ATR-derived average daily volatility (Ch14) → for intraday trades, size SL at roughly 10–20% of that value.

## Key Concepts
- **Barrier (for SL purposes)**: a zone price should not cross if the trade thesis remains valid; breaching it is the safety-net trigger to exit.
- **Combined barrier**: two or more independent barrier types (e.g., Volume Profile heavy zone + Price Action swing point) overlapping in the same area — considered the strongest possible SL location.
- **SL migration**: progressively moving Stop Loss forward through a sequence of VWAP-family levels (lower deviation → date-anchored VWAP → upper deviation) as a trade develops and earlier barriers become too distant to be useful.
- **Distance-vs-strength trade-off**: a stronger, farther barrier isn't automatically better than a weaker, closer one — especially when trailing a trade, since an overly distant SL can give back too much open profit if price reverses.

## Mental Models
- Default to combined barriers when available (strongest option); fall back to a single barrier type (Price Action, VWAP, or Volume Profile) matched to whatever structure is present; fall back further to ATR sizing only when no barrier exists at all.
- Treat SL migration through a developing VWAP Trend setup as an evolving barrier chain, not a single fixed decision — the "right" SL level changes as the trade matures.

## Anti-patterns
- **Leaving SL behind an increasingly distant original barrier**: as price moves favorably, an original VWAP or swing-point SL can become too far away to be meaningful — the author explicitly recommends migrating to closer valid barriers instead of leaving SL static indefinitely.
- **Chasing the strongest possible combined barrier regardless of distance**: sacrificing too much trailed profit to reach a marginally "stronger" but much farther barrier is discouraged — use a closer, weaker barrier instead when trailing.
- **Placing SL with no barrier logic at all**: even the ATR fallback is explicitly framed as a substitute for barrier analysis, used only when no Price Action/VWAP/Volume Profile structure is available — not a default-first choice.

## Worked Example
A Long trade entered on a pullback to a VWAP anchored at an important swing low: initial Stop Loss goes below that anchored VWAP line. As price rallies, a second VWAP — a Weekly VWAP with deviations — is also on the chart. The SL is migrated forward in stages as the trade develops: first below the lower deviation of the Weekly VWAP, then below the Weekly VWAP line itself as price climbs further, then below the upper deviation as the rally extends further still. Eventually, this final SL level is hit, closing out what the author calls a successful trade overall — the migration captured a large portion of the move by continuously trading up the barrier chain rather than leaving the original swing-low VWAP as a static, increasingly-irrelevant Stop Loss.

## Key Takeaways
1. Universal rule: SL always goes behind a barrier — Price Action, VWAP, or Volume Profile — never placed arbitrarily.
2. Combined barriers (two+ overlapping barrier types) are the strongest SL placement; use single-barrier or ATR-based sizing when combined barriers aren't available.
3. Migrate SL forward through a chain of valid VWAP-family levels as a trend develops, rather than anchoring to one increasingly distant original level.
4. When trailing, prefer a closer/weaker barrier over a farther/stronger one to protect accumulated open profit.
5. ATR-based SL (10–20% of average daily volatility, intraday) is the fallback for when no structural barrier is available.

## Connects To
- **Ch14**: mirrors the same four-method structure (Price Action / VWAP / Volume Profile / ATR), applied to the protective side of the trade rather than the target side; reuses the same ATR calculation.
- **Ch13**: the Reaction Point established during confirmed-reaction entries is a direct instance of Price-Action-based SL placement.
- **Ch16**: SL migration through developing VWAP-family levels is the mechanical foundation for the trailing techniques covered next.
