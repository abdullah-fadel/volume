# Patterns

Concrete, repeatable techniques from the book. Each includes when to use it, how to execute it, and its trade-offs.

## Support Becoming Resistance (and Vice Versa)
**When to use**: a level has produced two or more strong reactions (confirming real support/resistance), and price has since broken through it.
**How**: mark the level after 2+ strong reactions → wait for a confirmed breach → treat the breached level as flipped (support→resistance or resistance→support) → wait for price to pull back to it → enter in the direction consistent with the flip (short from new resistance, long from new support).
**Trade-offs**: reliable and frequent (author calls it a near-daily setup), but requires patience for the retest — don't chase the breakout candle. Also the base mechanic reused inside Strategy 6 (daily/weekly highs/lows) and the Reversal Trade pattern.

## Open-Drive
**When to use**: a sudden, strong, one-sided move appears, typically after a sideways range or at a session open.
**How**: mark the exact candle/point where the aggressive move began → wait a few candles to confirm the market accepted the new price as fair value → wait for a pullback to the origin point → enter in the direction that continues the original aggression (long if buyers drove it, short if sellers drove it).
**Trade-offs**: strong, frequently reliable level; less useful without the confirming candles, and can be triggered by news (treated as still valid regardless of cause).

## AB=CD
**When to use**: on 30-minute charts and above, as a confirmation for volume-based entries or standalone.
**How**: mark swing A and B → confirm C retraces ≥50% of AB without exceeding A → project D at the same pip distance from C as A is from B (via Fibonacci: 0%→A/100%→B, then shift 0%→C) → enter long at D (bullish) or short at D (bearish).
**Trade-offs**: psychology-based rather than institutional-footprint-based; author uses it mainly as a secondary confirmation layer, not a primary signal.

## Session Open / Daily Open
**When to use**: as confirmation only, never standalone.
**How**: mark the open of each session (Tokyo/London/New York) or the Daily Open (5 p.m. NY time) → if price moves down after the open, the level becomes resistance; if up, it becomes support → watch for reactions on retest.
**Trade-offs**: Daily Open is judged the strongest of these; Session Opens are weaker orientation points. Neither is traded alone.

## Daily/Weekly High-Low Breach-and-Flip
**When to use**: a previous day's/week's high or low is identified and hasn't already been retested with a new extreme.
**How**: wait for the high/low to be breached → require 1-3 confirming candles beyond it (30-min for intraday, daily for swing) → treat the breached level as flipped support/resistance → enter on the retest.
**Trade-offs**: explicitly replaces the naive "fade the untested high/low" approach, which the author rejected due to high false-breakout rates. Once a level is retested and exceeded again, discard it.

## Strong vs. Weak High/Low Filter
**When to use**: applied to every candidate swing high/low before trusting it as a trade level, and to gauge whether price approaching an S/R zone is likely to reverse or shoot through.
**How**: classify by aggression/speed of reversal (not candle shape) — fast, decisive reversal = strong (trust it, anchor trades near it); slow, multi-candle indecisive testing = weak (expect price to shoot through it; never place a vulnerable trade level near one).
**Trade-offs**: requires practice to judge "aggression" reliably; the payoff is avoiding trades that are structurally likely to fail (weak point on the vulnerable side) and gaining an early profit-protection signal (strong point ahead of an open position).

## Failed Auction Exploitation
**When to use**: (a) to extend a Profit Target when a failed auction sits just past the normal target; (b) as a trade filter, screening for a failed auction against your position before entering.
**How**: classify swing extremes as successful (one clean "winner") or failed (multiple bidders unresolved) → expect price to be drawn through failed auctions to resolve them → extend PT past a nearby failed auction rather than leaving pips on the table; avoid entries where a failed auction sits against the position (below a long, above a short).
**Trade-offs**: used daily by the author for extra pips on Profit Targets and for avoiding structurally doomed trades; requires the same judgment skill as strong/weak classification.

## Volume Accumulation Setup (#1)
**When to use**: a sideways rotation area is followed by a strong directional move.
**How**: identify the rotation + subsequent trend (direction reveals accumulation side) → apply Flexible Volume Profile inside the rotation to find the single heaviest-volume price → mark that level → enter on first touch, no confirmation required.
**Trade-offs**: one of three setups the author never trades without; requires Flexible Volume Profile tooling to execute precisely.

## Volume Trend Setup (#2)
**When to use**: within a strong, established trend.
**How**: locate the volume cluster(s) formed where price briefly paused within the trend and the trend continued afterward → mark the heaviest-volume price in the cluster → enter in the trend direction on first touch.
**Trade-offs**: strongest in confluence with Support-Becomes-Resistance (author's "most powerful" combination); thin trend profiles can make clusters hard to spot precisely.

## Volume Rejection Setup (#3)
**When to use**: a strong, aggressive price rejection has occurred (any candle shape, any timeframe).
**How**: identify the aggressive rejection → apply Flexible Volume Profile to the rejection itself to find the heaviest-volume price within it → mark that level → enter on retest (long after a rejection of lower prices, short after a rejection of higher prices).
**Trade-offs**: author's own hardest setup to master — judging rejection strength and reading volume distribution within it (especially with multiple strong volume areas) takes practice.

## Reversal Trade
**When to use**: any of the three Volume Setups (or a Price Action level) fails outright — price shoots through with no reaction and hits the Stop-loss.
**How**: wait for price to return to the original level → enter in the opposite direction of the original trade.
**Trade-offs**: validity requires a clean failure (no partial reaction, not even 1-2 pips) — a partial reaction means the level "worked, only sooner," not a reversal setup. Requires fast psychological bias-switching; start with smaller size to build confidence.

## Alternative Stop-loss Approach
**When to use**: swing trading only (author does not apply it intraday); when you want protection against being shaken out by noise/stop-hunts at a structurally valid level.
**How**: don't exit on a mere touch of the "normal SL" → wait for a full Daily candle close beyond it before exiting → cap worst-case risk with a "catastrophic scenario SL" at 150% of normal SL, which triggers an immediate exit regardless of candle closes.
**Trade-offs**: can save trades that would otherwise be stopped out by a temporary overshoot, but final risk is not known in advance except at the 150% ceiling.

## Correlation-Based Position Sizing
**When to use**: two or more heavily correlated instruments present a similar setup near the same time.
**How**: reduce position size on the correlated trades (rather than skipping or ignoring the overlap) since they are likely to move — and resolve — together.
**Trade-offs**: caps upside on the correlated trades in exchange for not doubling real exposure to one underlying driver.

## 5-Phase Strategy Validation
**When to use**: introducing and scaling into any new trading idea.
**How**: Phase 1 rough backtest (fast, simplified, ~1-2 hrs) → Phase 2 thorough backtest (full rules, more markets/settings) → Phase 3 micro live trading (10-20% normal size, real account, no demo) → Phase 4 half positions (~50% size, focus on flawless execution) → Phase 5 full positions (push through the expected early "trial by fire" losing streak).
**Trade-offs**: slower to reach full conviction than jumping straight to live full-size trading, but explicitly designed to separate "does the edge exist" from "can I execute it under real psychological pressure."
