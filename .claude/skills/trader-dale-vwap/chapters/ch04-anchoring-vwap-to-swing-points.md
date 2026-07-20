# Chapter 4: Anchoring VWAP to Swing Points

## Core Idea
Anchoring VWAP at a significant swing high/low — a point where market sentiment visibly reversed — turns the indicator into a "fair price since the game changed" reference that tends to produce precise, repeatable reactions because that turning point is widely recognized by other traders.

## Frameworks Introduced
- **Swing-point-anchored VWAP**: VWAP calculated starting from the candle that marked a significant swing high or swing low (typically a trend-reversal point).
  - When to use: works across timeframes — anchor on a Daily chart for swing trading, or a 5-minute chart for intraday trading — as long as the swing point is genuinely significant (widely recognized, decision-changing).
  - How: identify a swing high/low where the prevailing trend visibly reversed (the author notes there's no exact formal definition — pattern recognition improves with practice) → anchor VWAP's calculation to that candle → treat subsequent pullbacks to the resulting line as Support (after a low) or Resistance (after a high) → keep Stop Loss/Take Profit sizing consistent with whichever timeframe you anchored on.
  - Why it works: a genuine swing point is a moment many market participants collectively noticed and acted on — VWAP anchored there tells you whether current price is above or below the "fair" average price since that shared reference moment, which other traders are implicitly measuring against too.

## Key Concepts
- **Swing point**: a high or low where market sentiment shifted significantly enough to reverse the prevailing trend; identified by eye/experience rather than a fixed rule.
- **Timeframe consistency rule**: if you anchor VWAP using a swing point found on the Daily chart, trade that VWAP on the Daily timeframe (matching SL/TP sizing) rather than mixing it into intraday decisions.
- **VWAP anchor point ≠ the exact candle low/high**: because VWAP's calculation uses OHLC/4 (average of open, high, low, close) rather than the raw low or high price, the anchored line does not start exactly at the swing candle's extreme wick — a technical detail worth expecting rather than treating as an error.

## Mental Models
- Think of a swing point as "the moment the rules of the game changed" — VWAP anchored there answers "where is the average price since that reset?" rather than "where is the average price since an arbitrary calendar boundary?"
- Widely-recognized swing points work as anchors precisely because other traders are watching the same point — it's a self-reinforcing reference level, not just a private observation.

## Anti-patterns
- **Anchoring to a minor, unrecognized wiggle**: a swing point only works as an anchor if it was genuinely significant — a small retracement most traders wouldn't flag doesn't carry the same reference weight.
- **Mixing timeframes**: anchoring on the Daily chart but trading/sizing SL-TP on a 5-minute chart breaks the consistency the author recommends.
- **Assuming the anchor starts exactly at the extreme wick**: expect the line's start to sit slightly off the candle's literal high/low due to the OHLC/4 calculation basis.

## Worked Example
S&P 500 futures, 30-minute chart: the author anchors VWAP at the lowest point on the chart — the exact candle where a downtrend reversed into an uptrend. From that point forward, price interacts with this anchored VWAP on three separate occasions, and each time it acts as reliable Support, producing three clean Long entries as price pulls back down to touch the line before continuing higher. A second example on Apple's daily chart shows the same mechanic on a longer timeframe: VWAP anchored at a significant early-2023 swing low that marked a downtrend-to-uptrend reversal acts as strong Support on the first pullback, attracting aggressive buying that pushes price higher again — though the author notes this particular touch happened fast enough that the entry was easy to miss, a reminder that anchored-VWAP reactions can be sharp and require attentive monitoring.

## Key Takeaways
1. Anchor VWAP at genuine swing highs/lows — points that visibly reversed the trend and that other traders would recognize.
2. This anchor type works on any timeframe; just keep your anchor timeframe and your trading timeframe (and SL/TP sizing) consistent.
3. The anchored line will not start exactly at the candle's wick extreme — VWAP uses OHLC/4, so expect a small offset.
4. Reactions at a well-chosen swing-point VWAP tend to be precise and can move fast — watch for the touch rather than expecting a slow, easily-caught approach every time.

## Connects To
- **Ch2**: uses the same base pullback-to-VWAP entry logic, applied to a swing-point anchor instead of a calendar anchor.
- **Ch5**: "start of trend" anchoring is closely related — a swing point is frequently also where a new trend begins.
- **Ch12**: swing points anchored here overlap conceptually with the Price Action support-becomes-resistance confluence setup, since both key off significant reversal levels.
