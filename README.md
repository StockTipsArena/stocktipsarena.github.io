# Indian Equity Analyst Recommendations & Horizon Outcome Benchmark (NSE 2025–2026)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/StockTipsArena/india-analyst-accuracy-benchmark/blob/main/notebooks/india_analyst_accuracy_benchmark_2026.ipynb)
[![Live Benchmark Site](https://img.shields.io/badge/Live_Benchmark-stocktipsarena.com-0f766e)](https://stocktipsarena.com)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)

An open, empirical benchmark dataset and methodology companion from **[StockTipsArena](https://stocktipsarena.com)** measuring the real-world outcome accuracy, target-hit rates, stop-loss excursions, and Nifty 50 benchmark-relative returns of **27,954 public Indian stock market recommendations** (**21,736 resolved calls** and **6,218 active calls**) across **1,236 NSE-listed equities** and **303 tracked research analysts and brokerage houses**.

- **Interactive Benchmark & Live Tracker:** [https://stocktipsarena.com](https://stocktipsarena.com)
- **GitHub Pages Benchmark Report:** [https://stocktipsarena.github.io/india-analyst-accuracy-benchmark/](https://stocktipsarena.github.io/india-analyst-accuracy-benchmark/)
- **Product Hunt Hub:** [https://www.producthunt.com/products/stocktipsarena](https://www.producthunt.com/products/stocktipsarena)
- **Google Colab Notebook:** [Run in Google Colab](https://colab.research.google.com/github/StockTipsArena/india-analyst-accuracy-benchmark/blob/main/notebooks/india_analyst_accuracy_benchmark_2026.ipynb)

---

## Key Empirical Findings (November 2026 Release)

1. **Corpus Scale:** **27,954 public NSE calls** audited against official NSE intraday and daily OHLCV candle data (**21,736 resolved**: `8,236 TARGET_HIT`, `6,673 SL_HIT`, `6,827 EXPIRED`).
2. **Overall Target Hit Rate vs. Decided Win Rate:** Across all resolved recommendations, **37.89%** hit their stated target price prior to stop-loss or horizon expiry (`55.24%` decided win rate excluding time-expired calls).
3. **Horizon Stratification Matters:**
   - **Long-Term (`LONG_TERM` BUY, 11,412 calls / 6,270 resolved):** Achieves a **62.63% resolved target-hit rate** (**94.97% decided win rate**) with an average realized return of **+6.76%** against a **+1.71%** horizon-matched Nifty 50 benchmark return (**+5.05% alpha**).
   - **Swing (`SWING` BUY, 8,977 calls / 8,652 resolved):** Achieves a **26.10% resolved target-hit rate** (**34.71% decided win rate**) and **-0.35%** average realized return, illustrating how tight stop-losses (`avg 3.47%`) trigger before medium-range targets (`avg 6.24%`).
   - **Intraday (`INTRADAY` BUY, 4,142 calls / 4,142 resolved):** Achieves a **31.70% resolved target-hit rate** (`46.97%` decided win rate) with **-0.06%** average realized return prior to transaction costs.

---

## Aggregate Outcomes by Horizon & Call Type

| Horizon | Call Type | Total Calls | Resolved Calls | Target Hit | SL Hit | Expired | Target Hit Rate (Resolved) | Decided Win Rate | Avg Realized P&L | Avg Benchmark Return |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| `LONG_TERM` | `BUY` | 11,412 | 6,270 | 3,927 | 208 | 2,135 | **62.63%** | **94.97%** | 6.76% | 1.71% |
| `SWING` | `BUY` | 8,977 | 8,652 | 2,258 | 4,247 | 2,147 | **26.1%** | **34.71%** | -0.35% | -0.13% |
| `SHORT_TERM` | `BUY` | 2,798 | 2,324 | 781 | 1,168 | 375 | **33.61%** | **40.07%** | -0.54% | -0.76% |
| `INTRADAY` | `BUY` | 2,569 | 2,569 | 390 | 623 | 1,556 | **15.18%** | **38.5%** | -0.19% | 0% |
| `LONG_TERM` | `SELL` | 926 | 699 | 585 | 0 | 114 | **83.69%** | **100%** | 5.15% | -1.01% |
| `SWING` | `SELL` | 535 | 512 | 149 | 214 | 149 | **29.1%** | **41.05%** | -0.32% | 0.61% |
| `BTST` | `BUY` | 400 | 398 | 63 | 141 | 194 | **15.83%** | **30.88%** | -0.28% | 0.08% |
| `INTRADAY` | `SELL` | 196 | 196 | 34 | 43 | 119 | **17.35%** | **44.16%** | -0.01% | None% |
| `SHORT_TERM` | `SELL` | 106 | 81 | 48 | 19 | 14 | **59.26%** | **71.64%** | 1.25% | -0.79% |
| `BTST` | `SELL` | 35 | 35 | 1 | 10 | 24 | **2.86%** | **9.09%** | 0.25% | -0.29% |

---

## Live Production Directories on StockTipsArena

- **[A–Z NSE Stock Target Directory (`/stocks`)](https://stocktipsarena.com/stocks)** — Consensus target prices, upside distribution, and historical call resolution for all 1,236 tracked NSE stocks.
- **[SEBI-Verified Analyst Directory (`/analysts`)](https://stocktipsarena.com/analysts)** — Registry-verified Research Analysts (`INH...`), Investment Advisers (`INA...`), and brokerage houses.
- **[Analyst Accuracy Leaderboard (`/leaderboard`)](https://stocktipsarena.com/leaderboard)** — Horizon-faceted accuracy, win-rate, and risk-adjusted return rankings.
- **[Active Analyst Picks (`/picks`)](https://stocktipsarena.com/picks)** — Live open recommendations filtered by horizon (`intraday`, `btst`, `swing`, `short-term`, `long-term`).
- **[Most Recommended NSE Stocks (`/top-stocks`)](https://stocktipsarena.com/top-stocks)** — Multi-analyst consensus stock directory.
- **[Free NSE Stock Screeners (`/screeners`)](https://stocktipsarena.com/screeners)** — Technical, fundamental, and analyst-consensus stock screens.
- **[NSE Sector Consensus Hubs (`/sectors`)](https://stocktipsarena.com/sectors)** — [Chemicals & Petrochemicals](https://stocktipsarena.com/sectors/chemicals-and-petrochemicals) · [Auto Components](https://stocktipsarena.com/sectors/auto-components) · [Pharmaceuticals & Biotechnology](https://stocktipsarena.com/sectors/pharmaceuticals-and-biotechnology) · [Industrial Products](https://stocktipsarena.com/sectors/industrial-products) · [Capital Goods](https://stocktipsarena.com/sectors/capital-goods) · [IT - Software](https://stocktipsarena.com/sectors/it-software) · [Banks](https://stocktipsarena.com/sectors/banks) · [Power](https://stocktipsarena.com/sectors/power) · [Finance](https://stocktipsarena.com/sectors/finance) · [Healthcare Services](https://stocktipsarena.com/sectors/healthcare-services) · [Construction](https://stocktipsarena.com/sectors/construction) · [Consumer Durables](https://stocktipsarena.com/sectors/consumer-durables) · [Defence & Aerospace](https://stocktipsarena.com/sectors/aerospace-and-defense) · [Automobiles](https://stocktipsarena.com/sectors/automobiles) · [Metals & Mining](https://stocktipsarena.com/sectors/ferrous-metals)
- **[High-Activity Mid-Cap & Thematic Stock Pages](https://stocktipsarena.com/stocks)** — [WABAG (VA Tech Wabag Ltd)](https://stocktipsarena.com/stock/WABAG) · [CEMPRO (Cemindia Projects Ltd)](https://stocktipsarena.com/stock/CEMPRO) · [BEL (Bharat Electronics Ltd)](https://stocktipsarena.com/stock/BEL) · [BHEL (Bharat Heavy Electricals Ltd)](https://stocktipsarena.com/stock/BHEL) · [ANANTRAJ (Anant Raj Ltd)](https://stocktipsarena.com/stock/ANANTRAJ) · [NTPCGREEN (NTPC Green Energy Ltd)](https://stocktipsarena.com/stock/NTPCGREEN) · [LGEINDIA (LG Electronics India Ltd)](https://stocktipsarena.com/stock/LGEINDIA) · [CROMPTON (Crompton Greaves Consumer Electricals Ltd)](https://stocktipsarena.com/stock/CROMPTON) · [SSWL (Steel Strips Wheels Ltd)](https://stocktipsarena.com/stock/SSWL) · [RICOAUTO (Rico Auto Industries Ltd)](https://stocktipsarena.com/stock/RICOAUTO) · [GANDHAR (Gandhar Oil Refinery (India) Ltd)](https://stocktipsarena.com/stock/GANDHAR) · [DHOOTTRANS (Dhoot Transmission Pvt Ltd)](https://stocktipsarena.com/stock/DHOOTTRANS)

---

## Top 30 NSE Stocks by Tracked Analyst Call Volume

| NSE Ticker | Company Name | Total Calls | Distinct Analysts | Active Calls | Target Hits | Resolved Hit Rate | Avg Realized P&L |
|---|---|---:|---:|---:|---:|---:|---:|
| [HDFCBANK](https://stocktipsarena.com/stock/HDFCBANK) | HDFC Bank | 221 | 75 | 74 | 27 | 18.37% | -0.48% |
| [ETERNAL](https://stocktipsarena.com/stock/ETERNAL) | Eternal Limited | 216 | 82 | 58 | 70 | 44.3% | 4.34% |
| [HAL](https://stocktipsarena.com/stock/HAL) | Hindustan Aeronautics Ltd. | 188 | 70 | 36 | 35 | 23.03% | 1.05% |
| [COFORGE](https://stocktipsarena.com/stock/COFORGE) | Coforge Limited | 188 | 65 | 29 | 98 | 61.64% | 6.87% |
| [KOTAKBANK](https://stocktipsarena.com/stock/KOTAKBANK) | Kotak Mahindra Bank Ltd. | 175 | 70 | 41 | 49 | 36.57% | 2.84% |
| [SBIN](https://stocktipsarena.com/stock/SBIN) | State Bank of India | 174 | 75 | 42 | 41 | 31.06% | 3.55% |
| [ICICIBANK](https://stocktipsarena.com/stock/ICICIBANK) | ICICI Bank | 172 | 66 | 55 | 38 | 32.48% | 4.26% |
| [BHARTIARTL](https://stocktipsarena.com/stock/BHARTIARTL) | Bharti Airtel | 167 | 63 | 41 | 60 | 47.62% | 3.31% |
| [INDHOTEL](https://stocktipsarena.com/stock/INDHOTEL) | The Indian Hotels Company Limited | 166 | 66 | 49 | 40 | 34.19% | 1.01% |
| [TCS](https://stocktipsarena.com/stock/TCS) | Tata Consultancy Services | 163 | 68 | 30 | 64 | 48.12% | -1.2% |
| [BEL](https://stocktipsarena.com/stock/BEL) | Bharat Electronics | 162 | 73 | 34 | 36 | 28.13% | 1.52% |
| [TVSMOTOR](https://stocktipsarena.com/stock/TVSMOTOR) | TVS Motor Company Ltd. | 160 | 69 | 30 | 65 | 50% | 4.11% |
| [PERSISTENT](https://stocktipsarena.com/stock/PERSISTENT) | Persistent Systems Limited | 160 | 61 | 33 | 55 | 43.31% | 3.24% |
| [HINDALCO](https://stocktipsarena.com/stock/HINDALCO) | Hindalco Industries Ltd. | 156 | 68 | 30 | 54 | 42.86% | 4.21% |
| [TITAN](https://stocktipsarena.com/stock/TITAN) | Titan Company Ltd. | 151 | 60 | 30 | 43 | 35.54% | 3.52% |
| [PAYTM](https://stocktipsarena.com/stock/PAYTM) | One 97 Communications Limited | 151 | 67 | 36 | 64 | 55.65% | 0.59% |
| [FEDERALBNK](https://stocktipsarena.com/stock/FEDERALBNK) | Federal Bank Limited | 146 | 57 | 32 | 58 | 50.88% | 8.17% |
| [BHEL](https://stocktipsarena.com/stock/BHEL) | Bharat Heavy Electricals Ltd | 137 | 66 | 21 | 37 | 31.9% | 1.56% |
| [HEROMOTOCO](https://stocktipsarena.com/stock/HEROMOTOCO) | Hero MotoCorp | 134 | 63 | 26 | 49 | 45.37% | 3.93% |
| [LAURUSLABS](https://stocktipsarena.com/stock/LAURUSLABS) | Laurus Labs Ltd | 132 | 49 | 11 | 61 | 50.41% | -0.11% |
| [AXISBANK](https://stocktipsarena.com/stock/AXISBANK) | Axis Bank Limited | 131 | 57 | 42 | 23 | 25.84% | 3.19% |
| [ASHOKLEY](https://stocktipsarena.com/stock/ASHOKLEY) | Ashok Leyland | 131 | 61 | 22 | 40 | 36.7% | 2.86% |
| [SHRIRAMFIN](https://stocktipsarena.com/stock/SHRIRAMFIN) | Shriram Finance Limited | 131 | 54 | 39 | 41 | 44.57% | 6.11% |
| [DLF](https://stocktipsarena.com/stock/DLF) | DLF Limited | 130 | 51 | 26 | 27 | 25.96% | -1.24% |
| [INFY](https://stocktipsarena.com/stock/INFY) | Infosys | 130 | 53 | 34 | 37 | 38.54% | 0.8% |
| [HCLTECH](https://stocktipsarena.com/stock/HCLTECH) | HCL Technologies | 130 | 61 | 23 | 54 | 50.47% | 2.55% |
| [MARUTI](https://stocktipsarena.com/stock/MARUTI) | Maruti Suzuki India Limited | 127 | 62 | 51 | 29 | 38.16% | 1.67% |
| [BAJFINANCE](https://stocktipsarena.com/stock/BAJFINANCE) | Bajaj Finance Ltd. | 124 | 59 | 30 | 50 | 53.19% | 8.57% |
| [DRREDDY](https://stocktipsarena.com/stock/DRREDDY) | Dr. Reddy's Laboratories Limited | 124 | 59 | 32 | 38 | 41.3% | 1.79% |
| [BAJAJ-AUTO](https://stocktipsarena.com/stock/BAJAJ-AUTO) | Bajaj Auto | 123 | 62 | 23 | 50 | 50% | 5.02% |

---

## Repository Contents

- `data/horizon_outcomes_2026.csv` — Horizon-stratified outcome metrics (`LONG_TERM`, `SWING`, `INTRADAY`, `SHORT_TERM`, `BTST`, `POSITIONAL`).
- `data/sector_outcomes_2026.csv` — Sector-level call volume, target-hit rates, and realized returns.
- `data/stock_consensus_top60_2026.csv` — Top 60 NSE equities by multi-analyst coverage and outcome resolution.
- `data/benchmark_summary_2026.json` — Full machine-readable JSON benchmark snapshot.
- `notebooks/india_analyst_accuracy_benchmark_2026.ipynb` — Reproducible Python/Colab analysis notebook.
- `datapackage.json` & `CITATION.cff` — Frictionless Data and academic citation metadata.
