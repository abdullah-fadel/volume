# Cheatsheet — Trader Dale Order Flow

Quick-reference decision rules for live trading. Not a replacement for the chapters — this is what to keep beside you while reading a chart.

## Core Reading Rules

| If you see... | It means... | Because |
|---|---|---|
| Volume on BID | Aggressive Sellers **or** passive Buyers | Order type, not side, determines meaning (Ch 2) |
| Volume on ASK | Aggressive Buyers **or** passive Sellers | Same — never assume color = side |
| Bullish footprint + negative Delta | Possible reversal down brewing | Sellers stronger than the up-move suggests (Ch 3) |
| Bearish footprint + positive Delta | Possible reversal up brewing | Buyers stronger than the down-move suggests (Ch 3) |
| Trust Delta divergence more in... | Trending markets | In rotations, institutions blend order types to mask intent (Ch 3) |

## Thresholds & Defaults

| Parameter | Value | Notes |
|---|---|---|
| Imbalance trigger | 300% diagonal dominance | Default; software-adjustable |
| Stacked Imbalance minimum | 3+ imbalances vertically | Default; software-adjustable |
| Trades Filter — EUR Futures (6E) | 25+ lots | Author's baseline setting |
| Trades Filter — ES (S&P 500) | ~300+ lots | Different instrument, different liquidity |
| Target signal frequency (Trades Filter) | ~5–10 signals/day | Tune threshold to hit this, not a fixed lot number |
| Stop Loss sizing | 10–20% of ATR (avg. daily volatility) | Applies to all 3 SL methods |
| "Move away" confirmation before a pullback trade | 1–2 full footprints beyond the zone | Applies to nearly every trading setup |
| Re-trade rule | First touch/test only | Applies to nearly every trading setup |
| Correlation for level transfer | ~100% (EUR, AUD Futures↔Forex) | Transfer visually, 1:1 |
| Correlation for level transfer (inverse) | ~‑100% (CAD, JPY, CHF Futures↔Forex) | Mentally flip the chart; 1 tick ≠ 1 pip |

## Decision Rules

- **When** price reaches a zone from any primary setup, **do** wait for 1 of the 4 confirmations before entering, **because** S/R are zones, not exact prices — confirmation proves it's being defended now.
- **When** a passive confirmation (Limit Order/Absorption) is quickly followed by an active one (Aggressive Orders/Delta), **do** treat this "snowball" as the strongest entry signal, **because** it shows both a big initial player and followers agreeing.
- **When** a Volume-Based TP target is too close for a decent RRR, **do** skip the trade or target the next zone out, **because** a cramped RRR isn't worth the risk.
- **When** trailing and any confirmation fires against you, **do** stop trailing immediately, **because** that's evidence the aggression balance flipped.
- **When** an Unfinished Business marker sits just beyond your SL, **do** move the SL past it or reconsider, **because** price tends to run through to "fix" the marker.
- **When** a marker sits against your entry direction, **do** skip or delay entry, **because** the magnet can pull price through your entry first.
- **When** starting out, **do** trade one instrument (e.g., 6E) until mastered, **because** volume behavior is instrument-specific.
- **When** your Forex broker can't split Bid/Ask, **do** cross-check the correlated Futures contract, **because** Forex feeds typically only give Total Volume.
- **When** an SL method would land outside 10–20% of ATR, **do** fall back to a Fixed SL in range or skip, **because** too tight risks stop-outs, too wide erodes RRR.

## Trade-off Matrix — Stop Loss Methods

| Method | Adapts to Conditions | Simplicity | Best When |
|---|---|---|---|
| Fixed SL | No | High | You want zero per-trade decisions |
| S/R Zone High/Low | Yes | Medium | A clear zone boundary exists |
| Low-Volume-Behind-Zone | Yes | Medium | A heavy-volume zone with a visible low-volume pocket behind it exists |

## Volume Profile Shape → Market Phase

| Shape | Phase | Action Implication |
|---|---|---|
| D | Balance / accumulation | Watch for a breakout direction to emerge |
| P | Uptrend / downtrend ending | Favor Long bias, or watch for reversal up |
| b | Downtrend / uptrend ending | Favor Short bias, or watch for reversal down |
| Thin | Strong trend | Look for small "bump" Volume Clusters as pullback zones |

## Tells & Smells

- **Tell**: "Green = Buyers, Red = Sellers" taken at face value → **Smell**: ignores passive/active order type (Ch 2).
- **Tell**: A Trades Filter signal that never repeats at the same size on a similar instrument → **Smell**: threshold miscalibrated.
- **Tell**: Delta divergence in a clearly sideways market → **Smell**: lower confidence — institutions blend order types in rotations to mask intent.
- **Tell**: A confirmation signal far from any marked S/R zone → **Smell**: not valid — the workflow requires a pre-identified zone.
- **Tell**: Price never testing a distant Unfinished Business marker → **Smell**: normal — never treat it as guaranteed.
- **Tell**: A Rejection Setup where volume distribution is hard to read cleanly → **Smell**: author's own admission — hardest of the three VP setups; proceed cautiously.
- **Tell**: Stopped out right before price reverses in your favor → **Smell**: check if SL sat just short of a heavy-volume zone or Unfinished Business marker (Ch 8, Ch 11).
