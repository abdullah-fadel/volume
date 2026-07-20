---
name: trader-dale-vwap
description: "Knowledge base from Trader Dale's VWAP trading book. Use when applying Trader Dale's frameworks for VWAP and Anchored VWAP trading (anchoring to dates, swing points, trend starts, macro news, heavy volume zones, gaps, earnings), the VWAP Rotation and VWAP Trend strategies, confluences with Price Action/Volume Profile, trade entry confirmation, or Take Profit/Stop Loss placement; studying the book; or referencing its concepts."
---

<!-- argument-hint: [topic, framework name, or chapter number] -->

# VWAP Trading
**Author**: Trader Dale (full-time trader since 2008) | **Pages**: ~122 | **Chapters**: 17 | **Generated**: 2026-07-20

## How to Use This Skill

- **Without arguments** — load core frameworks for reference
- **With a topic** — ask about `anchoring`, `vwap rotation`, `stop loss`, or another indexed topic; I find and read the relevant chapter
- **With chapter** — ask for `ch10`; I load that specific chapter
- **Browse** — ask "what chapters do you have?" to see the full index

When you ask about a topic not covered in Core Frameworks below, I will read
the relevant chapter file before answering.

---

## Core Frameworks & Mental Models

**The central thesis**: VWAP works because institutions genuinely use it as an execution benchmark ("fill at VWAP or better"), not because of technical-analysis folklore — this is documented in Congressional testimony from a major hedge fund CEO. VWAP = sum(price × volume) / total volume, so heavy-volume prices pull the line toward them, unlike SMA/EMA.

**Strategy #1 — Reactions to VWAP**: trade pullbacks to the VWAP line itself. Above VWAP = buyers control, trade longs on pullback touches from above; below VWAP = sellers control, trade shorts on pullback touches from below. This is the entry-level signal — the author layers confirmation and confluence on top before real entries.

**Anchoring VWAP** — choose VWAP's start point at a market-significant turning moment instead of only a calendar boundary. Seven anchor types, each with its own reliability profile:
- **Dates** (Daily/Weekly/Yearly): Daily for intraday scalping (5-min), Weekly is the author's favorite intraday reference (30-min), Yearly for swing/long-term (Daily chart). Signal frequency drops sharply as the period lengthens.
- **Swing point**: anchor at a genuinely significant, widely-recognized reversal high/low. Works any timeframe; keep anchor TF and trading TF consistent.
- **Start of trend**: anchor at the large, decisive candle launching a new trend. Strong reactions here come from *two* combined order-flow sources — new trend-joiners entering at "fair price," plus trapped losing traders exiting at the same price (short-covering = buying, long-liquidation = selling).
- **Macro news candle**: anchor only at news confirmed to have *actually* shifted sentiment (started a durable trend), not just spiked and reverted — a red/high-impact tag alone is an insufficient filter.
- **Heavy volume zone**: use Volume Profile to find a rotation where institutions quietly accumulated, then anchor at the candle where that rotation resolves into a trend (not inside the rotation).
- **Gap** (stocks): anchor at the first candle after a big gap.
- **Earnings** (stocks): a specialized gap-anchor case — anchor at the earnings-release candle, prioritizing whichever earnings report produced the largest surprise/gap if several are visible.

**Strategy #2 — Reactions to 1st VWAP deviations**: trade the bands around a date-anchored VWAP instead of the line itself. Check deviation slope first: **horizontal = VWAP Rotation strategy** (Long off lower deviation, Short off upper deviation, TP at the VWAP line; invalidated the moment price closes outside the channel). **Vertical = VWAP Trend strategy** (trade pullbacks to whichever band is trending — upper in an uptrend, lower in a downtrend — with positive RRR and a trailable position). The same chart hands off between the two as regime changes.

**Confluences**: standalone VWAP signals are inconsistent alone. Combine with (a) Price Action's support-becomes-resistance flip (strong reaction(s) at a level → breach → level flips role → trade the retest), (b) the Volume Profile Trend setup (volume cluster within an established trend → trade the pullback in trend direction), or (c) a second, differently-anchored VWAP converging on the same zone. Confluence zones need only general-area overlap, not exact price match.

**Trade entry confirmation** (riskiest → most rigorous): blind first touch (not recommended) → first touch + confluence (OK when 2+ setups already agree) → confirmed reaction (default: wait for one candle to close beyond the level, enter next candle, SL at the Reaction Point) → Order Flow confirmation (author's favorite: Absorption, large Limit order, Cumulative Delta divergence — only meaningful at an already-identified level).

**Take Profit / Stop Loss**: both use the same barrier logic — Price Action flip level, VWAP-family line, or Volume Profile heavy volume zone. TP: exit a few pips *before* the barrier. SL: place *behind* the barrier (combined/overlapping barriers are strongest); migrate it forward as price advances rather than leaving it static. ATR-based sizing (10–20% of average daily ATR, intraday) is the fallback when no structural barrier exists.

**Trailing**: continuously walk SL through the barrier chain as a trend develops. When trailing, prefer a closer/weaker barrier over a farther/stronger one — don't sacrifice too much open profit chasing "the best" barrier.

**Start Simple template** (recommended starting point): confirmed-reaction entry + SL at the Reaction Point + 1:1 RRR Take Profit. Master this one loop before layering in confluence, Order Flow confirmation, or barrier-based TP/SL variety.

**Money management**: Risk per trade = (max tolerable drawdown %) ÷ (backtested worst losing streak × 1.2). Apply that fixed percentage on every trade — never size by confidence (unreliable, and "perfect-looking" trades fail just as often as ordinary ones).

---

## Chapter Index

| # | Title | Key Frameworks |
|---|-------|----------------|
| [ch01](chapters/ch01-introduction-to-vwap.md) | Introduction to VWAP | VWAP formula, why it works (institutional execution), where to get it |
| [ch02](chapters/ch02-strategy1-reactions-to-vwap.md) | Strategy #1: Reactions to VWAP | Base pullback strategy, anchoring overview |
| [ch03](chapters/ch03-anchoring-vwap-to-dates.md) | Anchoring VWAP to Dates | Daily/Weekly/Yearly VWAP |
| [ch04](chapters/ch04-anchoring-vwap-to-swing-points.md) | Anchoring VWAP to Swing Points | Swing-point-anchored VWAP |
| [ch05](chapters/ch05-anchoring-vwap-to-start-of-trend.md) | Anchoring VWAP to Start of the Trend | Trend-start anchor, dual entry/exit pressure |
| [ch06](chapters/ch06-anchoring-vwap-to-macro-news-candle.md) | Anchoring VWAP to Macro News Candle | News-candle anchor, severity filtering |
| [ch07](chapters/ch07-anchoring-vwap-to-heavy-volume-zones.md) | Anchoring VWAP to Heavy Volume Zones | Volume Profile + VWAP anchor |
| [ch08](chapters/ch08-anchoring-vwap-to-gaps.md) | Anchoring VWAP to Gaps | Gap-anchored VWAP (stocks) |
| [ch09](chapters/ch09-anchoring-vwap-to-earnings.md) | Anchoring VWAP to Earnings | Earnings-anchored VWAP (stocks) |
| [ch10](chapters/ch10-strategy2-1st-deviations-and-rotation.md) | Strategy #2 & VWAP Rotation Strategy | 1st deviations, VWAP Rotation strategy |
| [ch11](chapters/ch11-strategy2-vwap-trend-strategy.md) | VWAP Trend Strategy | Trend-band pullback entries, trailing setup |
| [ch12](chapters/ch12-confluences-with-other-strategies.md) | Confluences with Other Strategies | Support-becomes-resistance, Volume Profile Trend setup, combos |
| [ch13](chapters/ch13-trade-entry-confirmation.md) | Trade Entry Confirmation | First touch, confirmed reaction, Order Flow confirmation |
| [ch14](chapters/ch14-take-profit-placement.md) | Take Profit Placement | PA/VWAP/VP/ATR-based TP |
| [ch15](chapters/ch15-stop-loss-placement.md) | Stop Loss Placement | PA/VWAP/VP/combined/ATR-based SL |
| [ch16](chapters/ch16-trailing-your-trade.md) | Trailing Your Trade | SL migration, Start Simple template |
| [ch17](chapters/ch17-money-management.md) | Money Management | Risk-per-trade formula, position sizing, Trade Manager |

## Topic Index

- **Absorption / Order Flow confirmation** → ch13
- **Anchored VWAP (overview)** → ch2
- **ATR-based TP/SL** → ch14, ch15
- **Combined barriers (SL)** → ch15
- **Confluence** → ch12
- **Cumulative Delta divergence** → ch13
- **Daily/Weekly/Yearly VWAP** → ch3
- **Earnings anchor** → ch9
- **Gap anchor** → ch8
- **Heavy volume zone anchor** → ch7
- **Macro news anchor** → ch6
- **Money management / risk per trade** → ch17
- **Order Flow confirmation** → ch13
- **Position sizing** → ch17
- **Price Action support-becomes-resistance** → ch12
- **Reaction Point** → ch13, ch15, ch16
- **Risk-Reward Ratio (RRR)** → ch16, ch17
- **Stop Loss placement** → ch15
- **Start Simple template** → ch16
- **Swing point anchor** → ch4
- **Take Profit placement** → ch14
- **Trade Manager (software)** → ch17
- **Trade entry confirmation** → ch13
- **Trailing** → ch16
- **Trend-start anchor** → ch5
- **VWAP (formula, why it works)** → ch1
- **VWAP deviations (1st deviations)** → ch10, ch11
- **VWAP Rotation strategy** → ch10
- **VWAP Trend strategy** → ch11
- **Volume Profile Trend setup** → ch7, ch12

## Supporting Files

- [glossary.md](glossary.md) — all key terms with definitions
- [patterns.md](patterns.md) — all techniques and trading setups
- [cheatsheet.md](cheatsheet.md) — quick reference tables and decision guides

---

## Scope & Limits

This skill covers the book content only. It assumes basic familiarity with Price Action and
Volume Profile fundamentals (POC, profile shapes, support/resistance flips) as covered in the
sibling `trader-dale-price-action` skill, and Order Flow footprint reading as covered in the
sibling `trader-dale-order-flow` skill — this book references those concepts for VWAP
confluence and confirmation without re-teaching them from scratch, and this skill follows the
same approach. Promotional/upsell content (coupon codes, the "VWAP Pack" course pitch,
testimonials) was excluded as out of scope for a knowledge base. For hands-on chart practice
or live-market application, combine with your own charting/data tools. For topics beyond this
book, check related skills or ask the agent directly.
