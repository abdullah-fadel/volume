# Chapter 6: Anchoring VWAP to Macro News Candle

## Core Idea
Anchor VWAP at the candle where genuinely game-changing macro news was released — not merely "high-impact" by a calendar's generic label — because other traders will orient their decisions around that same moment, making it a strong reference point.

## Frameworks Introduced
- **News-candle-anchored VWAP**: VWAP calculated starting from the candle where a truly market-moving macro news release occurred.
  - When to use: short-term/intraday trading, author's own range is 5-minute to 30-minute timeframes; works best on instruments sensitive to the specific news released (e.g., EUR/USD to Fed/ECB decisions, USD/JPY to BoJ decisions).
  - How: identify candidate high-impact news events (e.g., via forex-factory.com's red/orange/yellow severity coloring, or TradingView's "economic events on chart" feature) → filter further by actual market reaction, not label alone — the same "high-impact" tag can cover both a non-event (e.g., generic Unemployment Claims) and a true game-changer (e.g., Monetary Policy Statement) → confirm the news candle actually shifted sentiment (started a new trend), not just caused a brief spike that reverted → anchor VWAP at that candle → trade subsequent pullbacks to the line as continuation entries in the new trend's direction.
  - Why it works: strong news creates a shared "before/after" reference moment that other traders orient around; VWAP anchored there shows whether current price is above or below the "fair" average since sentiment actually changed.

## Key Concepts
- **Forex Factory severity coloring**: yellow (low-impact), orange (medium-impact), red (high-impact) — used as a first filter, but not sufficient alone since red-tagged events vary widely in actual market-moving power.
- **Priority macro events for this anchor**: Rate Decision / Minimum Bid Rate (+ press conference), FOMC Meeting / Monetary Policy Statement (+ press conference), CPI, GDP, NFP, Unemployment Rate, major-economy leader speeches directly addressing their economy/currency.
- **Game-changing vs. noise news**: the deciding test is whether the news candle kickstarted durable directional action (a new trend) — a brief spike that fully reverts back to the prior range is explicitly not a valid anchor candidate.
- **TradingView economic-events overlay**: a chart feature (enabled via "economic events on the chart" in settings) that marks news release times directly on the price chart, making candidate anchor candles easy to locate.

## Mental Models
- Treat the Forex Factory color tag as a coarse pre-filter only; the real filter is "did this news actually change what happens next," judged by the price action that followed, not the label.
- Think of a validated news-candle anchor the same way as a trend-start anchor (Ch5) — it works because it's a shared reference point other market participants are also orienting around.

## Anti-patterns
- **Anchoring to every red-tagged news event indiscriminately**: many "high-impact" events (e.g., Unemployment Claims) rarely move price meaningfully — anchoring there produces a low-value line.
- **Anchoring before confirming the reaction held**: a strong-looking spike that fully reverts within the same session was not a sentiment-changing event — don't anchor there even if the initial candle looked dramatic.
- **Applying this anchor on instruments the news doesn't affect**: match the news source to the instrument (e.g., BoJ decisions to USD/JPY/other JPY pairs, Fed decisions to USD pairs) rather than anchoring generically.

## Worked Example
USD/JPY, 30-minute chart: the "BoJ Interest Rate Decision" produces a strong bullish candle that clearly marks the start of a new uptrend — a genuine game-changer, not a brief spike. The author anchors VWAP at that exact candle. The first pullback to the resulting VWAP line offers a strong long entry, capturing real momentum from the news-driven trend. Two further pullbacks later in the sequence still produce reactions and valid long entries, but by then the initial momentum has faded — these become quick in-and-out trades rather than trades worth trailing. Eventually price drops below the VWAP, flipping it into resistance, and offers one further quick short opportunity from the flipped line — the same broken-VWAP role-reversal mechanic seen with other anchor types (Ch3, Ch5).

## Key Takeaways
1. Filter macro news anchors in two steps: severity tag (red/high-impact) first, then actual observed market reaction (durable trend start, not a brief spike) second.
2. Priority news list for this anchor: Rate Decisions, FOMC/Monetary Policy Statement, CPI, GDP, NFP, Unemployment Rate, major-economy leader speeches.
3. Use forex-factory.com and/or TradingView's economic-events overlay to locate candidate candles quickly.
4. Best suited to short-term timeframes (5-min to 30-min); match the news source's currency/instrument to the chart you're trading.
5. Later pullbacks along the same anchored line can fade in strength as momentum decays — treat them as quick trades rather than assuming the same power as the first reaction.

## Connects To
- **Ch5**: shares the "trend-start" anchoring logic — a validated news candle often *is* the trend-start candle.
- **Ch3**: the broken/flipped VWAP mechanic recurs identically when price crosses through a news-anchored line.
- **Ch16 (Trailing Your Trade)**: the fading-momentum pattern here (later pullbacks = quicker, non-trailed trades) is directly relevant to deciding when to trail vs. take a fast exit.
