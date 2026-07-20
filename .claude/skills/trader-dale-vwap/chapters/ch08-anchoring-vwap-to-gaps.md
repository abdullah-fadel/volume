# Chapter 8: Anchoring VWAP to Gaps

## Core Idea
A large price gap — most common in stocks, since they don't trade 24/5 like forex — is a natural VWAP anchor point because it draws every trader's attention to "how am I doing relative to the fair price since the gap," making the first post-gap candle a strong anchor.

## Frameworks Introduced
- **Gap-anchored VWAP**: VWAP calculated starting from the first candle after a significant price gap (the opening candle following the gap).
  - When to use: primarily stocks (gaps are rare in continuously-traded forex); works on intraday (5–30 min) or daily/position timeframes.
  - How: scan charts for big gaps (a meaningful difference between one candle's close and the next candle's open) → anchor VWAP at the first candle after the gap → trade pullbacks to that VWAP line using the same base approach as every other anchor type (Ch2) — long if price holds above and pulls back down to it, short if price holds below and pulls back up to it, with a role-flip (Support↔Resistance) if price crosses to the other side.
  - Why it works: a big gap is a shared reference moment — traders assess their trade's performance against the "fair price established after the significant gap," making that post-gap VWAP a genuine behavioral anchor rather than an arbitrary technical line.

## Key Concepts
- **Gap**: a difference between one candle's closing price and the next candle's opening price; structurally more common in stocks (non-continuous trading hours) than in currencies.
- **First candle after the gap**: the specific anchor point — not the pre-gap candle, and not an arbitrary candle within the post-gap move.
- **"Big" gap requirement**: the strategy is explicitly for significant gaps that draw broad trader attention, not minor/routine overnight gaps.

## Mental Models
- Treat a big gap the same way you'd treat a game-changing news event (Ch6) — a moment that resets what "fair price" means for the instrument going forward.

## Anti-patterns
- **Applying this to forex majors as a primary anchor**: gaps are structurally rare in continuously-traded currency pairs, making this a stock-focused technique first.
- **Anchoring to small/routine gaps**: the technique depends on the gap being large enough to be a genuine shared reference point for other traders — minor gaps don't carry the same weight.

## Worked Example
Procter & Gamble, 5-minute chart: the stock opens with a significant gap to the upside, which would suggest bullish continuation. But sellers quickly take control and push price below the VWAP anchored to the first post-gap candle, flipping that VWAP from what might have been expected support into resistance. The gap was large enough that price goes on to react to this now-resistance VWAP multiple times, producing several short opportunities — illustrating that the gap's direction doesn't dictate which side ultimately controls the post-gap VWAP; the anchor is valuable regardless of which way it resolves.

## Key Takeaways
1. Anchor at the first candle after a big gap — not before it, not partway into the subsequent move.
2. This is primarily a stock technique because gaps require non-continuous trading hours to form meaningfully.
3. Works on both intraday (5–30 min) and daily/position timeframes.
4. Same base pullback/role-flip mechanics as every other VWAP anchor apply once the anchor is set.

## Connects To
- **Ch9**: earnings-driven gaps are the single most common and significant source of the large gaps this chapter targets — the two anchoring methods are closely linked.
- **Ch2**: base pullback-to-VWAP mechanics apply identically once the gap anchor is set.
- **Ch3**: the Support/Resistance role-flip mechanic recurs here exactly as with calendar-anchored VWAP.
