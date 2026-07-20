# Patterns — Trader Dale Order Flow

Concrete, tradable techniques from the book. Every pattern below routes through the shared "confirm move-away → wait for pullback → enter on defense" template unless noted otherwise.

## Volume Clusters (Trend / Rejection)
**When to use**: standalone; institutional heavy-volume area formed within a trend or a strong rejection.
**How**: set cell content to Volume. Find a dark (heavy-volume) area in a trend or rejection. Confirm price left it by 1–2 full footprints. Wait for pullback into the cluster; enter at its start/heaviest point, direction set by the trend/rejection direction.
**Trade-offs**: Volume-only, so works on Forex too. Misses which side (Buyers/Sellers) built the volume — direction relies on trend/rejection context, not the cluster itself.

## Multiple Nodes
**When to use**: standalone; 2+ consecutive footprint HVNs stacked at the same price, found before/within a trend or in a rejection.
**How**: cell content Volume (Bid x Ask optional), 30-min preferred. Confirm 2 full footprints beyond the node. Wait for the first pullback only; if price hits the node from above, go Long; if it hits from below, go Short.
**Trade-offs**: First-touch-only — no re-trading a level that's already reacted once.

## Trades Filter
**When to use**: standalone; pullback into a previously-marked unusually large single order.
**How**: Bid x Ask cell content, Trades Filter on (25 lots EUR Futures/6E baseline; ~300+ for ES; tune to ~5–10 signals/day). Confirm move-away, wait for pullback, enter on defense (direction = hit-from-above/below, not fill color). First touch only.
**Trade-offs**: Cannot see Iceberg-split institutional orders. Threshold must be recalibrated per instrument/session.

## Stacked Imbalances
**When to use**: standalone; 3+ same-direction 300%-diagonal Imbalances stacked vertically, best within or just before a trend.
**How**: Bid x Ask with Imbalances on. Confirm move-away, wait for pullback into highlighted zone (green=Support, red=Resistance — color *does* map to zone type here). Enter on defense, first touch only.
**Trade-offs**: Requires a genuinely one-sided move; doesn't need a strong trend, just clear directional aggression.

## Unfinished Business (Decision Aid — not standalone)
**When to use**: to refine TP, SL, trend-confirmation, and entry-screening decisions from another setup.
**How**: an improperly formed high/low (opposite side never hit 0 contracts) behaves like a magnet. (1) TP: hold a bit longer if a marker sits just ahead. (2) SL: don't place it just short of a marker — price tends to run through to fix it. (3) Confirmation: a pullback against you with a marker beyond in your favor is likely just a pullback. (4) Warning: don't enter Long with a marker below, or Short with one above.
**Trade-offs**: No guarantee distant markers ever get tested — never use as a standalone entry trigger.

## Confirmation #1: Big Limit Orders
**When to use**: at a pre-identified S/R zone, as final entry conviction.
**How**: 5-min Bid x Ask. Watch for an unusually large passive fill right at the zone — Limit Sell on Ask confirms Resistance/Short; Limit Buy on Bid confirms Support/Long. May build over a few minutes.
**Trade-offs**: "Unusually large" is instrument/session-relative, not a fixed number.

## Confirmation #2: Absorption
**When to use**: at a pre-identified S/R zone; simpler alternative to Confirmation #1.
**How**: 5-min or 30-min chart. Watch for heavy volume on *both* Bid and Ask at once while price stalls — one side is absorbing the other's pressure. Compare against recent average cell volume to judge "heavy."
**Trade-offs**: Can take several minutes to fully form; entering too early risks a partial/false read.

## Confirmation #3: Aggressive Orders and Delta
**When to use**: at a pre-identified S/R zone; fastest, most visual confirmation.
**How**: 5-min Bid x Ask. At Resistance, want Bid-side volume/negative Delta; at Support, want Ask-side volume/positive Delta.
**Trade-offs**: Strongest when stacked right after Confirmation #1 or #2 ("snowball effect") — used alone it's a weaker, faster read.

## Confirmation #4: Cumulative Delta Divergence
**When to use**: at a pre-identified S/R zone, as a confirmation only (not standalone, despite some traders using it that way).
**How**: 1-min price chart stacked over 1-min Cumulative Delta line. Short confirmation: price up, Cum. Delta down. Long confirmation: price down, Cum. Delta up.
**Trade-offs**: Popular for simplicity/reliability, but loses its edge when read away from a marked zone.

## Volume-Based Take Profit
**When to use**: default TP for any trade, Futures or Forex.
**How**: 30-min footprint. Close the position slightly *before* the next heavy-volume zone in your direction, not at it. If the nearest zone is too close for a decent RRR, skip the trade or target the next zone out.
**Trade-offs**: Requires having already mapped nearby heavy-volume zones (Ch 4, Ch 6).

## Trailing Take Profit
**When to use**: once already in profit with continued momentum.
**How**: 5-min Bid x Ask. Keep trailing while Imbalances continue to favor your side. Stop trailing immediately if any of the four confirmation signals fires against you, especially near a zone.
**Trade-offs**: Requires active monitoring; not a "set and forget" trail.

## Stop Loss Placement (3 methods)
**When to use**: every trade needs one.
**How**: (1) Fixed SL — same distance every trade. (2) High/Low of the S/R zone being traded. (3) Low-volume area just behind a heavy-volume zone — a push past the heavy zone signals real momentum against the trade. All three: size to roughly 10–20% of ATR-measured average daily volatility.
**Trade-offs**: Fixed SL is simple but ignores conditions; methods 2–3 adapt but aren't always available for every trade setup.

## Volume Accumulation Setup (Volume Profile)
**When to use**: the author's favorite; a rotation/tight channel immediately followed by a strong trend.
**How**: apply Volume Profile to the rotation to find the heaviest-volume zone (candidate S/R). On pullback, use an Order Flow confirmation (Ch 9–10) before entering.
**Trade-offs**: Requires patience to wait for both the initiating rotation and the later pullback.

## Trend Setup (Volume Profile)
**When to use**: a strong trend that briefly pauses and accumulates a Volume Cluster "bump."
**How**: apply Volume Profile across the trend to find the bump; on pullback into it, confirm with Order Flow before entering.
**Trade-offs**: Needs a clearly established trend first; not usable in choppy/rotational conditions.

## Rejection Setup (Volume Profile)
**When to use**: a strong, aggressive rejection of higher or lower prices (candle pattern irrelevant).
**How**: apply Flexible Volume Profile within the rejection itself to find the heaviest-volume zone (the "biggest fight"). On pullback, confirm with Order Flow before entering. Rejection of highs → Short; rejection of lows → Long.
**Trade-offs**: Explicitly the hardest of the three Volume Profile setups — judging rejection strength and reading volume distribution within it takes practice.
