# Chapter 11: VWAP Trend Strategy

## Core Idea
When the 1st VWAP deviations are moving vertically (a trending market), trade pullbacks to whichever deviation band price is riding — the upper deviation acts as dynamic support in an uptrend, the lower deviation as dynamic resistance in a downtrend — which lets you enter a trend on a pullback with positive Risk-Reward and room to trail.

## Frameworks Introduced
- **VWAP Trend strategy**: enter pullbacks to the trending 1st-deviation band (upper band in an uptrend, lower band in a downtrend), riding the deviation as it moves vertically with the trend.
  - When to use: only when the 1st deviations are moving vertically (at least one clearly trending) — the counterpart to the VWAP Rotation strategy (Ch10), which requires horizontal deviations instead.
  - How, Long scenario: confirm the upper 1st deviation is trending upward (moving vertically) → confirm price is positioned above the upper deviation → enter Long when price pulls back down and touches the upper deviation from above. How, Short scenario: confirm the lower 1st deviation is trending downward → confirm price is positioned below the lower deviation → enter Short when price pulls back up and touches the lower deviation from below.
  - Why it works / advantage: because this is a trend-following entry, it naturally offers a positive Risk-Reward Ratio and room to trail the Take Profit rather than taking a fixed target — the goal is to catch a pullback into an established trend and ride as much of the move as possible.

## Key Concepts
- **Deviation-as-dynamic-S/R**: unlike the Rotation strategy where both bands act as static-ish channel edges, in the Trend strategy the *trending* band (upper in an uptrend, lower in a downtrend) becomes the active pullback-entry reference — the opposite band is not used for entries here.
- **Deviation development lag**: at the start of a new date-anchored VWAP period (e.g., start of year), the 1st deviations are often too close together to trade — the author explicitly waits for them to develop and clearly separate before applying this strategy.
- **Trend strategy vs. Rotation strategy hand-off**: the same chart can move between the two Strategy #2 variants as regime changes — a market rotating (Ch10) that breaks its deviation channel becomes a Trend strategy candidate, and vice versa.
- **Positive RRR / trailing advantage**: distinguishes this strategy from the Rotation strategy, where Take Profit is a fixed target (VWAP line) — here, because you're trading with the trend, the position can be trailed for extended profit.

## Mental Models
- Think of the trending deviation band as "VWAP's more aggressive cousin" — while VWAP itself represents the broad average, the trending deviation band represents the edge of where the trend-following crowd is actively defending.
- Use deviation vertical slope as your green light: don't force Trend-strategy entries while the bands are still flat or only just beginning to separate.

## Anti-patterns
- **Entering before the deviations have clearly developed**: multiple examples in the source show the strategy only becoming viable once deviations had enough time (and often a catalyst like a macro event) to separate and confirm a real trend.
- **Trading the non-trending band**: in an uptrend, only the upper deviation is the active entry reference — the lower deviation isn't a valid pullback level for the Trend strategy.
- **Treating this as fixed-target trading**: unlike the Rotation strategy's VWAP-line Take Profit, the Trend strategy is meant to be trailed — capping it with a fixed target undercuts the whole rationale for using it (see Ch16 for trailing methods).

## Worked Example
GBP/USD, Daily chart with Yearly VWAP: at the start of the year, the 1st deviations sit too close together to trade — no clear trend signal yet. A significant macroeconomic event then triggers a strong, sustained sell-off, and the deviations begin moving vertically, confirming a genuine downtrend and activating the VWAP Trend strategy. From that point, the lower 1st deviation becomes the active short-entry reference: as price (trading below the lower deviation) pulls back up to touch it from below, three separate Short trades trigger off that band during the ongoing sell-off — each entered on a pullback into an already-established, catalyst-confirmed trend.

## Key Takeaways
1. Trade the trending band only: upper deviation for Long pullbacks in an uptrend, lower deviation for Short pullbacks in a downtrend.
2. Confirm vertical deviation movement (a real trend) before entering — flat/undeveloped deviations are not tradeable with this strategy.
3. Advantage over the Rotation strategy: positive RRR and a trailable position, since you're trading with the trend rather than a range.
4. Deviations often need time (and sometimes a catalyst like a macro news event) to separate into a clear trend after a new date-anchor period starts.
5. The same instrument can hand off between Rotation strategy (Ch10) and Trend strategy (this chapter) as the 1st deviations' slope changes.

## Connects To
- **Ch10**: the direct counterpart strategy — same 1st-deviation tool, opposite market regime (rotation vs. trend), with a live hand-off mechanic between them.
- **Ch6**: macro news events are shown here as a common catalyst that kicks deviations from flat into a clear vertical trend.
- **Ch16 (Trailing Your Trade)**: this strategy's core advantage — a trailable position — is where that chapter's trailing techniques apply most directly.
