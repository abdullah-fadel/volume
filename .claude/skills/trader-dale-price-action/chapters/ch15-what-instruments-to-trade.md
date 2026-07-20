# Chapter 15: What Instruments to Trade

## Core Idea
Specialize in a small number of instruments (like a lawyer specializing in one legal field) rather than spreading across many, because trading too many correlated instruments creates hidden "excessive risk exposure" and makes flawless strategy execution unmanageable.

## Frameworks Introduced
- **Excessive risk exposure**: holding multiple positions in heavily correlated instruments (e.g., several USD-based pairs) that all move together, so a single event (news, USD rally) can produce several losses at once instead of one.
  - When to use: as a portfolio-level check before or while holding multiple open positions.
  - How: consult a correlation table (correlation ranges from -100% to +100%); set a simple hard rule (e.g., "no more than two USD positions open at once") or halve position sizes when entering two heavily correlated trades simultaneously.
- **Steps to choose the right trading instruments** (author's stated process):
  1. Cut costs — favor the most liquid pairs (author's picks: EUR/USD, AUD/USD, USD/JPY, USD/CAD) and a reputable broker with tight spreads.
  2. Test the strategy — run a quick backtest per candidate instrument to decide whether to keep testing it or move on; follow with thorough backtesting and live testing (detailed in Ch21).
  3. Choose only a few instruments — start with one or two, get proficient, then add more gradually until reaching a desired trade-frequency level.

## Key Concepts
- **Correlation**: the degree to which two instruments move alike (+100% = identical, -100% = exact opposite); real-world values sit between these extremes (e.g., EUR/USD vs. USD/JPY ≈ -4.8%, effectively independent).
- **Market Share / liquidity and cost**: pairs with bigger market share generally have lower trading costs (tighter spreads); volatility also drives cost — the more volatile the instrument, the higher the typical spread.
- **Instrument specialization**: professional/institutional traders often focus on just one or two instruments to build deep familiarity with volatility, correlation, news sensitivity, and typical volume behavior.

## Mental Models
- Treat instrument selection like choosing a legal specialty: depth on one or two pairs beats shallow familiarity with many.
- Before opening a new correlated position, ask "if the news/catalyst behind my other open trade also moves this one, am I comfortable losing on both at once?"

## Anti-patterns
- **Trading too many pairs at once**: makes flawless execution (analysis, entry, exit, position/money management, news-awareness) unrealistic across 10+ simultaneous instruments.
- **Ignoring correlation when sizing multiple positions**: can silently multiply risk on what looks like several independent trades.
- **Trading GBP pairs with a Volume-Profile-based strategy tuned for cleaner reactions**: the author avoids GBP because it aggressively spikes past major S/R zones, which doesn't suit his level-based method.

## Reference Table

**Author's per-pair characteristics (forex majors)**

| Pair | Volatility | Cost | Reaction to volume-based S/R | Notes |
|---|---|---|---|---|
| EUR/USD | Average | Cheapest | Excellent | Author's #1 pair; most liquid; "tells you" when something significant is happening |
| AUD/USD | Lower / slow | Cheap | Good and precise | Commodity currency; China-news dependent; needs patience |
| USD/CAD | More volatile | Good, not cheapest | Good but sometimes imprecise (overshoots) | Very reactive to oil news; correlates with AUD/USD via commodities |
| USD/JPY | More volatile | Cheap (high liquidity) | Very precise despite volatility | Safe-haven currency; capable of large spikes |
| GBP/USD | Volatile | Moderately cheap | Hard to predict / inconsistent timing | Dead in Asian session; strong reaction to UK CPI/BREXIT news; good trend-catching but requires fast exits |

Author's preferred pair combo for Volume Profile trading: **EUR/USD + USD/JPY** — both cheap, good S/R reactions, low mutual correlation, and matching pip sizing for SL/PT.

- **Intraday instruments** (author's picks): EUR/USD, AUD/USD, USD/CAD, USD/JPY, plus non-currency instruments like FDAX, S&P 500, and crude oil (CL).
- **Swing/long-term instruments** (author's broader list): AUD/CAD, AUD/CHF, AUD/JPY, AUD/NZD, AUD/USD, CAD/JPY, EUR/GBP, EUR/JPY, EUR/USD, GBP/USD, CHF/JPY, NZD/CAD, NZD/USD, USD/CHF, USD/JPY, USD/CAD.
- **Crypto (bonus)**: focus on the highest market-cap coins for liquidity (Bitcoin first, then e.g. Ethereum, Ripple); avoid instruments that go sideways for long stretches then jump — poor fit for intraday/swing trading.

## Key Takeaways
1. Specialize in a small number of instruments before expanding — depth beats breadth.
2. Check correlation before stacking multiple open positions; cap exposure to correlated instruments with a simple hard rule.
3. Prioritize liquidity/low cost for intraday trading; cost matters far less for swing/long-term.
4. Avoid instruments whose price behavior conflicts with your method (author avoids GBP due to spike-through behavior vs. his level-based approach).
5. For crypto, prioritize market-cap leaders and avoid instruments with long dead stretches.

## Connects To
- **Ch14**: instrument choice interacts directly with the style (intraday/swing/long-term) chosen there.
- **Ch19 (Money Management)**: correlation-based risk limits here connect to the broader money-management/correlation discussion.
