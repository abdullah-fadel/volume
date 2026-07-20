# Chapter 14: Finding Your Style

## Core Idea
The same three Volume Profile setups apply unchanged across intraday, swing, and long-term investing — the only things that change per style are the timeframe, instrument selection, and how Stop-loss/Profit Target values are sized.

## Frameworks Introduced
- **ATR-based intraday SL/PT sizing**: use a long-period (e.g., 200) ATR on the daily timeframe over 300-500 days to get average daily volatility in pips (ATR value × 10,000), then set intraday SL/PT at roughly 10-20% of that average daily ATR.
  - Worked figure: ATR ≈ 0.0085 on EUR/USD → 85 pips average daily volatility → intraday SL/PT range ≈ 8.5-17 pips.
- **Swing SL/PT sizing**: base primarily on Price Action and volume-zone width rather than a strict ATR formula, but keep it loosely anchored to roughly 50-400% of average daily ATR (0.5x-4x daily volatility) as a sanity range; actual SL is often placed at the far edge of the relevant volume-based S/R zone, in a low-volume area behind a volume cluster.
- **Long-term SL/PT sizing**: hundreds to low-thousands of pips, placed behind a strong barrier (typically a low-volume area behind a strong volume cluster); author targets roughly a 1:1 risk-reward ratio and picks zones consistent with that ratio.

## Key Concepts
- **Intraday timeframe**: 5-minute to 1-hour charts (author prefers 30-minute).
- **Swing timeframe**: 1-hour to daily (author prefers 240-minute/4-hour and daily).
- **Long-term timeframe**: weekly to monthly.
- **Swap/rollover fee**: interest-rate differential charged or paid for holding a forex position overnight; can meaningfully erode long-term positions held through sideways periods, especially if negative — check a broker's Swap Calculator before committing to long-term currency trades.
- **Instrument fit by style**: intraday needs high liquidity/tight spreads (author's default is EUR/USD, then other USD majors; cross pairs avoided for cost reasons; indexes like S&P 500/DAX and oil also usable). Swing and long-term trading can use almost any instrument since spread/commission cost matters far less relative to the larger SL/PT distances.

## Mental Models
- Treat "style" as a dial on the same underlying method, not a different system — pick a timeframe/instrument combination that fits your schedule and risk tolerance, then apply the identical Volume Profile setups.
- Size positions to the SL distance, not the other way around — a wider long-term SL (e.g., 600 pips) requires reducing position size to stay within a fixed account-risk percentage.

## Anti-patterns
- **Daytrading cross pairs (non-USD pairs)**: trading costs are typically too high to overcome for intraday trading.
- **Using a fixed pip SL/PT regardless of volatility**: the author explicitly ties SL/PT sizing to ATR-derived volatility rather than a flat number.
- **Ignoring swap costs on long-held currency positions**: a negative swap held for months during a sideways market can meaningfully erode returns.
- **Sizing a large-SL trade at the same lot size as a small-SL trade**: risks exceeding the account risk budget; position size must be recalculated for every SL distance.

## Worked Example
Swing trade, EUR/USD daily chart: entry based on Volume Setup #2 (Trend setup) in confluence with the Support-becomes-resistance Price Action setup (Ch4 + Ch13). Stop-loss was placed tightly, just below the volume cluster that anchored the entry, because the author places stops in low-volume areas rather than in the middle of a defended zone. Long-term example: a short position on AUD/USD, analyzed on a Monthly chart using Volume Setup #2, carried a 600-pip Stop-loss placed behind a strong volume-cluster barrier, with position size reduced accordingly to stay within the author's 1-5%-of-account risk-per-trade guideline.

## Key Takeaways
1. The three Volume Profile setups (Ch13) don't change across styles — only timeframe, instrument, and SL/PT sizing do.
2. Use ATR-derived average daily volatility as the sizing anchor for intraday SL/PT (roughly 10-20% of ATR); loosen this to a wider 50-400% range for swing, and size long-term SL/PT off S/R zone structure directly.
3. Match instrument choice to trading cost sensitivity: tight-spread majors for intraday, almost anything for swing/long-term.
4. Always recalculate position size for the specific SL distance to keep risk per trade within a fixed account percentage (author's guideline: 1-5%).
5. Check swap costs before holding currency positions long-term.

## Connects To
- **Ch13**: the three setups applied here across styles.
- **Ch19 (Money Management)**: the risk-per-trade percentage and position-sizing discipline referenced here is developed fully there.
