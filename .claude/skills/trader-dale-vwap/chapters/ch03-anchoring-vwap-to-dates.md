# Chapter 3: Anchoring VWAP to Dates (Daily, Weekly, Yearly VWAP)

## Core Idea
Calendar-anchored VWAP comes in three flavors — Daily (start of day), Weekly (start of week), Yearly (start of year) — and each fits a different trading style: Daily for intraday scalping, Weekly as the author's favorite intraday reference, Yearly for swing/long-term positioning.

## Frameworks Introduced
- **Daily VWAP**: VWAP anchored at the start of the trading day (start of the Asian session), ending at the close of the US session.
  - When to use: intraday day trading; author's preferred chart is the 5-minute timeframe (workable from 1-minute to 1-hour).
  - How: plot VWAP fresh each day from the Asian-session open → trade pullback reactions to it while price stays on one side → once the US session closes, stop trading that day's VWAP and switch to the new day's line as the new Asian session begins.
- **Weekly VWAP**: VWAP anchored at the start of the trading week (Asian session open on Monday).
  - When to use: the author's favorite anchor for intraday trading, mainly on the 30-minute timeframe; found to give better signals than Daily VWAP at that timeframe. Kept permanently on his workspace and combined with Volume Profile.
  - How: same pullback logic as Ch2's base strategy, applied to the weekly line — works especially well in trending weekly conditions, where each pullback to Weekly VWAP is a continuation entry in the trend direction.
- **Yearly VWAP**: VWAP anchored at the first trading day of the calendar year, running to year-end.
  - When to use: swing trading and long-term trading, typically on the Daily timeframe (1 candle = 1 day); works on forex, stocks, and other instrument classes.
  - How: identify which side of the Yearly VWAP price has dominated since January 1 → treat pullbacks to it as continuation entries → because it moves slowly, expect infrequent but often high-quality signals, especially in strongly trending years.

## Key Concepts
- **"Broken" VWAP**: a Daily/Weekly/Yearly VWAP that price has crossed through, flipping its role from Support to Resistance (or vice versa) — treated as still tradeable, just from the new side, exactly like the Price Action support-becomes-resistance logic (Ch12).
- **Session boundaries**: Daily VWAP's calculation window is Asian-session-open to US-session-close; it is discarded (not carried overnight) once that window ends.
- **Trend fit**: the author explicitly notes VWAP performs best in trending conditions — a rangebound or choppy calendar period produces frequent role-flips and weaker signals.
- **Signal frequency trade-off**: Yearly VWAP, especially in a steep persistent trend, may only offer a couple of high-quality touches per year — the author's stated reason for trading multiple instruments and strategies rather than relying on any single anchor alone.

## Mental Models
- Use Daily VWAP when you need many intraday opportunities; use Weekly VWAP when you want fewer, higher-quality intraday signals on a slower timeframe; use Yearly VWAP when you're positioning for swing/long-term moves and can tolerate very low trade frequency.
- Think of a VWAP flip (Support→Resistance or Resistance→Support) as a live signal to switch your directional bias immediately, not evidence the tool has "stopped working."

## Anti-patterns
- **Carrying a Daily VWAP into the next session**: the calculation resets each day — dragging yesterday's line into today misrepresents where the current day's average participant transacted.
- **Expecting every touch to react**: the author is explicit that price sometimes overshoots VWAP before reacting, or ignores it entirely with no reaction at all — normal behavior, not a strategy failure.
- **Relying on Yearly VWAP alone for trade frequency**: in a strong, steep trend the line can go untested for very long stretches, producing as few as one or two trades per year on a single instrument.

## Worked Example
Weekly VWAP on a 30-minute EUR/USD chart: buyers initially dominate, so the plan is to buy every pullback to VWAP from above. A major news event then shifts sentiment — price drops sharply through VWAP, flipping the line from Support into Resistance. The long taken just before the flip becomes a losing trade. Rather than fighting the new regime, the correct response is to stop looking for longs and start watching for the price to rally back up and touch the now-Resistance VWAP from below — which happens later in the week, producing a valid short. The author notes a possible short existed near the start of the week too, but flags it as "risky" — better to let the VWAP fully develop for a session or two before trusting an early-week touch.

## Key Takeaways
1. Three calendar anchors, three use cases: Daily → intraday scalping (5-min); Weekly → the author's favorite intraday reference (30-min); Yearly → swing/long-term (Daily chart).
2. A broken/flipped calendar VWAP is still tradeable — just reverse the bias to match the new side.
3. Calendar VWAPs work best in trending conditions; expect weaker, less reliable signals in chop.
4. Trade frequency drops sharply as the anchor period lengthens (Daily > Weekly > Yearly) — diversify across instruments/strategies rather than over-relying on one calendar anchor.
5. Not every touch produces a clean reaction — overshoot and no-reaction are both normal outcomes.

## Connects To
- **Ch2**: applies the base pullback-to-VWAP strategy to three specific calendar anchor points.
- **Ch12**: the "broken VWAP" role-flip is the same underlying mechanic as the Price Action support-becomes-resistance confluence setup.
- **Ch4–Ch9**: the remaining six anchor types (non-calendar) for choosing a VWAP starting point.
