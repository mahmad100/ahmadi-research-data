# The Unraveling Guarantee

Reproducible data and code for the Ahmadi Research deck
**"The Unraveling Guarantee: Has the U.S. Lost Its Exorbitant Privilege?"**

- Deck: [ahmadiresearch.com/papers/the-unraveling-guarantee-feb2026.pdf](https://ahmadiresearch.com/papers/the-unraveling-guarantee-feb2026.pdf)
- Author: Mohammad Ahmadi

This package lets a reader regenerate every chart in the deck from cited
sources, change the assumptions, and rerun.

---

## What's in here

```
Unraveling_Guarantee_Charts.ipynb     20 figures, live FRED data where available, every claim cited.
Unraveling_Guarantee_Sources.ipynb    Per-figure source map plus curated bibliography.
README.md                             This file.
requirements.txt                      Python dependencies. Standard scientific Python.
```

## Quickstart

```bash
# 1. Clone or download this folder
# 2. Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate    # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the charts notebook
jupyter notebook Unraveling_Guarantee_Charts.ipynb
```

Run the setup cell first, then any section cell top to bottom. Every figure
in the deck comes from data in this notebook.

## Figures reproduced

| Section | Figure | Title |
|---|---|---|
| I.3 | 1.1 | U.S. Federal Debt and Fiscal Balance, 1970-Present |
| I.3 | 1.2 | CBO Long-Term Debt-to-GDP, Baseline vs. Alternative Scenarios, 2025-2055 |
| II.1 | 2.1 | Key Fiscal Metrics, FY2019-FY2035 |
| II.2 | 2.2 | The Interest Expense Trap |
| II.3 | 2.3 | The Maturity Structure Problem |
| III.1 | 3 | Fiscal Dominance, r-g Gap and Fed Funds vs. Net Interest Expense |
| III.2 | 3.1 | Federal Reserve Total Assets, 2006-2026 |
| III.2 | 3.2 | SOMA Unrealized Losses and Deferred Asset |
| III.2 | 3.3 | Annual Fed Remittances to U.S. Treasury, 2000-2025 |
| III.3 | 3.4 | Federal Spending by Component, 2000-2025 |
| III.3 | 3.5 | Mandatory Spending Components and Net Interest |
| III.3 | 3.6 | Federal Revenue and Outlays as % of GDP, 1970-2025 |
| IV.2 | 4.1 | Channel 1, Inflation, CPI vs. 10-Year Treasury Yield |
| IV.3 | 4.2 | Channel 2, Financial Repression, Real Fed Funds Rate, 1955-2026 |
| IV.4 | 4.3 | Channel 3, Dollar Debasement, USD Share of Global FX Reserves |
| V.1 | 5.1 | Money Supply Growth vs. Inflation |
| V.2 | 5.2 | Federal Funds Rate and Treasury Yields, 1954-Present |
| V.3 | 5.3 | The r-g Spread and Historical Debt-Reduction-Episode Growth Rates |
| V.4 | 5.4 | U.S. vs. Japan, Comparative Dashboard |
| VII | 7 | Investment and Geopolitical Implications |

The per-figure source map plus the curated bibliography live in
`Unraveling_Guarantee_Sources.ipynb`.

## Sources highlights

The deck leans on five categories of sources. The curated bibliography in
`Unraveling_Guarantee_Sources.ipynb` lists each one. Load-bearing items
include:

- **Congressional Budget Office**, *Long-Term Budget Outlook 2025* (Pub. 61187,
  Mar 2025) and *Alternative Scenarios* (Pub. 61429, May 2025). The CBO
  Extended Baseline anchors Figure 1.2 and the FY2035 projections in
  Figures 2.1 and 2.2.
- **Federal Reserve H.4.1 and Combined Quarterly Financial Statements**.
  The balance-sheet trajectory in Figure 3.1 comes from H.4.1; the
  unrealized losses and deferred-asset series in Figures 3.2 and 3.3 come
  from the Combined Quarterly Financial Statements.
- **U.S. Treasury Monthly Statement of the Public Debt (MSPD), December
  2025, Table III-A**. The maturity-bucket composition in Figure 2.3 is
  read directly from this table.
- **IMF Currency Composition of Official Foreign Exchange Reserves
  (COFER)**, World Aggregates Q3 2025. Figure 4.3 left panel.
- **Sargent and Wallace (1981)**, *Some Unpleasant Monetarist Arithmetic*,
  and **Reinhart and Sbrancia (2015)**, *The Liquidation of Government Debt*.
  The fiscal-dominance framing in Section III and the financial-repression
  framing in Section IV rest on these.

## What you can change

Things worth toying with:

- **CBO scenario anchors in Figure 1.2** are the published 2024, 2025,
  2028, 2035, 2040, 2045, 2050, and 2055 anchor years. Intermediate years
  use a cubic spline. Replace with a linear interpolation if a flatter
  trajectory matches your prior.
- **Rate-scenario shifts in Figure 2.2** are -100bps, hold, and +150bps
  relative to the FY2025 implied effective rate of about 2.58%. Substitute
  your own scenario set in `ia`, `ib`, `ic` to test a different policy
  path.
- **Debt growth assumption in Figure 2.2** is the CBO baseline of about
  $1.5T per year. Swap `debts = debt25 + 1.5 * np.arange(11)` for a
  different trajectory.
- **The 10-year Treasury yield series in Figure 4.1** is built from
  representative monthly anchors. The August 2020 0.65% issuance is fixed
  per the deck. Swap in a full GS10 pull from FRED for higher fidelity.
- **The 2010-2021 average remittance baseline in Figure 3.3** is computed
  across twelve fiscal years. Change the window to test how sensitive the
  decade-average reference line is to start and end dates.
- **Hardcoded quarterly SOMA losses and deferred-asset values in
  Figure 3.2** come from the Federal Reserve Combined Quarterly Financial
  Statements. Reconcile against the latest statement and rerun.

## License

- Code (notebooks): MIT
- Data tables and prose: CC-BY-4.0. Attribute Mohammad Ahmadi / Ahmadi
  Research and link back to the deck.

## Author

Mohammad Ahmadi
[ahmadiresearch.com](https://ahmadiresearch.com) , [GitHub](https://github.com/mahmad100)

*Nothing here is investment advice.*
