# The Numb Market — Companion Data

Reproducible code for the Ahmadi Research blog post
**[The Numb Market](https://ahmadiresearch.com/blog/numb-market/)**.

This notebook regenerates every chart in the post from publicly available primary sources, with
the data inline and the full source list at the bottom of the notebook.

> "If someone with the same data can't get to the same conclusion, the analysis isn't done."
> — [ahmadiresearch.com/approach](https://ahmadiresearch.com/approach.html)

---

## What's in here

```
Numb_Market_Charts.ipynb   The notebook: three charts, data inline.
README.md                  This file.
requirements.txt           Python dependencies. Standard scientific Python.
```

The source research report (`The_Numb_Market_v2.docx`) is **not part of this package**.

## Quickstart

```bash
# 1. Clone or download this folder
# 2. Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the notebook
jupyter notebook Numb_Market_Charts.ipynb
```

Run the cells top to bottom.

## Charts reproduced

| #  | Chart                                              | Source(s)                              |
|----|----------------------------------------------------|----------------------------------------|
| 1  | Shock-response curve (S&P 500 reaction to shocks)  | CNBC [6]; Supreme Court [1]; CBOE; FactSet [4] |
| 2  | Bifurcation — S&P 500 vs. UMich Current Conditions | S&P; UMich Surveys of Consumers [3]; Bloomberg [12] |
| 3  | April 2025 10-year Treasury yield surge            | Bloomberg [14]; NY Fed [14]; CNBC [15] |

## Things worth changing

Two data choices are open to substitution:
- Monthly S&P 500 closes are end-of-month. Substitute the daily series if you want intra-month
  precision around the Liberation Day window.
- UMich Current Conditions readings are monthly. For more granularity, swap in the Conference
  Board Consumer Confidence Index or the weekly Langer Consumer Comfort series.

## Sources

The full numbered reference list is in the final cell of the notebook. Key sources:

- S&P 500 closes and earnings: [CNBC](https://www.cnbc.com/2026/04/30/stock-market-today-live-updates.html);
  [FactSet Earnings Insight](https://insight.factset.com/sp-500-earnings-season-update-may-8-2026)
- Liberation Day and the April 2025 panic:
  [CNBC](https://www.cnbc.com/2025/04/03/stock-market-today-live-updates.html);
  [Macroption (VIX)](https://www.macroption.com/vix-all-time-high/)
- Tariff pause and the bond market:
  [Bloomberg](https://www.bloomberg.com/news/articles/2025-04-11/us-treasury-selloff-is-worst-since-repo-market-chaos-in-2019);
  [CBS News](https://www.cbsnews.com/news/trump-tariff-pause-bond-market-bond-yield-treasury-bill/);
  [CNBC, Apr 10 2025](https://www.cnbc.com/2025/04/10/trump-dodged-a-disaster-from-the-bond-market-but-the-damage-isnt-over-yet.html)
- SCOTUS IEEPA ruling:
  [SCOTUS opinion 24-1287](https://www.supremecourt.gov/opinions/25pdf/24-1287_4gcj.pdf);
  [SCOTUSblog](https://www.scotusblog.com/2026/02/supreme-court-strikes-down-tariffs/)
- Hormuz disruption: [IEA Oil Market Report, April 2026](https://www.iea.org/reports/oil-market-report-april-2026)
- Consumer sentiment:
  [University of Michigan Surveys of Consumers](https://www.sca.isr.umich.edu/);
  [Advisor Perspectives](https://www.advisorperspectives.com/dshort/updates/2026/04/28/two-measures-of-consumer-attitudes-april-2026);
  [Bloomberg](https://www.bloomberg.com/news/articles/2026-04-24/us-consumer-sentiment-falls-to-record-low-on-inflation)
- Fiscal: [CBO Monthly Budget Review FY2025](https://www.cbo.gov/publication/61307)
- Tariff rates:
  [Yale Budget Lab](https://budgetlab.yale.edu/research/state-us-tariffs-april-2-2026);
  [Penn Wharton Budget Model](https://budgetmodel.wharton.upenn.edu/p/2026-04-15-effective-tariff-rates-and-revenues-updated-april-15-2026/)
- Dollar:
  [Bloomberg, Dec 23 2025](https://www.bloomberg.com/news/articles/2025-12-23/usd-dollar-s-worst-slide-since-2017-has-further-to-go-options-show)

## License

- Code (notebook): MIT
- Data tables and prose: CC-BY-4.0, with attribution to Mohammad Ahmadi / Ahmadi Research and a
  link back to [the blog post](https://ahmadiresearch.com/blog/numb-market/).

The source research report is **not licensed for redistribution** and is not included here.

## Author

Mohammad Ahmadi
[ahmadiresearch.com](https://ahmadiresearch.com) · [GitHub](https://github.com/mahmad100)

*Nothing here is investment advice.*
