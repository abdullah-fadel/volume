# Chapter 21: Backtesting & Getting Started

## Core Idea
Validating and scaling into a new trading idea should follow a fixed 5-phase progression — rough backtest, thorough backtest, small live trading, half positions, full positions — that trades speed for rigor early (to avoid wasting time on dead ideas) and trades speed for psychological readiness late (to avoid blowing up on a strategy you haven't yet proven you can execute).

## Frameworks Introduced
- **The 5-Phase Method** (author's exact framework for taking an idea from hypothesis to full live trading):
  1. **Rough backtest**: as fast and simple as possible (~1-2 hours) — use RRR=1, ignore macro news, skip confirmations/confluences, strip out anything that would slow the check. Goal: quickly kill bad ideas before investing real time. If promising, proceed; if not, tweak and retry once, or drop it.
  2. **Thorough backtest**: now apply full rules, confluences, and exceptions across more trades and markets/settings. Explicit caveat: even a rigorous backtest never guarantees live profitability (the author reports strategies with 70%+ backtested win rates that failed live) — the point is filtering, not certainty. If it fails, adjust and retry a few times before abandoning (and keep the failed backtests for future ideas); if it looks profitable, proceed.
  3. **Micro trading**: skip demo entirely — trade the strategy on a real account with very small size (author's guideline: 10-20% of normal position size, e.g., 0.1-0.2 lot if normal is 1 lot) so there's enough real stakes to engage psychology without material risk. Stay in this phase long enough to see both winning and losing streaks before judging — don't quit after 5-10 losses or graduate after 10 straight wins.
  4. **Half positions**: once micro trading proves profitable, move to roughly 50% of normal volume. Focus on flawless execution, not strategy changes. Track results comparably to Phase 3. Advance to Phase 5 only when: (a) results over enough trades match Phase 3's profile, (b) execution is flawless (no psychological slip-ups or mistakes), and (c) you've built enough of a buffer to psychologically withstand a losing streak at full size.
  5. **Full positions**: normal size, no longer a "testing" phase. Expect a likely early losing streak ("trial by fire") — push through it rather than abandoning the strategy, since it already passed Phases 1-4. Only revert to Phase 4 (or further back to 2/3) if the strategy proves unprofitable over the long term — and even then, adjust rather than discard outright.
- **Trading journal**: a structured log (minimum fields: date, instrument, level value, profit/loss, notes) kept alongside trade screenshots; complexity is a matter of personal style (simple or highly analytical), but more detail directly improves your ability to backtest, optimize, and debug your strategy later.

## Key Concepts
- **Backtest-to-live gap**: the explicit acknowledgment that no amount of backtesting guarantees live performance — it only screens out clearly bad ideas and estimates a rough edge.
- **"Trial by fire"**: the author's term for the expected early losing streak upon reaching full position size — treated as a normal, necessary test of whether you can execute a validated strategy under real stakes, not as evidence the strategy stopped working.
- **Position-size ramp**: 10-20% (micro) → ~50% (half) → 100% (full) — a three-step scale-in specifically designed to separate "does the strategy work" from "can I execute it under increasing psychological pressure."

## Mental Models
- Treat backtesting speed as a filter, not a final verdict — spend the least time possible killing bad ideas (Phase 1), and reserve deep rigor (Phase 2) only for ideas that already survived the quick filter.
- Treat demo trading as functionally useless for this process — the author skips it entirely in favor of very-small-size live trading, because demo lacks the psychological stakes needed to test execution.
- Judge a phase transition by sample size and consistency, not a lucky streak or unlucky streak in either direction.

## Anti-patterns
- **Doing a slow, thorough backtest first**: wastes time on ideas that a quick rough pass would have already killed.
- **Using a demo account as the "small size" testing phase**: the author explicitly rejects this — real (even tiny) money is required for genuine psychological testing.
- **Abandoning a strategy after a short losing streak in any phase**: losing streaks are statistically expected even from a good strategy; only long-run underperformance across a phase should trigger reverting or discarding.
- **Jumping straight to full position size after a good backtest**: skips the execution-under-pressure testing that Phases 3-4 exist to provide.
- **Quitting during the Phase 5 "trial by fire"**: treating an expected early losing streak at full size as proof the strategy failed, when it already passed rigorous earlier phases.

## Key Takeaways
1. Filter new ideas fast (Phase 1 rough backtest) before investing in deep analysis (Phase 2).
2. Never treat a backtest — however thorough — as proof of future live profitability; it's a screening tool.
3. Skip demo trading; validate execution with very small real-money size instead (Phase 3).
4. Scale position size in three deliberate steps (micro → half → full), gating each transition on consistent results and flawless execution, not a hot or cold streak.
5. Expect and push through an early losing streak at full size ("trial by fire") rather than treating it as failure.
6. Keep a trading journal with at least date, instrument, level, P/L, and notes — plus screenshots — since richer data compounds into better future backtesting and debugging.

## Connects To
- **Ch19 (Money Management)**: the backtest-derived worst-drawdown figure used there for risk-per-trade sizing comes from this chapter's Phase 2 process.
- **Ch20 (Trading Psychology)**: the psychological readiness gates in Phases 3-5 (and the journal/screenshot habit) directly extend that chapter's tools.
