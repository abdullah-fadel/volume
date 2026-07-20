# Chapter 5: Anchoring VWAP to Start of the Trend

## Core Idea
Anchoring VWAP at the large candle that kicks off a new trend captures two simultaneous order-flow forces at the "fair price" — traders wanting to join the trend, and traders trapped on the wrong side wanting to exit — which is why this anchor tends to produce especially reliable support/resistance reactions.

## Frameworks Introduced
- **Trend-start-anchored VWAP**: VWAP calculated from the large, decisive candle that marks the beginning of a new trend.
  - When to use: any instrument/timeframe once a strong trend has begun (forex, indices, stocks, crypto — the author demonstrates all four); most useful when you can clearly identify a single dominant candle that kicked off the move.
  - How: locate the largest, most decisive candle near where the new trend began → anchor VWAP there → trade pullback reactions to it as continuation entries in the trend direction (short below a downtrend-start VWAP, long above an uptrend-start VWAP) → treat a break-and-flip of this VWAP (price crossing to the other side) as a signal the trend may be exhausting, and re-orient to the new side.
  - Why it works (two combined order-flow sources at the touch): (1) traders wanting to join the trend enter at what they consider the "fair price," reinforcing the move; (2) traders caught on the wrong side of the trend (short into an uptrend, or long into a downtrend) use that same VWAP touch as their preferred fair-price exit point — and because closing a losing short means buying (and closing a losing long means selling), their exits mechanically push price in the same direction as the new entrants.

## Key Concepts
- **Trend-start candle**: the author's chosen anchor — a large, visually obvious candle near the point where the trend began; bigger candles are weighted as more significant anchors.
- **Anchor subjectivity**: two traders may reasonably choose slightly different candles as the trend start; minor differences in anchor choice usually don't matter much, but anchoring to candles that are too far apart can produce meaningfully divergent VWAP lines.
- **Dual exit/entry pressure**: the mechanism unique to this anchor — both new trend-followers and trapped traders push price the same direction at a touch, because closing a losing position requires the opposite-direction order (short-covering = buying; long-liquidation = selling).
- **Trend-start VWAP flip**: when price crosses through a trend-start VWAP to the other side, the line's role flips (Support→Resistance or vice versa) — treated as a warning the original trend may be ending.

## Mental Models
- Think of the trend-start VWAP touch as attracting two crowds at once — new joiners and trapped exiters — both transacting in the same direction, which is why this particular anchor tends to produce unusually decisive reactions.
- If price breaks through a trend-start VWAP and it flips role, treat that as an early signal the trend's dominant side has lost control, not just a random overshoot.

## Anti-patterns
- **Anchoring to a small, ambiguous candle near the trend start**: the author explicitly weights bigger, more decisive candles as more significant anchors — a weak or unclear candle produces a less reliable line.
- **Ignoring a VWAP flip after a trend-start anchor**: when the line breaks and flips, the underlying trend that justified the anchor may already be over — continuing to trade the old bias into the new side is a mistake.
- **Assuming every trend-start anchor produces a lasting trend**: the Bitcoin example shows a strong-looking trend-start candle followed by an uptrend that failed quickly — the anchor method identifies a meaningful starting point, not a guarantee the trend will persist.

## Worked Example
Bitcoin, 5-minute chart: a massive green candle marks what looks like the start of a powerful uptrend. Anchoring VWAP there gives one good long entry on the first pullback — driven by both new buyers entering at "fair price" and trapped short-sellers covering (buying) to exit. But the uptrend fails shortly after: price breaks back below the VWAP, flipping it from Support into Resistance. At that new Resistance, the same dual mechanism now works in reverse — sellers wanting to sell at "fair price" combine with trapped longs liquidating (selling) to exit, producing two clean short opportunities off the flipped line. The lesson the author draws: the anchor mechanism (dual entry/exit pressure at VWAP) works reliably in both directions, even when the original trend it was anchored to doesn't survive.

## Key Takeaways
1. Anchor at the largest, most decisive candle near the trend's actual start — bigger candles carry more weight as anchors.
2. The reaction strength at this anchor comes from two combined forces: new trend-joiners plus trapped-trader exits, both transacting in the same direction at the touch.
3. Minor differences in anchor-candle choice between traders usually don't matter; anchors chosen too far apart can diverge meaningfully.
4. A flip of this VWAP (price crossing to the other side) is a signal the trend may be ending — re-orient your bias rather than fighting the flip.
5. Works across all instruments and timeframes (forex, indices, stocks, crypto) — the mechanism is universal.

## Connects To
- **Ch4**: closely related — a trend often begins right at a significant swing point, so these two anchor types frequently overlap.
- **Ch3**: the "broken/flipped VWAP" role-reversal mechanic first introduced there recurs here in the trend-start context.
- **Ch12**: trend-start anchoring pairs naturally with the Volume Profile Trend setup, since both key off volume behavior within an established trend.
