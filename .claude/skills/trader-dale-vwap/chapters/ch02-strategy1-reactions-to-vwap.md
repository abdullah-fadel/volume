# Chapter 2: Strategy #1 — Reactions to VWAP (and Anchoring VWAP, overview)

## Core Idea
The base VWAP strategy is trading the pullback: wait for price to move away from VWAP, then enter in the direction of the prevailing side (long if price is above VWAP and returns from above, short if below and returns from below) when price touches the line again, because VWAP is the price zone where the "average" market participant — including institutions targeting "VWAP or better" fills — is already positioned.

## Frameworks Introduced
- **Strategy #1 — Reactions to VWAP**: trade pullbacks to the VWAP line, treating VWAP as dynamic support (price above, pulling back down to it) or dynamic resistance (price below, pulling back up to it).
  - When to use: any instrument, any timeframe; author's own preference is 5-min or 30-min intraday and Daily for swing trades, on major forex pairs, S&P 500, and stocks.
  - How: identify which side of VWAP price currently trades on (above = buyers in control, below = sellers in control) → wait for a pullback that touches the VWAP line → enter in the direction consistent with the prevailing side (long on a touch from above, short on a touch from below). This is the "basic" version — the author explicitly layers confirmation and confluence on top later (Ch12–13) rather than trading this signal in isolation.
  - Why it works: VWAP marks where the average participant is already positioned, including institutional algorithms explicitly instructed to fill "at VWAP or better." When price returns to VWAP, that resting institutional interest re-engages (sellers defend from above, buyers defend from below), pushing price away from the line again.
- **Anchoring VWAP**: the general technique of choosing VWAP's calculation start point to correspond with a market-significant moment, rather than only using a fixed calendar boundary.
  - When to use: whenever the default Daily/Weekly/Yearly VWAP doesn't capture the specific turning point you care about (a swing low, a trend start, a news spike, etc.) — covered anchor-by-anchor in Ch3–Ch9.
  - How: pick a candle/point where "the rules of the game changed" (a decision point where market sentiment shifted) and start the VWAP calculation there instead of at a calendar boundary.

## Key Concepts
- **Anchor point**: the chosen starting candle/time for a VWAP calculation; determines which "average participant" the line represents.
- **The seven anchoring categories**: Beginning of Day/Week/Year (calendar anchors, Ch3); important swing point (Ch4); start of a trend (Ch5); strong macro news candle (Ch6); heavy volume zone (Ch7); gap (Ch8); earnings (Ch9, stocks only).
- **"VWAP or better"**: the instruction large trading desks give algorithmic execution systems — buy at or below VWAP, sell at or above it — which is the mechanical reason VWAP attracts real resting orders.
- **Prevailing side**: whichever side of VWAP price currently sits on, used to determine trade direction (above = long bias on pullback, below = short bias on pullback).

## Mental Models
- Think of VWAP as a magnet with directional bias, not a fixed wall: the side price is currently on tells you which direction the "defense" will come from on the next touch.
- Use the anchor-point list as a checklist before choosing which VWAP to plot on a chart — a Daily VWAP anchored at midnight is not automatically the most relevant VWAP if a stronger turning point (swing low, trend start, news spike) exists on the same chart.

## Anti-patterns
- **Trading the basic pullback-to-VWAP signal with no confirmation or confluence**: the author immediately flags this as the entry-level version of the strategy — he layers confirmation methods (Ch13) and confluences with Price Action/Volume Profile (Ch12) before actually pulling the trigger in practice.
- **Learning all seven anchoring methods at once**: the author explicitly recommends picking a couple that feel comfortable rather than trying to master all anchor types simultaneously.

## Worked Example
EUR/USD in a downtrend: price sits below VWAP, meaning sellers are in control and the average participant already sold. Rather than shorting at a random point or chasing the current daily low, the logical entry is where the market already transacted on average — at VWAP. As price rallies back up to touch the VWAP line from below, resting institutional sell interest (traders instructed to "short at VWAP or better") re-engages, and the aggressive selling that follows pushes price back down away from the line. That reaction — sell pressure re-emerging exactly at the touch — is the entry signal for the Short trade.

## Key Takeaways
1. The base strategy is simple: prevailing side of VWAP determines direction; touch of the line is the trigger.
2. VWAP is anchored at a chosen start point — the default calendar anchor (start of day/week/year) is only one of seven categories; the other six (swing point, trend start, news candle, volume zone, gap, earnings) target specific market turning points.
3. This chapter's basic touch-and-enter signal is intentionally the starting point — the author builds toward requiring confirmation and confluence before real trade entries (see Ch12–13).
4. Match your anchor and timeframe to your trading style: intraday (5-min/30-min) vs. swing (Daily), forex/index majors vs. stocks.

## Connects To
- **Ch3–Ch9**: each chapter details one specific anchoring method from the list introduced here.
- **Ch10–Ch11**: Strategy #2 (1st VWAP deviations) extends this same pullback logic to bands drawn around VWAP rather than the VWAP line itself.
- **Ch12**: shows how to combine this base signal with Price Action and Volume Profile setups for higher-conviction entries.
- **Ch13**: trade entry confirmation methods that upgrade this basic "touch and enter" signal.
