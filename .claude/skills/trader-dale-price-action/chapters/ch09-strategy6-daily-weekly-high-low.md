# Chapter 9: Strategy 6 — Daily/Weekly High and Low

## Core Idea
Rather than fading previous-day/week highs and lows directly (which produces too many false breakouts), the author waits for those highs/lows to be breached and then trades the retest of the breached level using the same support/resistance-flip logic as Strategy 1.

## Frameworks Introduced
- **Daily/Weekly High-Low breach-and-flip**: previous day's (or week's) high/low are strong S/R because many participants remember and defend them; but rather than trading the level directly, wait for a breach and trade the retest of the flipped level.
  - When to use: whenever a clean previous-day or previous-week high/low is identified and hasn't already been tested/exceeded again.
  - How (long scenario): wait for the previous day's high (resistance) to be breached; require 1–3 confirming candles above it (30-minute candles for intraday, daily candles for swing trading); once confirmed as new support, wait for price to return to it and enter long.
  - How (short scenario): mirror image — wait for the previous day's low (support) to be breached; require 1–3 confirming candles below it; once confirmed as new resistance, enter short on the retest.
  - Validity condition: the high/low must not have already been tested with a new higher-high or lower-low created — if it has, the author no longer considers it a valid S/R zone.
  - Same setup applies to weekly highs/lows, traded identically.

## Key Concepts
- **Daily/weekly high**: the price point where buyers stopped and sellers took over that day/week — remembered and defended by market participants.
- **Daily/weekly low**: the mirror point where sellers exhausted and buyers took over.
- **False breakout risk**: the author's stated reason for rejecting the "obvious" strategy (long from prior low, short from prior high) — it fails too often due to false breakouts through these zones.
- **Confirming candles**: 1–3 bars beyond the breached level (30-min for intraday, daily for swing) required before treating the flip as valid.

## Mental Models
- Treat a breach of a well-known high/low as evidence of real institutional force ("strong force = strong buyers or strong sellers") — this is what makes the flipped level worth trading, not the original level itself.
- Apply the exact Strategy 1 (support-becomes-resistance) mental model here — this strategy is explicitly that framework applied specifically to daily/weekly extremes.

## Anti-patterns
- **Fading the untested high/low directly** ("go long at prior low, short at prior high"): the author explicitly abandoned this due to high false-breakout rates.
- **Trading a high/low that's already been retested and exceeded**: once a new higher-high or lower-low forms, the original level is no longer treated as valid.
- **Entering immediately on the breach**: must wait for 1–3 confirming candles beyond the level, then wait further for the retest — no chasing the breakout.

## Worked Example
Long scenario, EUR/USD 30-minute chart: previous day's high (acting as resistance) is breached; 1–3 30-minute candles close above it, confirming the market accepted the breach; price later pulls back to this now-support level, and a long is entered on the retest — mirroring the same mechanic used for intraday and, with daily candles instead, for swing trades. Short scenario (also EUR/USD 30-minute): previous day's low (support) is breached, 1–3 candles confirm below it, and on the pullback retest of the newly-flipped resistance, a short is entered.

## Key Takeaways
1. Don't fade untested daily/weekly highs and lows directly — false breakout rates are too high.
2. Wait for a confirmed breach (1–3 candles beyond the level) before treating it as flipped.
3. Enter only on the retest of the flipped level, in the direction of the breach.
4. Discard a high/low as a valid zone once it has been retested and a new higher-high/lower-low has formed.
5. The identical method applies to both daily and weekly highs/lows — only the candle timeframe used for confirmation changes (30-min for intraday vs. daily candles for swing).

## Connects To
- **Ch4 (Strategy 1)**: this strategy is a direct, explicit application of the support-becoming-resistance framework to daily/weekly extremes.
- **Ch10**: Strong or Weak Highs/Lows extends the analysis of what a high/low formation reveals about underlying strength.
