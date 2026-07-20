# Chapter 7: Picking Stocks with the Stock Screener — Step-by-Step

## Core Idea
The screening workflow is the same fixed sequence for every sector — select the sector in the Descriptive tab, apply Market Cap + Dividend Yield, switch to the Fundamental tab and apply the seven ratio filters (adjusted for that sector's normal range), then manually review the resulting company list one by one before saving it to a watchlist/portfolio.

## Frameworks Introduced
- **The screening sequence** (repeated once per chosen sector, 4–5 sectors total):
  1. Descriptive tab: select one Sector; set Market Capitalization (≥$300M, prefer ≥$2B) and Dividend Yield (≥2%).
  2. Fundamental tab: set P/E, P/B, EPS growth (5yr, Positive), ROA, ROE, Debt/Equity, Net Profit Margin (Positive) — using that sector's adjusted ranges from Ch5/Ch6.
  3. Review the resulting stock list. Open each company's profile page and read off: Market Cap, Dividend Yield, P/E, P/B, EPS 5yr, ROA, ROE, Debt/Equity, Net Profit Margin.
  4. If any single ratio looks anomalous (e.g., an unusually low P/E), check the company's recent news/analyst commentary before deciding.
  5. Save the surviving list (e.g., to a FINVIZ portfolio) — this becomes your fundamentally-qualified watchlist, to which Volume Profile timing (Ch9–Ch10) gets applied later.
- **Repeat across sectors, then prune**: after screening all chosen sectors independently, consolidate all qualifying stocks into one master list, then deliberately cut entire sectors you don't want heavy exposure to (even if some of their stocks passed the filter) rather than diluting the portfolio across too many names.

## Key Concepts
- **Company profile page**: FINVIZ's per-stock detail page showing the description, sector/industry/country, price chart, and the full ratio table — this is where you do the manual sanity check after the automated filter narrows the list.
- **Watchlist/portfolio (FINVIZ)**: a saved, registered list of qualifying tickers so you don't need to re-run the screener from scratch each session; clicking a ticker in it jumps straight to that company's chart/details.

## Mental Models
- Treat the screener as a coarse net, and the manual company-profile review as the fine sieve — the filter narrows thousands of stocks to a few dozen; your own read of the numbers (and a news check on outliers) does the final judgment.
- A bad trade *entry* on a fundamentally good stock is far more forgivable than a good entry on a fundamentally bad stock — spend your effort getting the fundamentals right first (this chapter), then timing (Ch9–Ch10) second.

## Anti-patterns
- **Stopping at the automated filter results without opening individual profiles**: the seven ratios narrow the field, but reading the actual numbers per company (and checking outliers against news) is still required.
- **Keeping every sector that produces qualifying stocks**: passing the filter isn't the same as belonging in your final portfolio — actively cut sectors you have structural reservations about (e.g., Financial, Technology) even if individual names there look statistically fine.

## Worked Example
Screening the **Basic Materials** sector (per the author's November 2021 run): Descriptive tab set to Sector = Basic Materials, Market Cap ≥ $2B, Dividend Yield ≥ 2%. Fundamental tab set with that sector's adjusted ranges (P/E < 20, P/B ~2, EPS 5yr positive, ROA/ROE positive and sector-reasonable, Debt/Equity moderate, Net Margin positive). The filter returned 10 qualifying companies. Reviewing two of them individually:

- **AngloGold Ashanti (AU)** — gold mining, South Africa. Market Cap $8.00B | Dividend 2.83% | P/E 8.50 | P/B 2.06 | EPS 5yr +97.20% | ROA 11.70% | ROE 25.30% | Debt/Equity 0.55 | Net Margin 20.20%. Verdict: big company, strong dividend, very good (low) P/E, solid efficiency and manageable debt — passes the manual read as fundamentally sound.
- **BHP Group (BHP)** — diversified mining/petroleum, Australia. Market Cap $149.10B | Dividend 5.45% | P/E 12.82 | P/B 2.82 | EPS 5yr +92.20% | ROA 10.80% | ROE 23.00% | Debt/Equity 0.41 | Net Margin 18.60%. Verdict: a giant with a fantastic dividend, good P/E, and notably low debt for its size.

Both companies cleared the same fixed filter and both hold up under manual review — illustrating that the sequence (filter → open each profile → read the seven numbers → sanity-check outliers) is mechanical and repeatable across every sector, not sector-specific guesswork. (The author notes exact companies returned by the screener will differ over time as prices and fundamentals change — the *method* is what transfers, not any specific ticker.)

A separate example from the walkthrough (NRG-type situation) shows the outlier-check step in practice: a company with a strikingly low P/E (4.01) but otherwise decent numbers (Dividend 3.26%, ROE 99.40%, positive margins) warranted a news check before trusting the number — an abnormally cheap P/E is a flag to investigate, not an automatic buy signal.

## Key Takeaways
1. Run the same 5-step sequence per sector: Descriptive filters → Fundamental filters (sector-adjusted) → manual profile review → outlier news-check → save to watchlist.
2. Screen 4–5 sectors, not just one — consolidate results into a master list afterward.
3. After the automated filter, always open individual company profiles and read the actual numbers before trusting the list.
4. An anomalously good-looking single ratio (e.g., ultra-low P/E) needs a news check, not blind trust.
5. Save qualifying stocks to a persistent watchlist — this becomes the pool that Volume Profile timing (Ch9–Ch10) is later applied to.

## Connects To
- **Ch5, Ch6**: this chapter is the operational application of the sector guide (Ch5) and the seven ratio definitions (Ch6).
- **Ch9, Ch10**: the next step after building this fundamentally-qualified watchlist is finding the right entry price via Price Action + Volume Profile.
- **Ch11**: the same fundamental-filtering framework is reused (in reverse) to decide when a stock's valuation has become too high to keep holding.
