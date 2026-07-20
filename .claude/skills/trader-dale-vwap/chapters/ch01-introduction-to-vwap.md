# Chapter 1: Introduction to VWAP

## Core Idea
VWAP (Volume Weighted Average Price) is the average price the market actually paid, weighted by how many shares/contracts traded at each price — unlike SMA/EMA, which only look at time and price, VWAP is the one reference line institutions themselves are quoted against.

## Frameworks Introduced
- **VWAP (Volume Weighted Average Price)**: the average price of an instrument, weighted by traded volume at each price, over a defined period.
  - When to use: as the primary institutional reference line for the whole VWAP framework — everything in this book builds on locating price relative to VWAP.
  - How: sum(price × volume) for every trade in the period, divided by total volume traded in that period. Unlike SMA/EMA, a price level with heavier volume pulls VWAP toward it, so VWAP reflects where most participants actually transacted, not just where price visited.
- **Institutional VWAP execution**: large institutions slice big orders into hundreds of small child orders and execute them algorithmically over a day/week/month, with the explicit goal of filling "at VWAP or better."
  - When to use: as the causal explanation for why VWAP acts as support/resistance (covered in Ch2) — it is not a lagging technical curiosity, it is the actual execution benchmark a large share of institutional flow is measured against.
  - How: no direct action here — this is the "why it works" foundation for every strategy that follows.

## Key Concepts
- **VWAP vs. SMA/EMA**: SMA/EMA are pure time-and-price averages; VWAP adds a volume dimension, so a price with disproportionately heavy volume pulls the average toward it even if it was visited only briefly.
- **Average trader / average market participant**: the hypothetical composite trader VWAP represents — being above VWAP after buying means you paid more than the average buyer that period.
- **Program trades**: institutional algorithmic execution strategies (VWAP being one of the most common) that slice large orders into small pieces executed over time.
- **Anchored VWAP**: VWAP calculated from a chosen starting point other than a fixed calendar boundary (introduced here, detailed starting Ch2).

## Mental Models
- Think of VWAP as "the price the smart money is being graded against" — an institutional trading desk's performance is often judged by whether it filled at or better than VWAP, which makes VWAP a real behavioral magnet, not just a chart curiosity.
- Use the SMA-vs-VWAP divergence as a sanity check: whenever a large volume spike occurs at an atypical price, expect VWAP (not SMA) to reflect the "real" market average.

## Anti-patterns
- **Treating VWAP as "just another moving average"**: ignoring the volume-weighting is the core misunderstanding — a handful of low-volume prints skew an SMA/EMA but barely move VWAP, and vice versa for high-volume prints.
- **Expecting VWAP for free on any platform**: VWAP and Anchored VWAP are not standard indicators on most retail platforms; assuming they're built-in leads to wasted setup time.

## Worked Example
The author contrasts two small tape scenarios to make the weighting concrete. Scenario 1: 1,000 shares trade at $10 and 5,000 shares trade at $20. SMA = ($10+$20)/2 = $15, while VWAP = (($10×1,000)+($20×5,000))/6,000 = $18.33 — VWAP sits much closer to $20 because that's where most of the volume actually transacted. Scenario 2 pushes the point further: only 100 shares trade at $5, and 5,000 shares trade at $20. SMA = ($5+$20)/2 = $12.50, but VWAP = (($5×100)+($20×5,000))/5,100 = $19.70. SMA is badly skewed by the low-volume $5 print; VWAP correctly shows the market was overwhelmingly transacting near $20. The author's conclusion: VWAP reflects the real average of all market participants, which is exactly why institutions use it as an execution benchmark.

## Key Takeaways
1. VWAP = sum(price × volume) / total volume — the volume weighting is the entire point of the indicator.
2. VWAP works because institutions genuinely use it as an execution benchmark ("fill at VWAP or better"), not because of any technical-analysis folklore — this is documented in Congressional testimony from a major hedge fund CEO (Kenneth Griffin, Citadel).
3. Most retail platforms don't ship VWAP or Anchored VWAP by default; budget for either a paid charting tier (e.g., TradingView "Essentials") or a dedicated indicator pack.
4. Everything that follows in this skill — anchoring methods, deviation strategies, confirmations, TP/SL — is built on this single volume-weighted-average concept.

## Connects To
- **Ch2**: explains why price reacting to VWAP is a tradeable pattern, building directly on the institutional-execution rationale here.
- **Ch3–Ch9**: each covers a different way to choose VWAP's starting point (its "anchor"), all using the same underlying VWAP formula introduced here.
