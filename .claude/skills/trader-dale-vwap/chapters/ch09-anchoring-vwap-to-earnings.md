# Chapter 9: Anchoring VWAP to Earnings

## Core Idea
Earnings reports are the single biggest source of the large stock-only gaps covered in Ch8, so anchoring VWAP directly at the earnings-release candle is a natural, stocks-exclusive refinement of gap anchoring — with the added benefit that the earnings' surprise magnitude (not the market's initial direction) determines how meaningful the resulting VWAP will be.

## Frameworks Introduced
- **Earnings-anchored VWAP**: VWAP calculated starting from the candle where a stock's earnings report was released.
  - When to use: stocks only; the author's preferred timeframe is Daily, but it also works intraday (5–30 min).
  - How: locate the stock's earnings report date (TradingView displays earnings dates at the bottom of the chart) → anchor VWAP to the candle at the earnings release → trade pullbacks to the resulting VWAP using the standard approach (Ch2) → when comparing multiple earnings reports on the same chart, prioritize anchoring to the one that produced the largest gap/biggest surprise, since not all earnings reports move the market equally even though they're all "earnings."
  - Why it works: the same rationale as gap anchoring (Ch8) — a big, surprising earnings reaction resets what traders consider the "fair price," and that reference point draws broad attention regardless of whether the initial reaction was bullish or bearish.

## Key Concepts
- **Earnings report**: a scheduled corporate disclosure event that frequently produces the largest gaps a stock will see in a given period.
- **Relative earnings significance**: not every earnings report is equally market-moving — the author explicitly ranks earnings events by the size of the resulting gap/surprise and anchors only to the most significant one on a given chart, even when multiple earnings dates are visible.
- **Direction-independent reliability**: the earnings reaction's initial direction (up or down) does not predict which side will ultimately control the anchored VWAP — the anchor's value comes from the surprise magnitude, not the direction.

## Mental Models
- Treat earnings anchoring as a specialized case of gap anchoring (Ch8) — same underlying logic, narrower and more specific trigger (a scheduled, identifiable corporate event rather than any gap).
- When several earnings dates appear on one chart, rank them by reaction size and anchor only to the standout one — don't treat every earnings date as an equally valid anchor.

## Anti-patterns
- **Anchoring to every earnings date on a chart**: the author explicitly discounts subsequent earnings reports that didn't produce comparably large gaps or surprises — only the standout event deserves an anchor.
- **Assuming the earnings-day direction predicts VWAP control**: a positive earnings surprise doesn't guarantee buyers stay in control of the anchored VWAP — sellers can still take over even after bullish news (see Worked Example).

## Worked Example
Walmart, 5-minute chart: earnings produce a big gap up at the open — seemingly bullish news. But once the initial post-earnings volatility settles, price mostly trades below the earnings-anchored VWAP, meaning sellers actually held the upper hand despite the positive-looking earnings reaction. This produces three separate short opportunities as price pulls back up to touch the now-resistance VWAP line. The lesson: the earnings anchor's usefulness doesn't depend on correctly guessing the earnings reaction's "true" direction in advance — the anchored VWAP itself reveals which side actually gained control after the dust settles, which is the actionable signal.

## Key Takeaways
1. Stocks-only strategy, closely related to gap anchoring (Ch8) since earnings produce the largest and most significant gaps.
2. Anchor at the earnings-release candle itself; locate the date via TradingView's earnings markers or equivalent.
3. When multiple earnings dates are visible, anchor only to the one with the largest/most surprising gap — treat the rest as less significant.
4. Works on Daily (author's preference) or intraday timeframes.
5. The initial gap direction doesn't predict which side controls the anchored VWAP afterward — let the post-earnings price action relative to VWAP tell you who's actually in control.

## Connects To
- **Ch8**: the general gap-anchoring technique this chapter specializes for earnings events specifically.
- **Ch2**: standard pullback-to-VWAP entry mechanics apply once the earnings anchor is set.
