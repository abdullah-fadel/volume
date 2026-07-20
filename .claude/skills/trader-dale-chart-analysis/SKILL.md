---
name: trader-dale-chart-analysis
description: "Reads a trading chart screenshot (any instrument, any timeframe) and produces a structured technical analysis by applying Trader Dale's Price Action, Volume Profile, and Order Flow frameworks together. Use when the user gives a pair/instrument name and timeframe with a chart image and asks for analysis, trade setup identification, or a decision walkthrough. Depends on the trader-dale-price-action and trader-dale-order-flow skills being installed as sibling skills."
---

<!-- argument-hint: <instrument> <timeframe> + attach one or more chart screenshots -->

# Trader Dale Chart Analysis

Applies the frameworks already extracted into the `trader-dale-price-action` and
`trader-dale-order-flow` skills to an actual chart the user shows you — turning
"here's a screenshot" into a structured read using the author's own decision rules,
not generic TA.

This skill is an orchestrator, not a third knowledge base: it does not duplicate
content. It tells you which files to pull from the two sibling skills, in what
order, and how to assemble the result.

## Required inputs

Before analyzing, make sure you have:
1. **Instrument** — e.g. EURUSD, XAUUSD, ES futures, BTCUSD.
2. **Timeframe** — e.g. M5, M15, H1, D1.
3. **At least one chart screenshot**, attached as an image.

If any of these is missing, ask for it — do not guess an instrument, timeframe,
or price level that wasn't given to you.

## Step 1 — Classify the chart

Look at the image(s) directly. Determine which of these it is:
- **Plain candlestick / price chart** → Price Action + Volume Profile frameworks apply.
- **Volume Profile chart** (horizontal histogram on the price axis, POC/Value Area visible) → Volume Profile frameworks apply.
- **Footprint / order-flow chart** (per-candle bid×ask ladder, delta, imbalances visible) → Order Flow frameworks also apply.

Note what's *not* visible too (e.g. no footprint data, no higher-timeframe context) —
this determines what you can and cannot assess later.

## Step 2 — Pull the relevant decision rules

Locate the sibling skills relative to this skill's own directory (same
`SKILLS_HOME`, i.e. `../trader-dale-price-action/` and `../trader-dale-order-flow/`).

Always read first:
- `../trader-dale-price-action/cheatsheet.md` — decision rules, thresholds, tells & smells
- `../trader-dale-price-action/SKILL.md` — core frameworks + topic index (only if you need to locate a specific chapter)

Read on demand, only for what the chart actually shows:
- `../trader-dale-order-flow/cheatsheet.md` — only if a footprint/DOM chart was provided
- Specific chapter files under either skill's `chapters/` folder when you recognize a
  specific pattern and need the full detail (e.g. `../trader-dale-price-action/chapters/ch11-failed-auction.md`,
  `../trader-dale-order-flow/chapters/ch09-confirmations-big-limit-orders-absorption.md`)

Don't load chapters you don't need — that defeats the point of the on-demand design.

## Step 3 — Check systematically

Walk through, using only what's visible in the image:

- **Volume Profile shape** (if a profile is visible): D / P / b / thin-shaped, POC location, Value Area high/low, any high-volume or low-volume nodes.
- **Price Action institutional-activity tells**: sideways compression area, aggressive initiation move, strong rejection of higher/lower prices.
- **Named strategy match**: does the setup resemble support/resistance flip, open-drive, AB=CD, session open, daily open, daily/weekly high-low, or a failed auction? Check strong vs. weak highs/lows too.
- **Order Flow confirmations** (only if a footprint/DOM chart was given): passive vs. active participants, stacked imbalances, absorption at a level, cumulative delta divergence, unfinished business (poor high/poor low).

## Step 4 — Report

Use this template:

```markdown
# Technical Read — <INSTRUMENT> (<TIMEFRAME>)

## What's on the chart
<objective description of what is actually visible — chart type, visible price levels, visible session/date if shown>

## Volume Profile read
<POC, Value Area, shape, HVN/LVN — or "No Volume Profile visible in this screenshot.">

## Price Action signals
<institutional-activity tells and structure observed>

## Order Flow confirmations
<passive/active reads, imbalances, absorption, delta — or:
"Not assessed — no footprint/order-flow chart was supplied. Real-time delta and
order-book absorption can't be read from a static price chart.">

## Matching setup(s)
- **<Strategy name>** (see `trader-dale-price-action` ch<N>) — <why it matches, the book's entry criteria>

## Suggested levels (per the book's rules — not a guarantee)
- Entry zone: <...>
- Stop loss: <... per the relevant cheatsheet rule>
- Take profit: <... per the relevant cheatsheet rule>

## Confidence & limitations
<what can't be verified from a static screenshot — no live delta, no real-time order
book, no macro/news context, no higher-timeframe confirmation unless a second image
was given>

---
⚠️ Educational analysis only, based on Trader Dale's published frameworks applied to
what's visible in the screenshot you provided. Not financial advice, not a trade
recommendation, and not a substitute for your own risk management and due diligence.
Trading involves substantial risk of loss.
```

## Rules

1. **Never invent** price levels, volume numbers, or a profile shape that isn't
   visible or reasonably inferable from the image. Say "not clear from this
   screenshot" rather than guessing.
2. **Never skip the disclaimer** — it's part of the output, every time.
3. If the user asks for a running/live analysis across many charts in one session,
   re-run Steps 1–4 fresh for each new image; don't assume the setup carried over.
4. If the chart is unreadable (too small, cropped, wrong asset entirely), say so and
   ask for a clearer screenshot instead of forcing an analysis.
