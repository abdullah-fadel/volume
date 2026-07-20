# Chapter 10: Strategy #2 — Reactions to 1st VWAP Deviations, and the VWAP Rotation Strategy

## Core Idea
1st VWAP deviations ("bands" plotted above and below VWAP) reveal market regime at a glance — horizontal deviations mean rotation, vertical deviations mean trend — and each regime gets its own dedicated strategy: VWAP Rotation strategy for sideways markets (this chapter), VWAP Trend strategy for trending markets (Ch11).

## Frameworks Introduced
- **1st VWAP deviations ("bands")**: two lines plotted above and below VWAP, calculated from it, that move alongside VWAP as standard deviations.
  - When to use: as a fast regime-read tool — horizontal deviations = rotation (Ch10's territory); at least one deviation moving vertically = trend (Ch11's territory). The author's stated setting: 1st deviations are used exclusively with date-anchored VWAP (Daily/Weekly/Yearly, Ch3), not with swing-point/trend-start/news/volume/gap/earnings anchors — not incorrect to combine, just not his practical preference. Color convention: date-anchored VWAP + deviations in yellow/grey; anchored VWAP without deviations in blue.
  - How: plot the 1st deviation bands on a date-anchored VWAP → observe whether the bands move horizontally (rotation) or vertically (trend) → note this read is "user-friendly but not foolproof" — a quick-glance regime filter, not a precise signal.
- **VWAP Rotation strategy**: trade the two 1st-deviation bands as Support (lower band) and Resistance (upper band) while the market is in a sideways/rotation phase, taking profit at the VWAP line itself.
  - When to use: only while the 1st deviations are moving horizontally (confirmed rotation) — the strategy stops being valid the moment the deviations start trending or price closes outside the channel.
  - How: confirm the deviations are moving horizontally → enter Long when price touches the lower 1st deviation from above (acting as Support) → enter Short when price touches the upper 1st deviation from below (acting as Resistance) → set Take Profit at the VWAP line (the mid-channel reference) → intraday preference: Weekly VWAP (date-anchored) on a 30-minute chart (author finds it less volatile/more reliable than Daily VWAP on 5-minute); swing preference: Yearly VWAP on a Daily chart.

## Key Concepts
- **Regime read via deviation slope**: horizontal 1st deviations = rotation; vertical 1st deviations (at least one band) = trend. This single visual cue routes you to Ch10 (Rotation) or Ch11 (Trend).
- **Channel exit = strategy invalidation**: once price closes outside the 1st-deviation channel, the Rotation strategy is no longer valid — that is precisely the trigger to switch to the VWAP Trend strategy (Ch11).
- **VWAP as Take Profit**: in the Rotation strategy, the VWAP line itself (not a fixed pip target) is the designated Take Profit for both Long and Short entries.
- **Deviations require development time**: newly-plotted deviations often start as a tight channel close together; the author advises patience, waiting for the bands to widen and establish a clear rotation before trading them.

## Mental Models
- Use the deviation-slope read as your first "which strategy am I in" filter every session — before looking for any entry, check whether the bands are flat (Rotation) or angled (Trend).
- Treat a price close outside the 1st-deviation channel as a hard regime-change signal, not noise to fade — it marks the live handoff from Rotation strategy to Trend strategy on the same chart.

## Anti-patterns
- **Trading the Rotation strategy on a market that has already started trending**: the strategy explicitly requires horizontal deviations; forcing rotation-style entries once bands start slanting produces the "less favorable" trades the author flags (e.g., a short where price moves significantly beyond the deviation).
- **Trading newly-formed, still-tight deviations**: entering before the channel has developed and widened risks trading noise rather than a real rotation range.
- **Ignoring a channel breakout**: continuing to fade the deviation bands after price has closed outside them means missing the regime change to a trending market.

## Worked Example
USD/CAD, Daily chart with Yearly VWAP: the market starts in an uptrend (not tradeable with the Rotation strategy), then transitions into a rotation phase as the 1st deviations flatten out. Once rotation is confirmed, two Long entries trigger off the lower deviation and two Short entries trigger off the upper deviation, each targeting the VWAP line for Take Profit. Eventually price closes below the lower 1st deviation — breaking the channel. At that exact point, the author stops applying the Rotation strategy and the chart transitions into VWAP Trend strategy territory (Ch11), illustrating how the same chart, same VWAP, and same deviations can hand off between the two Strategy #2 variants as market regime changes.

## Key Takeaways
1. Check deviation slope first: horizontal = Rotation strategy (this chapter); vertical = Trend strategy (Ch11).
2. Rotation strategy entries: Long off the lower 1st deviation, Short off the upper 1st deviation, both targeting VWAP for Take Profit.
3. Use date-anchored VWAP (Daily/Weekly/Yearly) with deviations, not other anchor types, per the author's stated practical preference.
4. Preferred settings: Weekly VWAP + 30-min for intraday rotation trades; Yearly VWAP + Daily for swing rotation trades.
5. A channel breakout (price closing outside the 1st deviations) ends the Rotation strategy's validity and signals a shift to the Trend strategy on the same instrument.
6. Give newly-plotted deviations time to develop before trading them — don't force entries on a still-tight, undeveloped channel.

## Connects To
- **Ch3**: date-anchored VWAP (Daily/Weekly/Yearly) is the required base for this strategy's deviations.
- **Ch11**: the VWAP Trend strategy is the direct counterpart, triggered the moment deviations stop moving horizontally or price breaks the rotation channel.
- **Ch2**: shares the underlying "touch and enter" logic, applied here to deviation bands instead of the VWAP line itself.
