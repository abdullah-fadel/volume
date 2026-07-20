# Chapter 17: Money Management

## Core Idea
Even a great VWAP strategy can lose money without disciplined money management — the author gives a simple backtested-drawdown formula for sizing risk per trade, insists on fixed (not feel-based) position sizing, and offers his free Trade Manager tool to automate both.

## Frameworks Introduced
- **Risk per trade formula**: derive a percentage-of-account risk per trade from your strategy's worst backtested losing streak, padded for real-world conditions.
  - When to use: before trading any strategy live, as the foundational money-management calculation.
  - How (four steps): (1) Backtest the strategy to find its worst historical drawdown, expressed as a number of consecutive losing trades. (2) Pad that number ~20% to account for real trading being somewhat worse than backtested conditions (worst streak × 1.2). (3) Decide your personal maximum tolerable account drawdown percentage (varies by risk tolerance — the author notes a young ambitious trader might accept 50%, an experienced trader with a large account might be uncomfortable even at 10%; his own worked example uses 25%). (4) Risk per trade = max tolerable drawdown % ÷ padded losing streak. Worked example: 6 consecutive losses backtested → ×1.2 = 7.2, rounded to 7 → 25% ÷ 7 = 3.6% risk per trade.
- **Position sizing (fixed, not feel-based)**: use the same risk percentage on every trade, regardless of how confident you feel about a given setup.
  - When to use: every trade, without exception, once your risk-per-trade percentage is set.
  - How: apply the same account-percentage risk to every trade → let Stop Loss/Take Profit pip distance vary trade-to-trade, but never let the risked percentage itself vary → explicitly reject the alternative of sizing up on "high confidence" trades and down on "unsure" trades, for two stated reasons: feelings aren't a reliable, measurable input, and the author's own experience is that seemingly "perfect" trades fail just as often as ordinary-looking ones.
  - Why it works: consistency removes an unreliable, emotion-driven sizing variable from the system entirely.
- **Trade Manager (software)**: the author's free tool that automates position-size calculation and several related trade-management tasks.
  - When to use: to remove the manual math and friction of applying the Risk-per-trade and Position-sizing rules on every trade.
  - How / features: (1) calculates lot size automatically from a set risk percentage; (2) lets you adjust TP/SL with one click and see live RRR impact; (3) simplifies placing Limit orders in two clicks, with proximity alerts; (4) moves SL to breakeven or the first reaction point in one click; (5) allows partial position closure in one click; (6) "Secure Limit Orders" — automatically pulls Limit orders a few minutes before major macro news releases and restores them afterward, protecting against news-driven spike fills. Free, no limitations, lifetime license (link: mt4trademanager.com).

## Key Concepts
- **Drawdown**: the largest peak-to-trough loss (measured here as consecutive losing trades) a strategy produced during backtesting.
- **1.2x real-world padding factor**: the author's stated adjustment for the assumption that live trading conditions run roughly 20% worse than backtested ones.
- **Max tolerable drawdown %**: a personal, subjective ceiling — how much total account loss you can absorb without significant distress — that varies by risk appetite and account size/experience.
- **Fixed risk percentage**: the non-negotiable output of the formula, applied uniformly regardless of per-trade confidence level.

## Mental Models
- Treat the risk-per-trade formula as translating your personal loss tolerance into a single repeatable number, rather than deciding risk trade-by-trade from feel.
- Think of "confidence-based sizing" as reintroducing exactly the kind of subjective judgment the rest of this book's frameworks (VWAP, Price Action, Volume Profile, Order Flow) are designed to replace with structure — money management should be equally systematic.

## Anti-patterns
- **Sizing positions by gut confidence**: explicitly rejected — the author states even trades that look flawless fail just as often as ordinary ones, and confidence isn't a measurable, reliable sizing input.
- **Skipping the backtest step**: the entire risk-per-trade formula depends on knowing your strategy's actual worst losing streak — sizing without that data means guessing at your true drawdown risk.
- **Ignoring the 20% real-world padding**: using the raw backtested worst streak without padding likely underestimates true worst-case risk.

## Worked Example
A trader backtests their VWAP strategy and finds a worst losing streak of 6 consecutive losses. Padding this by 20% (6 × 1.2 = 7.2, rounded to 7) gives the expected worst-case real-world losing streak. The trader decides they're comfortable with a maximum 25% account drawdown. Dividing: 25% ÷ 7 = 3.6% risk per trade. This 3.6% figure is then applied identically to every trade going forward, regardless of how strong any individual VWAP + confluence signal looks — the same percentage, with SL/TP pip distances varying trade to trade based on the specific setup (per Ch14–Ch15), but the risked percentage of account equity never changing.

## Key Takeaways
1. Risk per trade = (max tolerable drawdown %) ÷ (backtested worst losing streak × 1.2).
2. Position size must be fixed across all trades at that risk percentage — never adjusted for how confident a trade "feels."
3. Backtesting is a prerequisite, not optional — the whole formula depends on knowing your real worst-case losing streak.
4. The author's free Trade Manager tool automates position sizing, TP/SL adjustment, Limit order placement, breakeven/reaction-point SL moves, partial closes, and automatic Limit-order protection around major news releases.
5. Max tolerable drawdown % is a personal risk-tolerance input — there's no universal "correct" number; it should reflect what you can absorb without abandoning the strategy under stress.

## Connects To
- **Ch14–Ch15**: Take Profit and Stop Loss placement determine the pip distance for each trade; this chapter determines the account-percentage risked at that distance, independent of the specific barrier method used.
- **Ch6**: the Trade Manager's automatic Limit-order protection around major news releases directly complements the macro-news anchoring and confirmation caution discussed there.
- **trader-dale-price-action skill**: that book's money-management chapter covers the same risk-per-trade formula and a fuller trading-psychology framework (Cycle of Doom and Despair, four kinds of trades) in more depth — this chapter presents the VWAP book's own, more compact version of the same core formula.
