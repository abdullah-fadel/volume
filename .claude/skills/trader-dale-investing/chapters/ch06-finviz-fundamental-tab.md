# Chapter 6: FINVIZ Fundamental Tab

## Core Idea
Of ~20 available Fundamental-tab parameters, seven do the real work of separating healthy companies from unhealthy ones — P/E, P/B, EPS growth (past 5 years), ROA, ROE, Debt/Equity, and Net Profit Margin — and every one of them must be read relative to the company's own sector average, never against a single universal number.

## Frameworks Introduced
- **P/E (Price to Earnings)**: `Current Stock Price ÷ EPS`, where `EPS = (Net Income − Dividends) ÷ Shares Outstanding`. Tells you how many years of current earnings it takes to "earn back" the price you paid.
  - When to use: as the default first-pass valuation filter for every stock.
  - How: recommended screener value **P/E < 20** (loosen to 25 for naturally high-P/E sectors). P/E < 5 is a red flag (market doubts the company's future), not a bargain. P/E changes over time as price and earnings both move — wait for price to drop to bring P/E down rather than chasing a stock at a high P/E.
- **P/B (Price to Book)**: `Current Stock Price ÷ Book Value`, where `Book Value = Total Assets − Total Liabilities`. Represents your worst-case-scenario recovery per share if the company liquidated.
  - When to use: to gauge downside protection, especially in asset-heavy sectors.
  - How: recommended **P/B < 3** as a general starting filter; loosen to ~3.5 for naturally high-P/B sectors (Technology, Healthcare); tighten to ~2–2.5 for naturally low-P/B sectors (Energy, Industrials, Utilities). Always compare to the sector average via a P/B reference site, not a universal cutoff.
- **EPS Growth (past 5 years)**: annualized growth of Net Income per share. Recommended filter: **Positive** (>0% over 5 years) — prefer the 5-year figure over "this year" or "next year" projections since it shows an actual track record, not analyst guesses.
- **ROA (Return on Assets)**: `Net Income ÷ Total Assets` — how efficiently a company turns its asset base into profit.
  - How: recommended filter **Positive**, prefer **>5%**, tighten to **>10%** for a narrower search. Only compare ROA within the same sector — asset-light sectors (Technology, Consumer Cyclical) naturally run high ROA; asset-heavy sectors (Energy, Utilities) naturally run low ROA.
- **ROE (Return on Equity)**: `Annual Earnings ÷ Equity`, where `Equity = Assets − Liabilities`. Same efficiency concept as ROA but measured against equity only (excludes the effect of debt financing).
  - How: recommended filter **>10%**, tighten to **15–20%+** for a narrower search. ROE will always read higher than ROA for the same company since the denominator (equity) excludes debt.
- **Debt/Equity**: `Total Debt ÷ Total Equity` — how leveraged the company is.
  - How: recommended **≤60–70%**; treat **>100%** as materially riskier. Also avoid **<10–20%** debt as a potential sign of under-utilized growth potential. Loosen the ceiling substantially for naturally high-debt sectors (Utilities, Energy, Financials, Real Estate/REITs — REIT average is ~350%). **Negative Debt/Equity** (liabilities exceed assets) is a hard avoid — sign of a company in real trouble.
- **Net Profit Margin**: `Net Profit ÷ Total Revenue` — the percentage of every sales dollar the company actually keeps after all expenses.
  - How: recommended filter **Positive** only (>0%) — the author treats this as a low-priority filter (mainly to exclude money-losing companies), not a precision tool, since typical margins vary enormously by sector (naturally high: Financial, Real Estate, Utilities; naturally low: Healthcare/drug distribution, Energy).

## Key Concepts
- **Sector-relative reading**: the single unifying rule across all seven ratios — a "good" P/E, P/B, ROA, ROE, or Debt/Equity number in one sector can be a red flag in another.
- **No debt ≠ good**: debt lets companies scale faster; zero debt can indicate under-investment in growth, not safety.

## Mental Models
- Use P/E as "years to earn your money back," not just an abstract ratio — makes the number intuitive and comparable.
- Treat Book Value/P/B as your personal worst-case Stop Loss for a stock investment — it's what you'd recover, per share, if the company failed.

## Anti-patterns
- **Treating any single ratio as a Holy Grail**: the author repeats this warning for both P/E and P/B specifically — a great-looking single number (e.g., Financial sector's low P/E and P/B) can mask sector-specific risk (leverage) rather than reveal a bargain.
- **Comparing ratios across sectors instead of within them**: e.g., judging a REIT's high Debt/Equity by the same 60–70% ceiling used for a Healthcare company misreads a structurally normal REIT balance sheet as dangerously leveraged.
- **Chasing extremely low P/E as a bargain signal**: P/E below ~5 usually signals the market has already priced in bad news, not an overlooked gem — dig into recent news/analyst commentary before treating it as cheap.

## Key Takeaways
1. Use exactly seven Fundamental-tab filters: P/E, P/B, EPS growth (5yr), ROA, ROE, Debt/Equity, Net Profit Margin.
2. Baseline screener values: P/E < 20, P/B < 3, EPS growth 5yr positive, ROA > 5%, ROE > 10%, Debt/Equity ≤ 60–70%, Net Margin positive.
3. Every one of these baselines must be adjusted up or down against the specific sector's typical range (see Ch5's sector table) — there is no universal cutoff.
4. A stock with a suspiciously perfect-looking single ratio (especially P/E below ~5) deserves a news check before being treated as a bargain.

## Connects To
- **Ch5**: sector-typical ranges for each ratio are cataloged there; this chapter defines the ratios themselves.
- **Ch7**: these seven filters are applied together, sector-by-sector, in the concrete screening walkthrough.
