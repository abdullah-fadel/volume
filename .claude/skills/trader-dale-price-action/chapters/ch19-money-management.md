# Chapter 19: Money Management

## Core Idea
Risk per trade should be derived mathematically from your strategy's backtested worst-case drawdown and your personal drawdown tolerance — not from a round number or a "feeling" about the trade — and Risk-Reward Ratio, position size, and correlation exposure all need their own explicit, fixed rules to keep a good strategy from being undone by poor money management.

## Frameworks Introduced
- **Risk-per-trade sizing formula** (author's exact method):
  1. Backtest the strategy to find the worst historical drawdown (consecutive losing trades).
  2. Apply a safety coefficient (~20%) to account for real trading being worse than backtest — e.g., 6 consecutive losses × 1.2 = 7.2, round to 7.
  3. Decide the maximum account drawdown percentage you can endure while still thinking clearly and sticking to your plan (this is personal — varies by risk tolerance, account size, life stage).
  4. Risk per trade = tolerable drawdown % ÷ worst-case losing streak. Worked example: 25% tolerable drawdown ÷ 7 losses = 3.58% risk per trade.
- **Risk-Reward Ratio (RRR) trade-offs**: RRR compares potential loss to potential gain (e.g., risking 20 pips to make 40 pips = 1:2). The author explicitly challenges the common wisdom of "always use positive RRR," pointing out the mechanical trade-off: stretching RRR to be more positive proportionally lowers your strike rate (e.g., a 60% strike rate at 1:1 degrades to roughly 40% at 1:2 for the same underlying edge). There's also a **time-in-trade risk**: longer holds (needed for a stretched PT) increase exposure to unexpected news/momentum shifts. Author's personal preference: RRR close to 1:1, avoiding both extremes (very negative RRR = small frequent wins but painful rare losses; very positive RRR = big rare wins but a low strike rate that's psychologically hard to sustain through long losing streaks).
- **Fixed position sizing rule**: use the same risk percentage for every trade of a given category — never scale size up because you "feel good" about a particular trade.
  - Category-level variation is fine (e.g., 2% on standard intraday trades, 1% on reversal trades, 3% on swing trades) as long as each category's number stays fixed.
  - High-water-mark rebasing: recalculate the fixed dollar risk only when the account sets a new equity high, not continuously — and explicitly do NOT lower risk % during a drawdown (doing so extends recovery time). E.g., on a $10,000 account risking 2% ($200/trade): a drawdown to $9,000 keeps risking $200; an increase to $11,000 resets the 2% base to the new $11,000 high.
- **Correlation risk control**: when two or more heavily correlated instruments present a similar trade setup at nearly the same time, reduce position size on those trades (rather than skipping or ignoring correlation) since they're likely to move — and resolve — together, effectively doubling exposure to the same underlying driver.

## Key Concepts
- **Drawdown**: the peak-to-trough decline in account balance from a losing streak; central input to the risk-per-trade formula.
- **Strike rate**: the percentage of trades that win; mechanically inversely related to how positive your RRR is, for a given underlying strategy edge.
- **High water mark**: the highest account balance achieved to date; the author's chosen rebasing point for recalculating fixed-dollar risk per trade.

## Mental Models
- Treat "feeling good about a trade" as noise, not signal — the author states plainly that trades that "don't look so perfect" have about the same win rate as the best-looking ones, and is actually wary when a setup looks too perfect.
- Think of RRR choice as a dial between strike rate and payout size, not a search for a "correct" ratio — pick based on your own psychological tolerance for long losing streaks vs. your tolerance for many small losses.
- Treat correlated simultaneous setups as one bigger bet in disguise, not two independent trades — size accordingly.

## Anti-patterns
- **Sizing risk per trade off a round number instead of a backtested drawdown**: skips the actual math connecting your risk tolerance to your strategy's real loss-streak behavior.
- **Lowering position size during a drawdown**: the author explicitly warns this only prolongs the recovery — keep size fixed to the pre-drawdown high-water-mark risk level.
- **Adjusting position size based on "how good a trade looks"**: explicitly rejected — feeling is unmeasurable and, per the author's experience, uncorrelated with actual outcome.
- **Taking full size on two heavily correlated setups simultaneously**: effectively doubles exposure to one underlying driver; the fix is reducing size on both, not ignoring the overlap.

## Worked Example
Correlation risk, AUD/USD and EUR/USD: two visually similar long setups appeared on both pairs at nearly the same time, both USD-driven (broad USD strength was pushing both pairs down against the author's long bias). Both long levels failed to hold as the USD kept strengthening, and both trades ended as losses. Had the author traded full standard size on both, the combined loss would have been double a single full loss; because he reduced size on both correlated positions in advance, the total damage was effectively halved.

## Key Takeaways
1. Derive risk-per-trade from (tolerable drawdown %) ÷ (backtested worst losing streak × ~1.2 safety factor) — not from an arbitrary number.
2. There is no "correct" RRR — moving toward positive RRR trades strike rate for payout size; the author's own default is close to 1:1.
3. Keep position size fixed within each trade category; never scale by feel.
4. Rebase your fixed dollar risk only at new account equity highs; never cut risk % during a drawdown.
5. Cut position size on simultaneous setups across heavily correlated instruments to avoid doubling real exposure.

## Connects To
- **Ch18**: Stop-loss distance decisions there feed directly into the position-size math here.
- **Ch15**: instrument correlation discussed there is the direct input to the correlation risk-control rule here.
- **Ch21 (Backtesting)**: the backtest referenced in the risk-per-trade formula is fully covered there.
