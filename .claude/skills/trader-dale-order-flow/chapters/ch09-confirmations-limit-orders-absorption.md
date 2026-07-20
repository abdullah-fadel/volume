# Chapter 9: Order Flow Confirmations — Big Limit Orders & Absorption

## Core Idea
Confirmation setups aren't independent strategies — they're the final "is this zone actually reacting right now" check applied at a Support/Resistance zone already identified by a primary setup (trading setups, Ch 6–8, or Volume Profile, Ch 12–13), and Big Limit Orders and Absorption are the first two of the author's four confirmations.

## Frameworks Introduced
- **The Confirmation Workflow (applies to all four confirmation setups)**: mark S/R zones first with a primary method, then wait for price to arrive and look for one of the four confirmations before entering.
  - When to use: whenever a level is unclear, price is moving fast/aggressively into it, or the level itself feels weaker than usual and you want extra conviction before risking a trade.
  - How: identify the S/R zone with Volume Profile, an Order Flow trading setup, or Price Action; when price reaches the zone (remember: S/R are *zones*, not exact price points), switch to Order Flow and watch for a confirmation appearing anywhere inside that zone.
- **Confirmation Setup #1: Big Limit Orders**: a large passive order appearing right at the S/R zone.
  - When to use: as the first, most direct sign that "the big guys" are willing to defend a level.
  - How: at the S/R zone, watch for an unusually large Limit order to print — a Limit Sell (large print on the Ask) confirms Resistance / a Short; a Limit Buy (large print on the Bid) confirms Support / a Long. Preferred view: 5-minute Bid x Ask. Enter as soon as the large order is visible; it may build over several minutes rather than appear all at once, and "unusually large" varies by instrument/session.
- **Confirmation Setup #2: Absorption**: heavy volume appears simultaneously on both Bid and Ask at the zone, without price breaking through.
  - When to use: a slightly simpler alternative read to Big Limit Orders — look for whoever is defending the zone soaking up all of the opposing side's aggression.
  - How: at the S/R zone, watch for unusually large volume on *both* Bid and Ask at once while price fails to move further — this signals one side is absorbing the other's momentum. To judge "unusually large," compare against the recent average cell volume on that instrument. Preferred views: 5-minute or 30-minute chart. Enter once absorption is confirmed; like Big Limit Orders, it can take a few minutes to build.

## Key Concepts
- **Support/Resistance as a zone, not a price**: confirmations should be looked for anywhere inside the marked zone, not at one exact tick.
- **Big Limit Order**: an unusually large single passive (limit) fill appearing right at an S/R zone.
- **Absorption**: simultaneous heavy Bid *and* Ask volume at a zone, indicating one side is soaking up the other's aggressive pressure without letting price break through.
- **Average cell volume**: the recent baseline volume-per-cell for an instrument, used as the yardstick for judging what counts as "unusually large" in both confirmations.

## Mental Models
- Think of Big Limit Orders as "the first domino" — a big passive trader steps in at the zone. Absorption is the "tug of war becomes a stalemate" picture — aggression from one side gets fully soaked up by the other without price moving.
- **Why it works (Limit Orders)**: passive traders use limit orders specifically because they want a *particular* price — so a big limit fill exactly at your S/R zone is direct evidence someone important agrees the level matters.
- **Why it works (Absorption)**: if aggressive Sell orders are hitting the market and price simply isn't dropping, someone with size is buying everything being sold — that's only rational if they believe the level should hold.
- **Failure mode**: judging "unusually large" from a single glance rather than the local average — both confirmations are instrument- and session-relative, so a fixed mental threshold carried over from a different instrument will misfire.

## Anti-patterns
- **Treating a Big Limit Order or Absorption signal seen away from a marked S/R zone as meaningful**: both confirmations only carry weight when they occur inside a zone already identified by a primary method — elsewhere they're just noise.
- **Entering the instant the first large print appears**: both setups note the full order/absorption picture can take a few minutes to fully form; jumping in on a partial read risks a false signal.

## Worked Example
**Big Limit Order confirmation logic (EUR Futures, 5-minute chart):** Price approaches a zone previously marked as Resistance via Volume Profile. The trader watches the 5-minute Bid x Ask chart and sees an unusually large print appear on the Ask — a Limit Sell far bigger than the surrounding cells. Because this occurs precisely inside the marked Resistance zone (not randomly elsewhere on the chart), it confirms institutional Sellers are defending the level, and the trader treats this as the green light to enter Short immediately.

## Key Takeaways
1. All four confirmation setups (this chapter and Ch 10) require a pre-identified S/R zone — they confirm reactions, they don't locate levels themselves.
2. Big Limit Orders confirm via passive size: Limit Sell on Ask → Resistance/Short; Limit Buy on Bid → Support/Long.
3. Absorption confirms via simultaneous heavy Bid+Ask volume without a price break — evidence one side is soaking up the other's pressure.
4. "Unusually large" is relative to the instrument's recent average cell volume, not an absolute number — and may take a few minutes to fully form.
5. Use confirmations especially when uncertain: fast/aggressive approaches to a level, unclear zone boundaries, or a level you already suspect is weaker than usual.

## Connects To
- **Ch 2**: Passive vs. Active framework underlies why Big Limit Orders (passive) and Absorption (mixed) read differently.
- **Ch 6, Ch 7, Ch 8**: The primary trading setups that supply the S/R zones these confirmations are applied to.
- **Ch 10**: Confirmation Setups #3 and #4 continue the same workflow with active-order and Cumulative-Delta-based confirmations, and can combine with #1/#2 for the strongest read.
