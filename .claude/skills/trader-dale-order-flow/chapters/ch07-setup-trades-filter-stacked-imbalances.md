# Chapter 7: Trading Setups — Trades Filter & Stacked Imbalances

## Core Idea
Trading Setups #3 (Trades Filter) and #4 (Stacked Imbalances) locate the same kind of institutional defense zone as Chapter 6, but by isolating unusually large single orders and one-sided aggression bursts instead of shaded volume or stacked HVNs.

## Frameworks Introduced
- **Trading Setup #3: Trades Filter**: trade the pullback into a zone previously marked by an unusually large single order.
  - When to use: standalone, or layered with a confirmation setup for extra conviction (Ch 9–10).
  - How:
    1. Switch cell content to Bid x Ask and enable Trades Filter at an instrument-appropriate threshold (author uses 25 lots on EUR Futures / 6E; ES needs ~300+; tune per instrument/session, targeting roughly 5–10 signals/day).
    2. Look for a non-zero highlighted value on the Trades Filter — a big single order that acted as Support/Resistance.
    3. Confirm price has moved away (1–2 full footprints above/below) — 30-minute footprint preferred.
    4. Wait for a pullback into that big-order zone.
    5. Enter: hit from above → Long; hit from below → Short. (Green/red highlighting does not itself dictate direction.)
    6. First touch only — don't re-trade the same level.
- **Trading Setup #4: Stacked Imbalances**: trade the pullback into a zone with three or more same-direction Imbalances stacked vertically.
  - When to use: best sought within a trend or just before one begins; doesn't require a strong trend, just a clear one-way move.
  - How:
    1. Switch to Bid x Ask cell content with Imbalances enabled (default trigger: 300% diagonal dominance).
    2. Identify a Stacked Imbalance (3+ imbalances on top of each other) — software auto-highlights Support (green, from stacked Buying Imbalances) or Resistance (red, from stacked Selling Imbalances).
    3. Confirm price has moved away (1–2 full footprints above/below) — 30-minute footprint preferred.
    4. Wait for a pullback into the highlighted zone.
    5. Enter: hit from above → Long; hit from below → Short. Red highlight = Resistance, green highlight = Support (this labeling *does* map directly, unlike the Trades Filter's color).
    6. First touch only.

## Key Concepts
- **Trades Filter threshold**: an instrument- and session-specific lot-size cutoff below which fills are hidden; the goal is roughly 5–10 clean signals per day, not a fixed universal number.
- **Iceberg order (recap)**: split institutional entries the Trades Filter cannot catch — a structural limitation of Setup #3, since it only reveals large *single*-order fills.
- **Buying Imbalance**: Ask ≥ 300% of the diagonally-opposite Bid; shown in blue on the Ask.
- **Selling Imbalance**: Bid ≥ 300% of the diagonally-opposite Ask; shown in blue on the Bid.
- **Stacked Imbalance**: 3+ same-direction Imbalances vertically adjacent; default trigger is user-adjustable in the software.

## Mental Models
- Both setups are really the same "big-order-zone pullback" template from Ch 6, applied with a different detector: Trades Filter finds a single unusually large order, Stacked Imbalances find a run of one-sided aggression. Recognizing the shared template makes it easier to combine or compare signals across setups.
- **Why it works**: a 300%+ one-sided imbalance is a statistically unusual event by itself; three or more stacked together is strong evidence that one side deliberately dominated that price — not random noise — which is why the zone tends to attract a defensive reaction on retest.
- **Failure mode**: assuming the highlight color (green/red) always maps directly to trade direction. It does for Stacked Imbalances (green=Support, red=Resistance) but not for the Trades Filter, where color reflects the buy/sell side of that one order, not automatically the correct trade direction — direction there is set purely by "hit from above vs. below."

## Anti-patterns
- **Copy-pasting the 25-lot Trades Filter threshold across instruments**: ES alone needs roughly 10x that size; using one instrument's calibration on another produces either too much noise or almost no signals.
- **Trading a Trades Filter or Stacked Imbalance zone on a second retest**: both setups explicitly restrict entries to the first touch, since the probability of a second successful reaction drops.
- **Expecting the Trades Filter to catch every large institutional order**: Iceberg-split entries stay invisible to it by design.

## Worked Example
**Trades Filter zone (EUR Futures / 6E, 25-lot threshold):** The author sets the filter so only single fills of 25+ contracts remain visible on the chart. When such a large fill appears and price subsequently moves away, forming clean footprints on one side, that filtered print becomes a marked zone. On the next pullback into that exact print, the author enters in the direction implied by "hit from above vs. below" (not by the fill's own color) — e.g., a large filtered buy order that price later pulls back down into would still be traded Long only if that pullback approaches from above the level, consistent with the setup's mechanical entry rule rather than the print's own color.

## Key Takeaways
1. Both setups follow the same "confirm move-away → wait for pullback → enter on defense" mechanics used throughout the book's trading setups.
2. Trades Filter threshold must be tuned per instrument and session (25 lots ≈ EUR Futures baseline; ES needs far more) — aim for ~5–10 signals/day.
3. Trades Filter cannot see Iceberg-split institutional orders — it only reveals large single fills.
4. Stacked Imbalances need 3+ same-direction 300% imbalances; green highlight = Support, red = Resistance.
5. Both are first-touch-only setups — don't re-trade a level that's already reacted once.

## Connects To
- **Ch 4**: Special Features defines the Trades Filter and Imbalance/Stacked Imbalance mechanics used here.
- **Ch 6**: Trading Setup #1/#2 share this chapter's pullback-into-a-defended-zone template with different zone detection.
- **Ch 11**: Stop Loss placement can use a "low volume area behind a heavy volume area" logic that pairs naturally with either setup here.
