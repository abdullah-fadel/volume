# Patterns

Concrete, repeatable techniques from the book. Each includes when to use it, how to execute it, and its trade-offs.

## Strategy #1 — Reactions to VWAP
**When to use**: any instrument/timeframe; base entry once you know which side of VWAP currently controls price.
**How**: identify prevailing side (above VWAP = buyers control, below = sellers control) → wait for a pullback that touches the VWAP line → enter long on a touch from above, short on a touch from below.
**Trade-offs**: simplest possible VWAP signal; the author explicitly treats it as the entry-level version, layering confirmation (Ch13) and confluence (Ch12) on top before real entries.

## Anchoring VWAP to Dates (Daily/Weekly/Yearly)
**When to use**: Daily for intraday scalping (5-min), Weekly for the author's favorite intraday reference (30-min), Yearly for swing/long-term (Daily chart).
**How**: plot VWAP from the relevant calendar boundary → trade pullback reactions → if price crosses through, flip bias to match the new Support/Resistance role.
**Trade-offs**: signal frequency drops sharply as the anchor period lengthens (Daily > Weekly > Yearly); works best in trending conditions, weaker in chop.

## Anchoring VWAP to Swing Points
**When to use**: any timeframe, once a genuinely significant swing high/low (widely recognized trend-reversal point) is identified.
**How**: anchor VWAP at the swing candle → trade pullback reactions → keep trading timeframe and SL/TP sizing consistent with the anchor's timeframe.
**Trade-offs**: reactions can be sharp and fast (easy to miss the entry); the anchor point sits slightly off the literal candle wick due to VWAP's OHLC/4 calculation.

## Anchoring VWAP to Start of the Trend
**When to use**: once a strong trend has begun with a clear, decisive launch candle.
**How**: anchor VWAP at the largest, most decisive candle near the trend's start → trade pullbacks in the trend direction → treat a role-flip (price crossing to the other side) as an early trend-exhaustion warning.
**Trade-offs**: reaction strength benefits from combined new-entrant + trapped-trader-exit order flow; minor anchor-candle disagreement between traders usually doesn't matter, but anchors chosen too far apart can diverge meaningfully.

## Anchoring VWAP to Macro News Candle
**When to use**: short-term/intraday (5–30 min); best on instruments the specific news event actually affects.
**How**: filter candidate news by severity tag (red/high-impact) first, then by actual observed reaction (durable trend start, not a brief spike) → anchor VWAP at the confirmed news candle → trade pullbacks in the resulting trend's direction.
**Trade-offs**: many "high-impact" tagged events don't move markets meaningfully — the severity label alone is an insufficient filter; later pullbacks along the same line can fade in strength as momentum decays.

## Anchoring VWAP to Heavy Volume Zones
**When to use**: any timeframe/instrument, when a Volume-Profile-identified rotation zone with heavy volume is followed by a clear trend.
**How**: use Volume Profile to find a heavy-volume rotation zone → read the trend that follows to infer institutional side (accumulation direction) → anchor VWAP at the trend-launch candle (end of rotation, not inside it) → trade pullbacks in the trend direction.
**Trade-offs**: requires a Volume Profile tool as a companion — not usable from price action alone; universal across instruments/timeframes once available.

## Anchoring VWAP to Gaps
**When to use**: primarily stocks (gaps are structurally rare in continuous forex trading); intraday or daily timeframes.
**How**: scan for a big gap → anchor VWAP at the first candle after the gap → trade pullback reactions using the standard base logic, including role-flips.
**Trade-offs**: only worthwhile for large, attention-drawing gaps; the gap's initial direction doesn't predict which side ultimately controls the anchored VWAP.

## Anchoring VWAP to Earnings
**When to use**: stocks only; specialized case of gap anchoring, since earnings produce the biggest gaps.
**How**: locate the earnings-release candle (e.g., via TradingView's earnings markers) → anchor VWAP there → if multiple earnings dates are visible, anchor only to the one with the largest/most surprising reaction → trade pullbacks as usual.
**Trade-offs**: the earnings day's apparent direction (positive/negative surprise) doesn't reliably predict which side controls the anchored VWAP afterward.

## VWAP Rotation Strategy
**When to use**: 1st VWAP deviations are moving horizontally (confirmed sideways market); date-anchored VWAP only (Daily/Weekly/Yearly).
**How**: confirm horizontal deviation slope → enter Long off the lower 1st deviation (from above, as Support) → enter Short off the upper 1st deviation (from below, as Resistance) → target the VWAP line for Take Profit.
**Trade-offs**: invalidated the moment price closes outside the deviation channel — at that point, hand off to the VWAP Trend strategy instead; give newly-plotted deviations time to develop before trading them.

## VWAP Trend Strategy
**When to use**: 1st VWAP deviations are moving vertically (confirmed trending market).
**How**: in an uptrend, confirm the upper deviation trends upward and price sits above it → enter Long on a pullback touching the upper deviation from above. In a downtrend, mirror with the lower deviation and Short entries.
**Trade-offs**: offers positive RRR and a trailable position (unlike the Rotation strategy's fixed VWAP-line target); deviations often need time (sometimes a catalyst like macro news) to separate into a clear trend after a new anchor period starts.

## Confluence Trading (Combos)
**When to use**: whenever you want higher-conviction entries than a standalone VWAP signal.
**How**: identify a VWAP-based level (any anchor/strategy) → separately identify a Price Action support-becomes-resistance level or Volume Profile Trend setup level (or a second, differently-anchored VWAP) → check for overlap in the same general zone → prioritize entries at the overlap.
**Trade-offs**: only meaningful when the combined setups are genuinely independent methods; not every valid VWAP touch will have confluence available — it raises conviction, it isn't a requirement.

## Price Action Setup: Support Becomes Resistance (and vice versa)
**When to use**: standalone Price Action confirmation, or as a VWAP confluence partner; works across timeframes (author prefers Daily and 30-minute).
**How**: spot strong reaction(s) at a level (2+ adds confidence) → wait for the level to be breached → treat the breached level as flipped and still significant → enter on the retest in the direction of the flip.
**Trade-offs**: reused throughout the book as both a standalone Price Action tool and the most common confluence partner for VWAP levels.

## Volume Profile Trend Setup
**When to use**: within an established, strongly trending market — the author's preferred VWAP confluence partner since both favor trending conditions.
**How**: confirm a strong trend → find a volume cluster formed as a pause within the trend → mark the cluster as Support (uptrend) or Resistance (downtrend) → enter at the start of the cluster on a retest, trend direction.
**Trade-offs**: full setup detail (and two sibling setups — Accumulation, Rejection) covered in the author's dedicated Volume Profile book.

## Trade Entry Confirmation — Entering After a Successful Reaction
**When to use**: the author's default confirmation method when confluence isn't already present.
**How**: watch price approach the level → wait for one full candle to close confirming the reaction (bullish close above Support / bearish close below Resistance) → enter as the next candle opens → place SL behind the Reaction Point (the confirming candle's swing).
**Trade-offs**: enters later, can miss part of the move (especially with an unusually large confirming candle), but validates that price is actually reacting, not just touching.

## Trade Entry Confirmation — First Touch with Combos
**When to use**: only when a level already has multi-setup confluence backing it (Ch12).
**How**: skip candle confirmation and enter directly on first touch, relying on the multi-setup agreement itself as confirmation.
**Trade-offs**: the author's explicit exception to his own "don't blind-enter" rule — validated specifically by confluence strength, not by waiting for a reaction.

## Order Flow Confirmation
**When to use**: the author's preferred, most advanced confirmation method; requires Order Flow software/training. Only meaningful at an already-identified VWAP/Price-Action/Volume-Profile level, not in isolation.
**How**: watch for Absorption (heavy Bid+Ask volume simultaneously at the level), a large Limit Order (single oversized order on one footprint side at the level), or Cumulative Delta divergence (Delta moving opposite to price near the level) → treat any of these as institutional confirmation.
**Trade-offs**: highest-confidence method but the steepest learning curve and tooling requirement; a signal appearing away from a real level carries little value.

## Take Profit Placement (Price Action / VWAP / Volume Profile / ATR)
**When to use**: every open trade needs a Take Profit plan.
**How**: identify the nearest strong barrier (Price Action flip level, opposing VWAP level, or Volume Profile heavy zone) ahead of the position → exit a few pips before reaching it. Alternative: size a fixed TP at 10–20% of ATR-derived average daily volatility (intraday).
**Trade-offs**: overplotting VWAP levels creates false barriers everywhere — restrict to the strongest signals; a barrier that only stalls (rather than reverses) price is often still worth exiting at rather than waiting out chop.

## Stop Loss Placement (Price Action / VWAP / Volume Profile / Combined / ATR)
**When to use**: every trade requires SL behind a barrier.
**How**: place SL behind the nearest swing point (Price Action), VWAP/deviation line (VWAP), or heavy volume zone (Volume Profile) — or, for the strongest protection, behind two or more overlapping barrier types at once (combined). Migrate SL forward through the VWAP-family chain as price advances. Fallback: ATR-based SL at 10–20% of average daily volatility when no barrier is available.
**Trade-offs**: combined barriers are strongest but shouldn't be chased too far away when trailing — a closer, weaker barrier beats a farther, stronger one for protecting open profit.

## Trailing Your Trade
**When to use**: after entering a strong trend on a pullback, to ride the move for larger profit than a fixed TP would capture.
**How**: place initial SL behind the first valid barrier → as the trend develops and new barriers (swing points, heavy volume zones, VWAP levels) form, walk SL forward to each in turn → continue until the trend ends and the trailed SL is hit.
**Trade-offs**: same distance-vs-strength trade-off as combined-barrier SL placement — never trail to a distant barrier at the cost of giving back too much accumulated profit.

## Start Simple Template
**When to use**: recommended default for beginners overwhelmed by the full entry/SL/TP toolkit.
**How**: Entry = confirmed-reaction method (candle close confirmation) → SL = the Reaction Point that entry naturally creates → TP = 1:1 Risk-Reward Ratio (mirror the SL distance).
**Trade-offs**: deliberately simplified — skips barrier-based TP/SL variety and confluence requirements in favor of one consistent, learnable loop; the same rule set can still produce both quick scalp trades and larger trend trades.

## Risk Per Trade Formula
**When to use**: before trading any strategy live, to size positions.
**How**: backtest the strategy's worst losing streak → pad it 20% (×1.2) → divide your personal max tolerable drawdown % by that padded streak → apply the resulting percentage as a fixed risk on every trade.
**Trade-offs**: depends entirely on having real backtest data; requires an honest, personal assessment of drawdown tolerance rather than a generic number.
