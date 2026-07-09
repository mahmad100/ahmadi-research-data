# Palantir Is Down: What I Learned From a First Mini Research

Reproducible code for the Ahmadi Research blog post
**[Palantir Is Down: What I Learned From a First Mini Research](https://ahmadiresearch.com/blog/palantir-scorecard/)**.

The post revisits a September 2025 short call on Palantir (PLTR) priced at $171.43. This notebook
regenerates every chart in the post from publicly available sources, with the data inline and the
full numbered source list at the bottom of the notebook.

---

## What's in here

```
Palantir_Scorecard_Charts.ipynb   The notebook: three charts, data inline.
README.md                         This file.
requirements.txt                  Python dependencies. Standard scientific Python.
```

## Quickstart

```bash
# 1. Clone or download this folder
# 2. Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the notebook
jupyter notebook Palantir_Scorecard_Charts.ipynb
```

Run the cells top to bottom.

## Charts reproduced

| # | Chart                                                    | Source(s)                                   |
|---|----------------------------------------------------------|---------------------------------------------|
| 1 | Price since the call, with the $171.43 short-call line    | Nasdaq; Macrotrends [2]                      |
| 2 | The growth the bear case missed (20% premise vs. 85%)    | Beyond the Buzz [1]; Palantir Q1 2026 [4]   |
| 3 | Price-to-sales: call vs. today vs. peer median           | Beyond the Buzz [1]; filings [4]; stockanalysis.com [5] |
| 4 | Revenue concentration: government vs. commercial, US vs. international | Palantir Q1 2026 Business Update [11]         |
| 5 | Dilution: diluted weighted-average share count           | Palantir SEC filings [12]                    |
| 6 | The shareholder vote: outside support vs. dual-class control | Financial Times [18]                       |

## Things worth changing

Two data choices are open to substitution:
- The price series is approximate month-end closes. Substitute the daily series if you want
  intra-month precision around the November 2025 peak and the June 2026 low.
- The peer median price-to-sales uses a seven-name enterprise-software set (Salesforce,
  ServiceNow, Oracle, SAP, Snowflake, Datadog, CrowdStrike). Swap the peer group or use forward
  multiples to test how sensitive the comparison is.

## Sources

The full numbered reference list is in the final cell of the notebook. Key sources:

- The original deck: [Beyond the Buzz: Why Palantir's Valuation May Not Add Up](https://ahmadiresearch.com/papers/palantir-valuation.pdf) (Ahmadi Research, September 2025)
- Price history: [Macrotrends](https://www.macrotrends.net/stocks/charts/PLTR/palantir-technologies/stock-price-history)
- Q1 2026 results: [Palantir 8-K, Exhibit 99.1](https://www.sec.gov/Archives/edgar/data/1321655/000132165526000026/a2026q1ex991pressrelease.htm)
- Valuation statistics and peers: [stockanalysis.com](https://stockanalysis.com/stocks/pltr/statistics/)
- Analyst consensus: [TipRanks](https://www.tipranks.com/stocks/pltr/forecast)
- The 2026 software de-rating: [CNBC](https://www.cnbc.com/2026/02/04/software-stocks-plunge-us-ai-disruption.html)

## License

- Code (notebook): MIT
- Data tables and prose: CC-BY-4.0, with attribution to Mohammad Ahmadi / Ahmadi Research and a
  link back to [the blog post](https://ahmadiresearch.com/blog/palantir-scorecard/).

## Author

Mohammad Ahmadi
[ahmadiresearch.com](https://ahmadiresearch.com) · [GitHub](https://github.com/mahmad100)

*Nothing here is investment advice.*
