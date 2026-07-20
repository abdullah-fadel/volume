---
name: trader-dale-order-flow
description: "Knowledge base from \"Order Flow\" by Trader Dale. Use when applying Trader Dale's frameworks for footprint chart reading, Volume Profile, market participants (passive vs. active), trading setups, confirmation setups, or take profit/stop loss placement, studying the book, or referencing its concepts."
---

<!-- argument-hint: [topic, framework name, or chapter number] -->

# Order Flow
**Author**: Trader Dale (Dale — full-time trader since 2008, certified portfolio/investment manager) | **Pages**: ~161 | **Chapters**: 13 | **Generated**: 2026-07-20

## How to Use This Skill

- **Without arguments** — load core frameworks for reference
- **With a topic** — ask about `imbalances`, `volume profile`, `take profit`, or another indexed topic; I find and read the relevant chapter
- **With chapter** — ask for `ch06`; I load that specific chapter
- **Browse** — ask "what chapters do you have?" to see the full index

When you ask about a topic not covered in Core Frameworks below, I will read
the relevant chapter file before answering.

---

## Core Frameworks & Mental Models

**Passive vs. Active (Aggressive) Market Participants** — the foundational lens for every other framework here. Passive participants use limit orders and wait for price; active participants use market orders and force an immediate fill. BID shows aggressive Sellers *and* passive Buyers; ASK shows aggressive Buyers *and* passive Sellers. Never read "green=Buyers, red=Sellers" at face value — classify by order type, not by side.

**Futures-first analysis, Forex-optional execution** — analyze on a centralized Futures contract (true Bid/Ask data) even if you execute in Forex. Use correlated pairs (6E↔EUR/USD) for near-1:1 level transfer; for inversely-correlated pairs (CAD, JPY, CHF) mentally flip the chart before transferring a level.

**One-Instrument Mastery Rule** — start and stay with a single instrument (author uses 6E) until volume behavior, active hours, and reaction style are mastered before adding a second.

**Delta / Cumulative Delta** — Delta = Ask − Bid for one footprint; Cumulative Delta is the running daily sum. Watch for divergence: price and Delta (or Cumulative Delta) disagreeing in direction, especially near a Support/Resistance zone, is a reversal warning. Trust this far more in trending than rotational conditions.

**Volume Cluster / Multiple Node / Imbalance / Stacked Imbalance** — four different "detectors" for the same underlying question: where did institutions commit heavy volume? Volume Clusters and Multiple Nodes use shading/stacked HVNs (Volume-only, works on Forex); Imbalances (300%+ diagonal dominance) and Stacked Imbalances (3+ in a row) use order aggression (needs Bid x Ask). All feed into the shared **pullback-into-a-defended-zone** trading template: confirm price left the zone by 1–2 footprints → wait for the first pullback only → enter on defense, direction set by context.

**Unfinished Business** — an improperly formed high/low (opposite side never hit 0 contracts) behaves like a magnet, pulling price back to "fix" it. Use only as a decision aid — never a standalone entry: (1) stretch a Take Profit if a marker sits just ahead, (2) avoid placing a Stop Loss just short of one, (3) treat a pullback against you as likely temporary if a marker sits beyond it in your favor, (4) avoid entries with a marker against your direction.

**The Confirmation Workflow** — mark S/R zones first with a primary method (a trading setup or Volume Profile), then wait for price to arrive and look for one of 4 confirmations before entering: **Big Limit Orders** (large passive fill at the zone), **Absorption** (heavy Bid+Ask volume with no price break), **Aggressive Orders/Delta** (active participants piling in), **Cumulative Delta Divergence** (1-min price vs. Cum. Delta disagreeing). The strongest pattern is a "snowball": a passive confirmation (#1 or #2) followed shortly by an active one (#3).

**Volume Profile** — shows Volume *at Price* (not volume over time), calculated from Price+Time+Volume, revealing where institutions actually committed capital. Four recurring shapes: **D** (balance/accumulation), **P** (uptrend or downtrend-ending rotation), **b** (downtrend or uptrend-ending rotation), **Thin** (strong trend, small "bump" clusters). Three trading setups locate zones from three market contexts: **Volume Accumulation** (pre-trend rotation — author's favorite), **Trend Setup** (mid-trend pause), **Rejection Setup** (single aggressive reversal — hardest of the three).

**Take Profit & Stop Loss** — default TP: bank profit slightly *before* the next heavy-volume zone (30-min footprint). Trail only while Imbalances favor your side; stop trailing the instant a confirmation signal fires against you. Three SL methods (Fixed, S/R zone high/low, low-volume-behind-heavy-zone), all sized to roughly 10–20% of ATR-measured average daily volatility.

---

## Chapter Index

| # | Title | Key Frameworks |
|---|-------|----------------|
| [ch01](chapters/ch01-setting-up-order-flow.md) | Setting Up Order Flow | Futures-first analysis, One-Instrument Mastery, level transfer |
| [ch02](chapters/ch02-market-participants.md) | Order Flow – Market Participants | Passive vs. Active participants |
| [ch03](chapters/ch03-basic-chart-description.md) | Order Flow – Basic Chart Description | Footprints, Delta, HVN, Delta Divergence |
| [ch04](chapters/ch04-special-features.md) | Order Flow – Special Features | Volume Clusters, Imbalances, Unfinished Business, Trades Filter, Cumulative Delta |
| [ch05](chapters/ch05-trading-workspace.md) | Order Flow – Trading Workspace | Four-Chart Linked Workspace |
| [ch06](chapters/ch06-setup-volume-clusters-multiple-nodes.md) | Trading Setups — Volume Clusters & Multiple Nodes | Setup #1, Setup #2, two-factor push |
| [ch07](chapters/ch07-setup-trades-filter-stacked-imbalances.md) | Trading Setups — Trades Filter & Stacked Imbalances | Setup #3, Setup #4 |
| [ch08](chapters/ch08-setup-unfinished-business.md) | Trading Setup — Unfinished Business | Unfinished Business as decision aid |
| [ch09](chapters/ch09-confirmations-limit-orders-absorption.md) | Confirmations — Big Limit Orders & Absorption | Confirmation #1, Confirmation #2 |
| [ch10](chapters/ch10-confirmations-aggressive-orders-cumulative-delta.md) | Confirmations — Aggressive Orders/Delta & Cumulative Delta Divergence | Confirmation #3, Confirmation #4, snowball effect |
| [ch11](chapters/ch11-take-profit-stop-loss.md) | Take Profit & Stop Loss with Order Flow | Volume-Based TP, Trailing TP, 3 SL methods |
| [ch12](chapters/ch12-volume-profile-basics.md) | Finding Support & Resistance with Volume Profile | Volume Profile shapes (D/P/b/Thin) |
| [ch13](chapters/ch13-volume-profile-trading-setups.md) | Volume Profile – Trading Setups | Volume Accumulation, Trend, Rejection setups |

## Topic Index

- **Absorption** → ch04, ch09
- **Active/Passive participants** → ch02, ch10
- **ATR / Stop Loss sizing** → ch11
- **Cumulative Delta** → ch03, ch04, ch10
- **Delta / Delta Divergence** → ch03, ch04
- **Data feed / Level 1 vs Level 2** → ch01
- **Footprints** → ch03
- **Forex vs. Futures** → ch01, ch04
- **High Volume Node (HVN)** → ch03, ch04, ch06
- **Iceberg Order** → ch04, ch07
- **Imbalance / Stacked Imbalance** → ch04, ch07
- **Instrument selection (6E, ES)** → ch01, ch07
- **Multiple Node** → ch03, ch04, ch06
- **Risk/Reward Ratio (RRR)** → ch11
- **Stop Loss (3 methods)** → ch11
- **Support/Resistance (zones)** → ch04, ch09, ch12
- **Take Profit (volume-based & trailing)** → ch11
- **Trades Filter** → ch04, ch07
- **Trading Workspace setup** → ch05
- **Unfinished Business** → ch04, ch08, ch11
- **Volume Accumulation Setup** → ch13
- **Volume Cluster** → ch04, ch06, ch12, ch13
- **Volume Profile (definition & shapes)** → ch12
- **Volume Profile trading setups** → ch13

## Supporting Files

- [glossary.md](glossary.md) — all key terms with definitions
- [patterns.md](patterns.md) — all techniques and trading setups
- [cheatsheet.md](cheatsheet.md) — quick reference tables and decision guides

---

## Scope & Limits

This skill covers the book content only — the author repeatedly stresses that Order Flow reading is a hands-on skill that "cannot be learned from a book" alone; use this skill to apply the frameworks while reviewing real charts, not as a substitute for screen time. For hands-on implementation in your own trading platform/software, combine with your platform's documentation. For topics beyond this book (e.g., broader technical analysis, risk/position sizing theory, other markets), check related skills or ask the agent directly.
