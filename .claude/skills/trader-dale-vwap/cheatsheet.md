# Cheatsheet — Trader Dale's VWAP Decision Rules

## Core Filter
Every VWAP touch is a *candidate*, not a trigger. Before entering: (1) confirm which side of VWAP/deviation controls price, (2) get one of the four entry confirmations (Ch13), (3) prefer levels backed by confluence (Ch12) over standalone VWAP touches. Never blind-enter on first touch unless confluence is already present.

## Which VWAP Anchor to Use
| Situation | Anchor | Timeframe |
|---|---|---|
| General intraday scalping | Daily VWAP | 5-min |
| Author's favorite intraday reference | Weekly VWAP | 30-min |
| Swing / long-term positioning | Yearly VWAP | Daily |
| A clear reversal point exists | Swing point | Match your trading TF |
| A decisive trend-launch candle exists | Start of trend | Match your trading TF |
| Confirmed game-changing news just hit | Macro news candle | 5–30 min |
| Volume Profile shows accumulation → breakout | Heavy volume zone | Any |
| Stock just gapped meaningfully | Gap (1st candle after) | Stocks; 5–30 min or Daily |
| Stock just reported earnings | Earnings candle | Stocks; Daily preferred |

## Regime Read (1st Deviations)
| Deviation slope | Regime | Strategy |
|---|---|---|
| Horizontal | Rotation | VWAP Rotation strategy — fade the bands, TP at VWAP |
| Vertical (at least one) | Trend | VWAP Trend strategy — ride the trending band, trail |
| Price closes outside the channel | Regime just changed | Switch Rotation → Trend (or vice versa) |

## Entry Confirmation Ladder (riskiest → most rigorous)
1. Blind first touch — **not recommended standalone**.
2. First touch + confluence — OK **only** when 2+ independent setups already agree on the zone.
3. Confirmed reaction (default) — wait for one candle to close beyond the level, enter next candle open, SL at the Reaction Point.
4. Order Flow confirmation (author's favorite, most advanced) — Absorption / large Limit order / Cumulative Delta divergence, **only meaningful at an already-identified level**.

## Take Profit Decision Rule
"Always exit a few pips *before* a barrier, never wait for it to be tested." Barrier sources, in no fixed priority — use whichever is nearest/strongest: Price Action flip level, opposing VWAP-family line, Volume Profile heavy zone. No barrier nearby → ATR-based TP = 10–20% of average daily ATR (intraday).
**Don't** overplot every possible VWAP anchor — restrict to the strongest levels or you'll see a "barrier" every few pips and exit too early.

## Stop Loss Decision Rule
SL always goes *behind* a barrier. Priority: combined barrier (2+ types overlapping) > single barrier (Price Action / VWAP / Volume Profile) > ATR-based (10–20% of average daily ATR, only when no structural barrier exists).
**Migrate forward** as price advances through a developing trend — don't leave SL at an increasingly distant original level.
**When trailing**: prefer a closer, weaker barrier over a farther, stronger one — protect accumulated profit over chasing "the best" barrier.

## Start Simple Template (recommended default)
Entry: confirmed-reaction candle close. SL: the Reaction Point that entry creates. TP: mirror SL distance for a 1:1 RRR. Master this one loop before adding confluence, Order Flow confirmation, or barrier-based TP/SL variety.

## Confluence Checklist
A level is stronger when 2+ of these independently agree on the same general zone:
- [ ] VWAP (any anchor type, or a deviation)
- [ ] A second, differently-anchored VWAP
- [ ] Price Action support-becomes-resistance flip
- [ ] Volume Profile Trend setup (volume cluster within a trend)

## Money Management
Risk per trade = (max tolerable drawdown %) ÷ (backtested worst losing streak × 1.2). Example: 6-loss worst streak → ×1.2 = 7.2 ≈ 7; 25% max drawdown tolerance → 25% ÷ 7 = **3.6%** risk per trade. Apply that percentage identically to every trade — never size up on "confident" trades or down on "unsure" ones (confidence isn't measurable, and "perfect-looking" trades fail just as often).

## Macro News Filter (for anchoring or avoiding trades around)
Red/high-impact tag alone is insufficient — filter further by actual reaction. Priority events worth anchoring to: Rate Decision, FOMC/Monetary Policy Statement, CPI, GDP, NFP, Unemployment Rate, major-economy leader speeches. A "strong" tagged event that fully reverts (no lasting sentiment shift) is **not** a valid anchor.

## Red Flags / Tells
- Deviations still tight/undeveloped right after a new anchor period starts → wait, don't force a Trend-strategy entry yet.
- A VWAP-family line crossed and flipped role → re-orient bias immediately to the new side, don't fight it.
- An Order Flow signal (Absorption, Limit order, Delta divergence) appearing away from any real level → low value, ignore it.
- Confirming candle is unusually large → expect to miss part of the move; that's the accepted trade-off of waiting for confirmation, not a reason to chase.
- Chart cluttered with many plotted VWAP anchors → simplify; too many "barriers" causes premature TP/SL exits.
