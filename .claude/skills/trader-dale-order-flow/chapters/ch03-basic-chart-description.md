# Chapter 3: Order Flow – Basic Chart Description

## Core Idea
The footprint chart replaces standard OHLC candles with a full record of executed Bid/Ask volume per price level, and its four building blocks — Green/Red cells, the High Volume Node, Delta, and the Volume Profile overlay — are the vocabulary every later setup in the book is written in.

## Frameworks Introduced
- **Footprint Chart Reading**: a candle-replacement that shows executed orders at each price level within the candle, not just OHLC.
  - When to use: as the base chart type for all Order Flow analysis.
  - How: a Buyer entering Long with a market order prints on the ASK side; a Seller entering Short with a market order prints on the BID side.
- **Delta Divergence**: watching for a footprint whose color (bullish/bearish) disagrees with its Delta sign.
  - When to use: as an early warning that a price reversal may be building, especially in trending conditions.
  - How: a bullish (up) footprint with *negative* Delta warns that Sellers are entering and are stronger than the Buyers pushing price up; a bearish (down) footprint with *positive* Delta warns the opposite. Note this signal is unreliable in rotational/sideways markets, because institutions there often blend market and limit orders to mask intent.

## Key Concepts
- **Footprint**: the box representing one candle, annotated with the actual Bid and Ask volumes traded at each price level within it.
- **Green cell**: a cell where the Ask number exceeds the Bid number at that price.
- **Red cell**: a cell where the Bid number exceeds the Ask number at that price.
- **High Volume Node (HVN)**: the price level within a single footprint where volume was heaviest, marked with a black outline — usually the place institutions were most active.
- **Yellow-highlighted HVN**: two or more consecutive footprints whose HVNs line up at the same price — an early flag for a Support/Resistance zone (formalized later as a "Multiple Node," Ch 4).
- **Delta**: the net of Ask minus Bid volume for a whole footprint; positive (green) means more volume traded at the Ask, negative (red) means more traded at the Bid.
- **Cumulative Delta**: the running sum of Delta across all footprints since the start of the trading day (defined fully in Ch 4).
- **Volume Profile (daily)**: a built-in overlay showing volume distributed by price across the whole session; blueish/green segments are Ask-side volume, red segments are Bid-side volume.

## Mental Models
- Read color as "who's currently stronger, roughly" — green cells/footprints suggest Buyer strength, red suggests Seller strength — but always keep Chapter 2's passive/active caveat in mind; this is a simplification the author deliberately keeps easy at this stage.
- Use the footprint summary panel like a dashboard, not a wall of gauges: the author deliberately limits his own summary to three fields — Delta, Cumulative Delta, and Volume — because more clutters the read rather than helping it.
- Treat the daily Volume Profile as the "zoomed-out" partner to the footprint's "zoomed-in" detail — combining the two (favorite intraday approach) is a recurring theme through the rest of the book.

## Anti-patterns
- **Reading Delta divergence the same way in a rotation as in a trend**: in a rotating/sideways market, big players mix market and limit orders specifically to disguise intent, so Delta divergence there is much less trustworthy than in a clear trend.
- **Cluttering the summary panel with every available stat**: the author explicitly warns that most Order Flow software's long feature lists mostly distract from the handful of numbers (Delta, Cumulative Delta, Volume) that actually matter.

## Worked Example
**Price and Delta Divergence trade (EUR Futures / 6E, real trade from the author's log):**
1. The author had previously identified and publicly posted a Resistance level on EUR/USD using Volume Profile, then waited roughly a week for price to reach it.
2. When price arrived, the market was in a strong intraday uptrend, which made a Short entry against the trend feel risky on its own.
3. He switched to the 6E Futures footprint (rather than the Forex chart) specifically to see split Bid/Ask volume and Delta, which Forex data doesn't provide.
4. At the Resistance level, he spotted a Price/Delta divergence: price was still climbing, but Delta was falling — meaning aggressive Sellers were quietly building even as price ticked up. He treats this divergence as one of his favorite trade confirmations.
5. He entered Short on that signal and took a modest 10-pip Take Profit quickly, reasoning that pushing for more against a strong prevailing uptrend was not worth the added risk.
6. The trade worked as expected — price reversed shortly after the divergence appeared, validating the read.

## Key Takeaways
1. Footprints show executed Bid/Ask detail per price level — always read Green/Red as a rough Buyer/Seller strength signal, not an absolute one.
2. The HVN (black outline) marks the price within a footprint where institutions were most active; stacked HVNs across footprints upgrade a level's importance.
3. Delta divergence (price direction disagreeing with Delta sign) is a reversal warning — but trust it far more in trending conditions than in rotations.
4. Keep your footprint summary panel minimal: Delta, Cumulative Delta, Volume are enough for most decisions.
5. Pair the footprint (granular) with the daily Volume Profile (big picture) rather than relying on either alone.

## Connects To
- **Ch 2**: Market Participants supplies the passive/active lens needed to interpret Green/Red cells correctly.
- **Ch 4**: Special Features formalizes the "yellow HVN" idea into the Multiple Node setup and introduces Cumulative Delta in full.
- **Ch 10**: Confirmation Setup #4 (Cumulative Delta Divergence) is the same Price/Delta divergence logic applied specifically at Support/Resistance zones.
