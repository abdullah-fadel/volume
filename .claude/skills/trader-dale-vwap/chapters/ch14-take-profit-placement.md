# Chapter 14: Take Profit Placement

## Core Idea
One universal rule governs all Take Profit placement — exit a bit before price reaches a barrier strong enough to reverse it — and the author offers four ways to locate that barrier: Price Action, VWAP, Volume Profile, or a fixed ATR-based percentage when you'd rather not track barriers at all.

## Frameworks Introduced
- **The universal Take Profit rule**: always exit a trade a little before it reaches a significant barrier (a strong Support/Resistance identified via Price Action, VWAP, or Volume Profile) that could stop or reverse the move.
  - When to use: applies not just to VWAP trading but to the author's Volume Profile, Order Flow, and pure Price Action trading as well — a general principle, not VWAP-specific.
  - How: identify the nearest strong barrier ahead of your position in the trade's direction → exit a few pips before price actually reaches it, rather than waiting to see if it holds or breaks.
- **Price Action based Take Profit**: exit before price reaches a Price Action support-becomes-resistance (or vice versa) level.
  - When to use: whenever a broken S/R level (Ch12) sits ahead of an open position.
  - How: identify the nearest old S/R level that has flipped role in the direction opposing your trade → close the trade a couple of pips before price reaches it.
- **VWAP based Take Profit**: exit before price reaches an opposing VWAP-based Support/Resistance — any anchor type (Ch3–Ch9) qualifies.
  - When to use: whenever a differently-anchored VWAP line (swing point, trend start, date-anchored, etc.) sits ahead of your position as a potential barrier — including the VWAP line itself as a target in the Rotation strategy (Ch10).
  - How: identify the nearest VWAP-based level ahead of your trade → exit a few pips before reaching it. Explicit warning: don't plot every possible VWAP/anchored-VWAP on one chart, or you'll see a "barrier" every few pips and exit prematurely — only track the strongest, most significant VWAP levels as TP candidates.
- **Volume Profile based Take Profit**: exit before price reaches a heavy-volume zone acting as Support/Resistance.
  - When to use: whenever a Volume-Profile-identified heavy volume zone sits ahead of an open position.
  - How: identify the nearest heavy volume zone in the trade's direction → exit a few pips before it, since even a barrier that doesn't fully reverse price tends to at least slow momentum into a sideways stall, which the author considers not worth waiting out.
- **ATR based Take Profit**: a fixed, barrier-independent Take Profit sized as a percentage of the instrument's average daily volatility.
  - When to use: when you'd rather use a consistent fixed target instead of tracking specific barriers — the author's fallback/alternative method.
  - How: set ATR to a long period (e.g., 200) on the Daily timeframe with 300–500 days of data loaded → read the average ATR value → multiply by 10,000 to express it in pips (average daily volatility) → for intraday trades, set Take Profit at 10–20% of that average daily ATR value.

## Key Concepts
- **Barrier**: any strong Support/Resistance level — from Price Action, VWAP, or Volume Profile — capable of stopping or reversing price; the shared concept underlying three of the four TP methods.
- **Exit-before-barrier margin**: consistently "a few pips" before the identified barrier, not at or beyond it — the buffer that protects against the barrier actually holding.
- **Chart clutter warning**: plotting too many VWAP anchors simultaneously creates false barriers everywhere, leading to premature exits — restrict to the strongest signals only.
- **ATR-derived volatility target**: average daily volatility (ATR × 10,000, in pips) as the base unit; intraday Take Profit = 10–20% of that value.

## Mental Models
- Think of all three barrier-based TP methods (Price Action, VWAP, Volume Profile) as the same underlying rule applied through three different lenses — pick whichever barrier type is nearest/strongest on a given chart, or combine them.
- Use ATR-based TP as the "no barrier available, or don't want to track one" fallback — a purely volatility-driven, mechanical alternative to the barrier-hunting methods.

## Anti-patterns
- **Waiting for a barrier to actually be hit (or broken) before exiting**: the entire framework is built around exiting *before* the barrier, not testing it — this is Quality Rule zero of Take Profit placement in this book.
- **Overplotting VWAP levels on one chart**: leads to seeing potential barriers every few pips and exiting positions far too early — restrict to the strongest, most significant VWAP levels.
- **Sitting through a stalled, sideways market waiting for a Volume-Profile barrier to fully reverse price**: the author explicitly prefers exiting at the point momentum slows into chop rather than tying up the trade for hours with no clear direction.

## Worked Example
A Long trade entered on a reaction to a VWAP anchored at a significant swing low: price rallies, and as it climbs, a second VWAP — this one anchored at the candle marking the start of a strong prior trend — comes into view ahead of the position. Rather than holding for that second VWAP to be tested and potentially rejected, the trade is closed as price approaches this VWAP-based Resistance, a few pips before actually reaching it. The logic mirrors the author's broader Take Profit rule: two independently-anchored VWAP lines don't need to be the same type of barrier (Price Action vs. VWAP vs. Volume Profile) to apply the rule — any sufficiently strong barrier, VWAP-based or otherwise, is worth exiting ahead of.

## Key Takeaways
1. Universal rule: exit a few pips before any strong barrier (Price Action, VWAP, or Volume Profile), not at or after it.
2. Three barrier types to scan for ahead of an open position: Price Action support-becomes-resistance flips, other VWAP-anchored lines, and Volume Profile heavy volume zones.
3. Don't overplot VWAP anchors — restrict TP-barrier hunting to the strongest, most significant levels to avoid exiting on noise.
4. ATR-based TP is the fixed-target fallback: 10–20% of average daily ATR (in pips) for intraday trades.
5. Even a barrier that only slows momentum (rather than reversing price outright) is often worth exiting at, rather than waiting out a sideways stall.

## Connects To
- **Ch12**: the Price-Action-based TP method directly reuses the support-becomes-resistance confluence framework.
- **Ch3–Ch9**: any VWAP anchor type can supply the barrier for VWAP-based TP.
- **Ch15**: Stop Loss placement mirrors this chapter's four-method structure (Price Action / VWAP / Volume Profile / ATR), applied to the opposite side of the trade.
