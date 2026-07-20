# Chapter 12: Building a Portfolio

## Core Idea
A long-term stock portfolio here means roughly 20 fundamentally-qualified stocks, each capped at a fixed 4% of capital split across two Volume-Profile Supports, with a mandatory 20% cash reserve for extreme discounts, no leverage, no Stop Loss, and execution via limit orders so the whole system runs on autopilot rather than active monitoring.

## Frameworks Introduced
- **Full pipeline recap (how ~65 candidates become ~20 portfolio positions)**: fundamental screening (Ch5–Ch7) across 4–5 sectors might yield ~65 qualifying stocks; deliberately cut entire sectors you have structural reservations about (e.g., Financial, Technology) even if some of their stocks passed, narrowing to ~40; apply Volume Profile timing (Ch9–Ch10) — only about half of stocks will show a clean, identifiable Support, narrowing to ~20 final candidates.
- **Fixed position sizing — 4% per stock, split into two entries**: allocate an equal 4% of total capital to each of ~20 stocks (never overweight "favorites" — the author notes favorites often underperform other list members). Split each 4% into two 2% tranches at two different Volume-Profile Supports: buy the first 2% when price hits the shallower Support, buy the remaining 2% if price drops further to the second, deeper Support. With ~20 stocks × 4% each, full deployment at all first Supports uses about 80% of capital.
- **20% Cash Reserve**: hold back 20% of total capital, undeployed, specifically for a 3rd, much deeper "catastrophic" Support per stock (identified during charting, alongside the two normal Supports) — reserved for genuine market-wide crashes when otherwise-good stocks become extremely cheap. Not meant to be used often; explicitly *not* a Martingale (increasing risk after losses) because the trigger is a fundamentals-unchanged price discount, not a losing streak.
- **No Leverage**: never use margin/leverage for this style — a market-wide crash (which the strategy explicitly plans to buy into) could wipe a leveraged account before the recovery happens.
- **No Stop Loss**: deliberately omitted for this style — since no leverage is used, the effective worst case is the stock's Book Value (Ch6), which functions as a natural floor; a hard price-based Stop Loss would risk being shaken out right before a legitimate recovery.
- **Limit Orders over active monitoring**: place limit (pending) orders at each identified Support so entries execute automatically, without watching ~20+ charts daily; alerts (via broker or a mobile app) are the fallback if you prefer to manually confirm before entering.
- **Free capital allocation while waiting**: capital not yet deployed at a Support should not sit idle — allocate it to corporate bond ETFs (low/negative correlation to stocks, so it's available exactly when stocks are cheap) rather than dividend stocks (which fall together with the rest of the market in a broad sell-off, defeating the purpose of "dry powder").

## Key Concepts
- **The "Standard Portfolio Theory" critique**: the author explicitly rejects Beta-based risk models, which would flag a fast-falling stock as newly "risky" and could lead a Beta-following manager to buy an already-overpriced stock at its peak (when Beta looks low) instead of a fundamentally same stock at a discount (when Beta looks high).
- **Stocks vs. Stock CFDs**: CFDs charge a daily overnight holding fee ("swap") even without leverage, which compounds destructively over a multi-year holding period — the author recommends owning actual shares, not CFDs, for this style.
- **Fractional shares**: a workaround for smaller accounts where a single expensive stock (e.g., a $1,000/share name) would otherwise breach the 2–4% per-position sizing rule — buy a fractional dollar amount instead of a whole share.

## Mental Models
- Treat the whole portfolio-construction pipeline as a funnel: ~65 fundamentally-passable stocks → ~40 after sector pruning → ~20 after Volume Profile timing confirms a real Support — each stage removes candidates for a *different* reason (sector conviction, then technical clarity).
- Treat the 20% reserve as "insurance capital for the best sale of the cycle," not spare cash to be casually deployed.

## Anti-patterns
- **Overweighting favorite stocks**: equal-weight every position; the author notes personal favorites have not reliably outperformed the rest of the list.
- **Using leverage or CFDs "just for convenience"**: leverage risks account-wiping in the crash scenarios this strategy is specifically designed to buy into; CFDs' daily swap fee quietly erodes multi-year returns.
- **Parking reserve cash in dividend stocks**: dividend stocks fall in the same broad sell-offs that create the buying opportunities the reserve is meant for — defeats the purpose of holding dry powder.
- **Checking the portfolio and charts too often**: encourages emotional, plan-breaking decisions; the system is built around limit orders and periodic (roughly weekly) review, not daily monitoring.

## Worked Example
With $100,000 in capital and 20 qualifying stocks, each stock receives $4,000 (4%), split into two $2,000 tranches at two Volume-Profile Supports. A separate $20,000 (20%) is held in reserve for a 3rd, deep "catastrophic" Support on select stocks. Illustration: a stock currently at $100 might have Support #1 at $70, Support #2 at $40, and a catastrophic Support #3 at $10. If price reaches $70, the first $2,000 buys ~28 shares. If it continues to $40, the second $2,000 buys ~50 shares. In the rare case it collapses to $10 (fundamentals still intact), the $20,000 reserve could buy ~200 shares at that price — the same dollar amount buying dramatically more shares the cheaper the stock gets, which is the entire logic of treating a crash as a buying opportunity rather than a reason to panic.

## Key Takeaways
1. Target roughly 20 fundamentally-qualified, Volume-Profile-confirmed stocks, each capped at a fixed 4% of capital (never overweighted by preference).
2. Split each position's 4% into two 2% entries at two separate Supports; keep a 20% reserve specifically for a rare, much deeper 3rd Support.
3. No leverage, no Stop Loss — Book Value is the natural worst-case floor for this style.
4. Use limit orders (or alerts) so the strategy runs without daily active monitoring.
5. Park undeployed capital in corporate bond ETFs, not dividend stocks or cash, so it's available exactly when stock prices are cheapest.
6. Avoid Stock CFDs for long-term holding — the daily swap fee compounds against you over years; fractional shares solve the "expensive stock, small account" problem instead.

## Connects To
- **Ch7**: the ~65-stock starting point of the funnel is the direct output of the sector-by-sector screening process there.
- **Ch10**: the two-Support split-entry sizing logic here is a direct extension of the split-entry technique introduced for individual trades.
- **Ch11**: capital freed by trimming overextended positions (Ch11) flows back into this same reserve/bond-ETF allocation system.
- **Ch13**: several Common Mistakes (checking charts too often, betting too much on one stock/sector, using leverage-adjacent products) are the negative-space restatement of the rules in this chapter.
