# Chapter 2: Order Flow – Market Participants

## Core Idea
Every print on the Order Flow footprint can come from two fundamentally different kinds of trader — passive (limit-order) or active (market-order) — and the single biggest reason people misread Order Flow is failing to keep this distinction straight.

## Frameworks Introduced
- **Passive vs. Active (Aggressive) Market Participants**: the foundational lens for reading any footprint print.
  - When to use: every time you look at a Bid or Ask number on the footprint — this is prerequisite knowledge for every other framework in the book.
  - How: classify each fill by *how* the order entered, not by *which side of the market it appears on*. Passive = limit order, waits for price to arrive. Active = market order, forces an immediate fill.
- **Bid/Ask Dual Interpretation**: the same footprint side can represent two opposite types of participant depending on order type.
  - When to use: whenever you're tempted to read "BID = Sellers, ASK = Buyers" at face value.
  - How: remember BID shows aggressive Sellers *and* passive Buyers; ASK shows aggressive Buyers *and* passive Sellers. Context (trend, location, size) is what tells you which is more likely dominating.

## Key Concepts
- **Passive market participant**: enters with a limit (pending) order; waits for price to reach their level rather than chasing it.
- **Active (aggressive) market participant**: enters with a market order, willing to accept slippage to get filled immediately.
- **Long via limit order**: appears on the BID (left) side of the footprint.
- **Short via limit order**: appears on the ASK (right) side of the footprint.
- **Long via market order**: appears on the ASK (right) side of the footprint.
- **Short via market order**: appears on the BID (left) side of the footprint.
- **BID (footprint)**: shows the combination of aggressive Sellers and passive Buyers.
- **ASK / Offer (footprint)**: shows the combination of aggressive Buyers and passive Sellers.

## Mental Models
- Use the passive/active split when you catch yourself thinking "green = buyers, red = sellers" — that shorthand is, in the author's words, only a "half-truth." Two-color Volume Profile tools that claim to show pure buyer/seller volume are misrepresenting what Bid/Ask data can actually tell you.
- Think of every footprint cell as a tug-of-war between two possible stories (aggressive vs. passive on each side); the rest of the book's trading and confirmation setups exist to help you infer which story is more likely true in a given context.
- There is no certainty, only reasonable estimation: the author is explicit that you cannot know with 100% confidence whether a given print was passive or active — the goal is a good-enough read, not a perfect one.

## Anti-patterns
- **Treating BID volume as automatically bearish and ASK volume as automatically bullish**: both sides carry two possible interpretations (aggressive vs. passive); skipping this step is, per the author, the main reason traders "struggle to make money" with Order Flow.
- **Trusting Volume Profile or footprint color schemes that label one color "Buyers" and another "Sellers"**: this oversimplifies data that is fundamentally ambiguous without the passive/active lens.

## Key Takeaways
1. Classify every print by order type (passive/limit vs. active/market) before deciding what it means, not by which side of the footprint it lands on.
2. BID = aggressive Sellers + passive Buyers; ASK = aggressive Buyers + passive Sellers — memorize this pairing before moving on.
3. There is no way to know with certainty whether a specific print is passive or active; the rest of the framework is about making the best reasonable estimate from context.
4. Simplistic "green=buy, red=sell" color coding on any indicator should be treated with suspicion.

## Connects To
- **Ch 3**: Basic Chart Description builds the physical footprint/Delta/HVN vocabulary on top of this passive/active lens.
- **Ch 9, Ch 10**: The Confirmation setups (Big Limit Orders = passive; Aggressive Orders/Delta = active) are direct applications of this chapter's distinction.
