# Chapter 1: Setting Up Order Flow

## Core Idea
Order Flow only pays off if the underlying setup is right: a centralized-market data feed with real Bid/Ask, one mastered trading instrument, and (if you actually execute in Forex) a disciplined way to carry Futures-based levels across to the Forex chart.

## Frameworks Introduced
- **Futures-first analysis, Forex-optional execution**: Trader Dale analyzes on Futures (where Bid/Ask is real) and can execute either on Futures or transfer the read to spot Forex.
  - When to use: whenever your broker/instrument doesn't give true Bid/Ask (most Forex feeds don't).
  - How: pick a correlated Futures contract (e.g., 6E for EUR/USD), do all Order Flow reading there, then transfer levels to the pair you actually trade.
- **One-Instrument Mastery Rule**: Start and stay with a single trading instrument until it is mastered.
  - When to use: always, especially early on.
  - How: pick one instrument (Dale uses 6E — EUR Futures), learn its typical volume, active hours, and reaction style before adding a second instrument. Every instrument behaves differently, so skill on one doesn't automatically transfer.

## Key Concepts
- **Level 1 data**: Bid/Ask price and size data — the minimum feed quality Order Flow requires.
- **Level 2 data**: Full market depth (pending order book); not needed for Order Flow, only for DOM/tape reading.
- **DOM (Depth of Market)**: Shows pending orders in the book; Dale abandoned it because most pending orders never fill and are placed only to influence price ("carrot in front of a donkey").
- **Centralized market (Futures)**: Everyone sees the same price and the same Bid/Ask volumes — required for genuine Order Flow reading.
- **Decentralized market (Forex)**: Each broker/data provider sees slightly different prices and generally cannot split Bid vs. Ask reliably, so it only supports Total Volume, not true Order Flow.
- **6E**: CME EUR/USD currency futures contract — the author's primary instrument, used as the Futures proxy for EUR/USD.
- **NinjaTrader 8**: The free charting platform the author builds and runs Order Flow on; trade execution can still happen with a separate broker.

## Mental Models
- Think of Forex Order Flow as "volume without a scoreboard": you get Total Volume (heavy vs. light areas) but not who's winning the Bid/Ask fight — still useful, just less precise than Futures.
- Use Futures-to-Forex level transfer like reading a mirror: positively-correlated pairs (EUR, AUD) map visually 1:1; inversely-correlated ones (CAD, JPY, CHF) require mentally flipping the chart, and 1 Futures tick ≠ 1 Forex pip.
- Treat picking a data feed and platform as infrastructure, not strategy — get it right once so it never becomes a source of doubt while reading Order Flow live.

## Anti-patterns
- **Trading Order Flow on old/limited platforms (e.g., MetaTrader 4) or plain Forex feeds without a Futures cross-check**: these can't show real Bid/Ask, so signals such as Delta, Imbalances, and Absorption become unreliable or unavailable.
- **Jumping between multiple instruments while still learning**: each instrument has its own "normal" volume and behavior; splitting attention early slows down pattern recognition and produces false reads.

## Worked Example
Transferring a level from Futures to Forex, as described by the author:
- **Positively correlated case (EUR, AUD Futures → EUR/USD, AUD/USD)**: Place the Futures and Forex charts side by side. Because correlation is close to 100%, a Support/Resistance level identified on 6E sits at essentially the same visual location on the EUR/USD chart — read it across directly.
- **Inversely correlated case (CAD, JPY, CHF Futures)**: Correlation is close to ‑100%, so the Forex chart is the mirror image of the Futures chart, and one Futures tick does not equal one Forex pip. The author still transfers the level visually, but mentally flips the chart top-to-bottom before mapping the level across. He describes this as a skill that clicks with repetition — "like learning to ride a bike."

## Key Takeaways
1. Order Flow requires Level 1 (Bid/Ask) data on a centralized market — verify your feed supports this before building a strategy around it.
2. Master one instrument (the author uses 6E) before adding others; volume behavior is instrument-specific.
3. If you execute in Forex but read Futures, build the visual habit of transferring levels — remember to flip the chart for inversely-correlated pairs (CAD, JPY, CHF).
4. Skip DOM/tape reading as a primary tool — pending orders are mostly noise; Order Flow only shows orders that actually filled.
5. NinjaTrader 8's free tier is fully functional for Order Flow charting even if you execute trades elsewhere.

## Connects To
- **Ch 3**: Basic Chart Description explains exactly what the Bid/Ask data enabled by a proper feed lets you see (Footprints, Delta).
- **Ch 4**: Special Features notes that some setups (Volume Clusters, Multiple Nodes) work on Volume-only data and are therefore usable directly on Forex.
