# Chapter 23: BONUS — How I Manage My Intraday Trades

## Core Idea
This chapter is the author's exact personal rulebook — specific numbers, not general principles — for entries, SL/PT sizing, trailing, level validity ("tested" levels), holding duration, gaps, and daily discipline, offered as a concrete reference implementation of everything taught earlier in the book.

## Frameworks Introduced
- **Entry order type selection** (~50/50 market vs. limit split): use MARKET orders specifically when (a) entering against a strong spike move — enter only if the spike is confirmed *not* news-driven (checked via a real-time news service), since a strong spike can offer entry a few pips better than the original level; or (b) price has been rotating near the level creating weak highs/lows (Ch10) — enter during the resulting small spike/rejection for a better price than a static limit order.
- **Fixed SL/PT setting (author's own default)**: 10-pip Profit Target, 12-pip Stop-loss, applied uniformly across his four intraday pairs (EUR/USD, AUD/USD, USD/CAD, USD/JPY). Stated reasons:
  1. Minimizes time-in-trade risk (shorter holds = less exposure to surprises).
  2. A 10-pip counter-trend correction is statistically much more likely than a 20-pip one (which would effectively end the prevailing short-term trend).
  3. Empirically, 10 pips is an adequate reaction size for his levels, supporting roughly a 70% long-run strike rate.
  4. Near-1:1 RRR avoids both extremes (devastating losses from skewed-negative RRR; reduced strike rate and "Murphy's law" risk of missing the one big winner from skewed-positive RRR).
  - Explicit caveat: other traders in his course use different settings (e.g., 20/20) successfully — the specific numbers matter less than consistent application of whatever rule you pick.
- **Trailing Stop-loss (Neutral style, Ch18) with situational triggers**: move SL to the reaction point once in profit, at slightly different profit thresholds depending on context:
  - Counter-trend trade: secure at +7 pips (more conservative/faster, since counter-trend is riskier).
  - With-trend trade: secure at +7.5 to +8 pips (more room, since trend-aligned trades are lower risk).
  - No clear trend: secure around +7.5 pips.
  - Sharp, precise reaction right at the level within 1-2 minutes: secure sooner, at +7 pips, since a sharp reaction confirms the aggressive participants are present and a return to that reaction point would mean the counter-move is too strong to trust.
- **"Tested level" validity check**: a level that's already produced a strong reaction nearby is treated as used up and discarded, based on five judgment factors:
  1. Distance/size of the prior reaction — a reaction of 8+ pips starting within 0-3 pips of the level generally invalidates it, unless the level is otherwise very significant.
  2. Zone width (checked via Volume Profile, Ch12) — a narrow, tightly-pinpointed zone tolerates a near-miss test better than a wide zone; if a wide zone was tested anywhere within it, treat the whole zone as used.
  3. Reaction sharpness — a slow, low-energy turn before the level leaves it more valid than a sharp, swift, high-volatility reaction.
  4. Trend alignment — more benevolent/aggressive about reusing a tested level when trading with the trend; more willing to discard when trading counter-trend.
  5. Discretion — acknowledged as an irreducibly judgment-based factor; no rule set fully replaces experience here.
  - Scope: this tested/untested filtering is only applied during actively-monitored sessions (EU/US); during the Asian session the author just uses plain limit orders on all valid levels without this filter.

## Key Concepts
- **Daily close (5:00 PM Eastern) handling**: avoid holding through the futures-close/spot-rollover spread-widening window unless the position is currently near breakeven (far from both PT and SL, so widened spreads pose little risk); exit if close to PT or SL before the widening hits.
- **Weekly close handling**: always exit all intraday positions before the weekend — a weekend gap on tight intraday stops is an unnecessary, undiversifiable risk with no offsetting benefit for a day trader.
- **Gap-at-open entries**: treated as a bonus confirmation, not a red flag — markets tend to fill opening gaps, so a gap landing right on a volume-based level is welcomed (after waiting briefly for the initially wide open-spread to tighten).
- **Level permanence**: levels are never deleted or modified once created, regardless of how much time or distance has passed — the author notes markets can react to levels 30-40+ days old, and offers a documented 40-day-old USD/JPY reaction as evidence.
- **Take every valid setup, regardless of the day's running P/L**: no discretionary stop after a good run ("I've made enough today") and no discretionary stop after a bad run ("I can't take another loss") — the author explicitly trades every valid level every day, citing both a real day that recovered from 2 early losses to a net winning day, and the broader point that a small number of days often generate a disproportionate share of monthly profit, which you can't predict in advance and therefore must always be positioned to capture.

## Mental Models
- Treat specific number choices (10/12 pips, 7-8 pip trail trigger, etc.) as *examples of a consistently-applied rule*, not universal constants — the author is explicit that consistency of application matters more than the exact numbers.
- Use Volume Profile zone width as the objective proxy for "how strict should my tested-level rule be" — narrow zone = stricter near-miss tolerance is unnecessary; wide zone = treat any test within it as using up the whole zone.
- Treat every valid level as an independent trial in a long-run statistical process — daily P/L so far is not information that should change whether you take the next valid setup.

## Anti-patterns
- **Stopping trading after a good run ("I've made enough today")**: forfeits expected value from the remaining valid setups and specifically risks missing the rare outsized days that drive a large share of monthly profit.
- **Stopping or downsizing after a bad run ("I can't take another loss")**: the author's own example (2 early losses recovered by 3 winners into a net-positive day) is offered as direct evidence against this instinct.
- **Holding intraday positions through the weekly close**: unnecessary, undiversifiable gap risk with tight stops.
- **Reusing a level after a strong, sharp, close reaction already invalidated it** (especially counter-trend): treated as a lower-quality repeat trade.
- **Deleting or "cleaning up" old unused levels**: the author deliberately keeps levels indefinitely since the market can and does react to levels weeks later.

## Worked Example
Market-order spike entry: watching a strong, non-news-driven spike move into a level on the 1-minute chart, the author entered with a market order and achieved an entry 6 pips better than the original static level — illustrating the first market-order use case above. Daily-discipline example: after opening a trading day with 2 losing trades, the author continued trading at full size rather than stopping or downsizing, took 3 subsequent winners, and closed the day net positive — directly demonstrating the "take all valid setups" rule against the instinct to protect against further losses after a rough start.

## Key Takeaways
1. Use market orders for spike entries (news-filtered) and rotation/weak-high-low entries; limit orders otherwise — roughly a 50/50 split in practice.
2. Pick a consistent SL/PT ratio near 1:1 (author's own: 10 PT / 12 SL) and apply it uniformly — the specific numbers matter far less than consistent execution.
3. Trail SL to the reaction point around +7 to +8 pips profit, adjusting the trigger slightly by trend context (tighter counter-trend, looser with-trend).
4. Discard a level after a strong nearby reaction has already "tested" it — judge validity using reaction size, zone width (via Volume Profile), reaction sharpness, and trend alignment.
5. Exit before the weekly close always; exit before daily-close spread widening only if near PT/SL.
6. Treat a gap landing on your level as a bonus confirmation, not a reason to hesitate.
7. Never delete old levels — the market can react to them a month or more later.
8. Take every valid setup every day regardless of the running daily P/L.

## Connects To
- **Ch18**: this chapter's SL/PT and trailing rules are a concrete instantiation of the general Position Management frameworks there.
- **Ch10, Ch12**: the tested-level filter directly reuses the weak-high/low concept and Volume Profile zone-width reasoning from those chapters.
- **Ch20**: "take all valid setups" is the practical trading-floor expression of that chapter's discipline-over-outcome psychology.
