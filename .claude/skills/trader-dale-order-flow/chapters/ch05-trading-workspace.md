# Chapter 5: Order Flow – Trading Workspace

## Core Idea
A workable Order Flow workspace links four linked charts at different timeframes — big picture, entry detail, noise filter, and momentum confirmation — so every decision has both a macro and a micro view available without switching charts mid-trade.

## Frameworks Introduced
- **Four-Chart Linked Workspace**: the author's standard screen layout for live intraday trading.
  - When to use: as a starting template for setting up your own Order Flow trading screen.
  - How: link all four charts to the same instrument and lay them out as below (Reference Table). Adjust timeframes to taste once the roles are understood, but keep the "big picture / entry detail / noise filter / momentum" role split intact.

## Key Concepts
- **Top-left chart (big picture)**: 30-minute footprint, Total Volume (Bid+Ask) cell content, Delta printed per footprint, Daily Volume Profile on the side, with a Delta/Cumulative Delta/Volume summary.
- **Top-right chart (entry/exit detail)**: 5-minute footprint with Bid x Ask cell content and per-footprint Delta — used specifically for trade entries and exits.
- **Bottom-left chart (noise filter)**: 30-minute Order Flow with Trades Filter enabled plus Daily Volume Profile — used to filter out small orders and focus on big trading activity.
- **Bottom-right chart (momentum)**: 1-minute price chart stacked above a 1-minute Cumulative Delta chart, for spotting price/Delta divergence in real time.

## Mental Models
- Treat the four charts as four different "questions" asked of the same instrument at once: Where's the bigger structure? (top-left) Where exactly do I get in/out? (top-right) Where are the big guys actually active right now? (bottom-left) Is momentum confirming or diverging? (bottom-right).
- Keep timeframes nested (30m → 5m → 1m) so each chart zooms progressively tighter rather than jumping around unrelated intervals.

## Anti-patterns
- **Trading off a single timeframe/chart**: the author's whole workspace exists because no single chart answers all four questions (structure, entry precision, noise filtering, momentum) at once.

## Reference Table

| Position | Timeframe | Cell Content | Purpose |
|---|---|---|---|
| Top-left | 30 Min footprint | Volume (Bid+Ask total) | Big picture / structure; Daily Volume Profile + Delta/Cum. Delta/Volume summary |
| Top-right | 5 Min footprint | Bid x Ask | Entry and exit precision |
| Bottom-left | 30 Min footprint | Bid x Ask + Trades Filter | Filter noise, track big orders; Daily Volume Profile |
| Bottom-right | 1 Min price + 1 Min Cumulative Delta | — | Momentum confirmation / divergence spotting |

## Key Takeaways
1. Use a 30-minute chart for structure and S/R zones, a 5-minute chart for precise entries/exits, and a 1-minute chart for momentum confirmation.
2. Keep the Trades Filter on a dedicated chart (bottom-left) so it doesn't clutter your entry-precision chart.
3. Pair a 1-minute price chart directly above a 1-minute Cumulative Delta chart specifically to make divergence visible at a glance.
4. This is a starting template, not a rulebook — the timeframe choices should track the setups in Ch 6–13, which are mostly built around 30-minute structure and 5-minute triggers.

## Connects To
- **Ch 6, Ch 7**: The Trading Setups typically use the 30-minute footprint for structure, matching this workspace's top-left/bottom-left charts.
- **Ch 9, Ch 10**: Confirmation setups favor the 5-minute Bid x Ask view, matching the top-right chart here.
- **Ch 10**: Confirmation Setup #4 (Cumulative Delta Divergence) is read directly off the bottom-right chart described here.
