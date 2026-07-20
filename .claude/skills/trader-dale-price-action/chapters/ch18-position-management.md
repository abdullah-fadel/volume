# Chapter 18: Position Management

## Core Idea
Both Profit Target and Stop-loss can be set either as a simple fixed pip value (fast, consistent, volatility-adjusted via ATR) or dynamically from Volume Profile structure (more precise, placed just in front of/behind the nearest significant volume zone) — and once in a trade, three distinct Stop-loss management styles (Aggressive, Neutral, Conservative) trade off simplicity against protecting a partial gain.

## Frameworks Introduced
- **Fixed vs. Volume-based Profit Target**: Fixed PT uses one ATR-derived pip value for every trade (simpler, less decision fatigue); Volume-based PT places the target a few pips *before* the nearest significant volume zone in the trade's path, since price risks reversing there.
  - Validity filter: if the nearest volume zone is closer than ~10% of average daily volatility, skip the trade — the potential gain isn't worth the risk.
- **Fixed vs. Volume-based Stop-loss**: Fixed SL uses one ATR-derived pip value for every trade; Volume-based SL is placed behind the nearest significant volume zone (often at a swing point where volume is thinnest), since that zone may itself stop price from reaching the SL.
  - Practical adjustment: if the nearest volume-based SL would be too tight relative to the instrument's volatility (author's example: 5-pip SL on an instrument with ~150-pip daily volatility), either use a fixed SL instead or place the SL behind the *second*-closest significant volume area.
- **Alternative SL approach**: instead of exiting the instant price touches the "normal SL" level, wait for a full candle *close* beyond it (author uses Daily candles, swing trading only — not applied to intraday) before exiting, since price sometimes overshoots a valid level (volatility, stop-hunts, insufficient room) and reverses back in your favor.
  - Safety net: a "catastrophic scenario SL" set at 150% of the normal SL — hit this and you exit immediately regardless of candle closes, capping the worst-case loss.
- **Three Stop-loss management styles**:
  - **Aggressive**: never move the initial SL; outcome is binary (full SL or full PT). Author's choice for the Asian session, when he's asleep and can't manage manually.
  - **Neutral**: move SL to the reaction/turn point once price reaches 70-80% of the Profit Target. Author's preferred approach for EU/US sessions. If price then returns to the moved SL, exit — the reaction already happened, just weaker than hoped.
  - **Conservative**: move SL to breakeven once price reaches 70-80% of PT. Author explicitly dislikes this — price commonly pulls back to entry before the real reaction plays out, so this style prematurely stops out trades that would have won.
- **Quitting early at breakeven**: applicable under any of the three SL styles — if price makes a long, unconvincing rotation against the entry with no real rejection, and then the entry level itself gets breached and starts acting as the opposite type of zone (resistance if long, support if short), exit at breakeven rather than waiting for the full SL. Best executed by pre-placing the PT/exit order at breakeven rather than trying to time a manual exit, since the window to do so is often only seconds to minutes. The author personally stopped using this technique in recent years in favor of simply holding trades to their conclusion.

## Key Concepts
- **Reaction point**: the specific price where the market actually turned during a favorable move — the anchor for the Neutral SL-management style.
- **Break-even (BE)**: SL moved to the entry price, eliminating downside on the trade (but potentially eliminating upside too, per the author's critique of the Conservative style).
- **Catastrophic scenario SL**: 150% of the normal SL distance — a hard backstop used specifically alongside the Alternative SL approach so worst-case risk is still known in advance.

## Mental Models
- Think of Volume-based PT/SL placement as anchoring to *where the market itself is likely to turn* (volume zones), rather than an arbitrary pip count.
- Use the Alternative SL approach as protection against getting shaken out by noise/stop-hunts at a level that was structurally correct — but always cap it with a catastrophic SL so the "wait it out" flexibility doesn't become unlimited risk.
- Match SL-management style to how actively you can monitor the trade: Aggressive for unattended sessions, Neutral/Conservative for actively watched sessions (with Neutral favored over Conservative).

## Anti-patterns
- **Using a Volume-based SL that's too tight relative to instrument volatility**: gets stopped out by normal noise; switch to fixed SL or the next-nearest volume zone.
- **Defaulting to Conservative (breakeven-at-70-80%) SL management**: the author explicitly warns this cuts winners short because price often pulls back to entry before the real move develops.
- **Applying the Alternative SL approach without a catastrophic SL cap**: removes the one safeguard that makes "wait for a candle close" tolerable from a risk-management standpoint.
- **Applying the Alternative SL approach to intraday trades**: the author restricts this technique to swing trading with Daily candles only.

## Worked Example
Swing trade, AUD/NZD Daily chart: a long entry based on the Volume Accumulation setup had its "normal SL" placed just below a support volume cluster, at the low of a prior pin-bar wick (≈1.0659). Price dipped through that normal SL level — likely triggering many standard stop orders clustered there — but because the author was using the Alternative SL approach, he didn't exit on the touch. Since neither the Daily candle closed beyond the normal SL nor did price reach the 150%-catastrophic SL, he held the position; price reversed upward the next day and the trade reached full profit. A second example (EUR/USD swing short) followed the identical pattern: price pushed into the SL zone without a confirming candle close or catastrophic-SL breach, the position was held, and price eventually reversed to deliver a profit.

## Key Takeaways
1. Choose Fixed PT/SL for simplicity and consistency; choose Volume-based PT/SL for precision anchored to where the market is likely to actually turn.
2. Skip a trade if the nearest volume-based PT zone is too close (under ~10% of average daily volatility) to justify the risk.
3. Consider the Alternative SL approach (wait for a candle close, capped by a 150% catastrophic SL) on swing trades to avoid being shaken out by noise — never on intraday.
4. Match SL-management style to your ability to monitor the trade: Aggressive when unattended, Neutral when actively watching (preferred over Conservative).
5. Avoid the Conservative breakeven-at-70-80% style as a default — it statistically cuts too many eventual winners short.

## Connects To
- **Ch13**: Volume Profile setups (Accumulation, Trend, Rejection) are the source structure for volume-based PT/SL placement.
- **Ch14**: ATR-based sizing introduced there underlies the Fixed PT/SL approach here.
- **Ch19 (Money Management)**: SL distance decisions here directly determine position sizing there.
