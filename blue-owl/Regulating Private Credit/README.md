# The Case for Regulating Private Credit: Companion Data

Reproducible data and code for the Ahmadi Research thematic post
**"The Case for Regulating Private Credit: How a $2.3 Trillion Industry
Outgrew Its Oversight."**

- Live post: [ahmadiresearch.com/blog/regulating-private-credit/](https://ahmadiresearch.com/blog/regulating-private-credit/) (forthcoming)
- Author: Mohammad Ahmadi

This package lets anyone regenerate every chart in the post from cited sources,
change the assumptions, and rerun. It exists because of the rule on the
[Approach page](https://ahmadiresearch.com/approach.html):

> "If someone with the same data can't get to the same conclusion, the analysis isn't done."

---

## What's in here

```
Blue_Owl_Charts.ipynb     14 charts, all data inline, every claim cited.
Blue_Owl_Sources.ipynb    Per-chart source map plus curated bibliography.
README.md                 This file.
requirements.txt          Python dependencies. Standard scientific Python.
```

## Quickstart

```bash
# 1. Clone or download this folder
# 2. Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the charts notebook
jupyter notebook Blue_Owl_Charts.ipynb
```

Run the cells top to bottom. Every chart in the live post comes from data
in this notebook.

## Charts reproduced

| #  | Chart                                                     | Key sources                                                                |
|----|-----------------------------------------------------------|----------------------------------------------------------------------------|
| 1  | Private Credit: A 40-Year Timeline                        | Preqin; McKinsey GPMR; SEC                                                 |
| 2  | How Private Credit Works                                  | Investment Company Act 1940; Blue Owl, Ares, Apollo 10-Ks                  |
| 3  | The Private Credit Promise                                | Cliffwater Direct Lending Index; LSEG LPC; PitchBook LCD                   |
| 4  | Private Credit AUM Growth, 2010-2025                      | Preqin Global Private Debt Reports; McKinsey GPMR (2024, 2025)             |
| 5  | Private Credit Share of LBO Financing, 2014-2024          | LSEG LPC; PitchBook LCD; ABF Journal / S&P Global                          |
| 6  | The Business Grew. The Stock Didn't.                      | Blue Owl 10-K (FY2025); quarterly earnings decks; Yahoo Finance            |
| 7  | Two Years, $142B of AUM Growth (waterfall)                | Blue Owl quarterly earnings decks Q4'23-Q4'25; 10-K (FY2025)               |
| 8  | Where Blue Owl's Revenue Comes From, and Where It Goes    | Blue Owl 10-K (FY2025); Q4 2025 Earnings Deck                              |
| 9  | Software / SaaS Concentration                             | Morgan Stanley IM; Blue Owl Q4 2025 deck; OTIC prospectus; CNBC            |
| 10 | Blue Owl's Redemption Crisis Escalated in Six Months      | Bloomberg; FT; Citywire; OCIC 10-K; OBDC II 8-K                            |
| 11 | OWL Has Never Sustainably Traded Above Its SPAC Valuation | Yahoo Finance / Bloomberg; Blue Owl IR                                     |
| 12 | Q1 2026 Multi-Sponsor Redemption Pressure                 | PitchBook; Bloomberg; WithIntelligence; Bisnow / GlobeSt                   |
| 13 | BREIT vs Blue Owl: A Counterexample                       | Blackstone press release; Blackstone Q4 earnings; Blue Owl Q4 2025 deck    |
| 14 | The Regulatory Gap: Banks vs Private Credit               | Federal Reserve FEDS Notes; NAPFM v. SEC, 5th Cir.; AIFMD II               |

The full per-chart source map plus the curated bibliography live in
`Blue_Owl_Sources.ipynb`.

## Sources highlights

The post leans on five categories of sources. The curated bibliography in
`Blue_Owl_Sources.ipynb` lists each one; load-bearing items include:

- **Court decisions:** *NAPFM v. SEC*, No. 23-60471 (5th Cir., Jun 5, 2024).
  Vacated the SEC Private Fund Advisers Rule. Slip opinion at
  [ca5.uscourts.gov](https://www.ca5.uscourts.gov/opinions/pub/23/23-60471CV0.pdf).
- **EU regulation:** [Directive 2024/927 (AIFMD II)](https://eur-lex.europa.eu/eli/dir/2024/927/oj/eng).
  Loan-origination rules and 175% / 300% NAV leverage limits, transposition
  by April 16, 2026.
- **UK supervisory:** [FCA Asset Management & Alternatives Portfolio Letter](https://www.fca.org.uk/publication/correspondence/portfolio-letter-asset-management-alternatives-supervisory-strategy-interim-update.pdf)
  (Mar 1, 2024). Multi-firm review of private market valuation governance.
- **Australian supervisory:** [ASIC REP 820](https://download.asic.gov.au/media/q42bgduw/rep820-published-5-november-2025.pdf)
  (Nov 5, 2025). Surveillance of 28 funds; private credit named a 2026
  enforcement priority.
- **Federal Reserve research:** FEDS Notes "Private Credit: Characteristics
  and Risks" (Feb 23, 2024); Boston Fed Current Policy Perspectives 25-8 on
  whether private credit growth poses a financial-stability risk.

## What you can change

The point of publishing the data is so you can argue with it. Things worth
toying with:

- Platform-level AUM splits in Chart 7 (Credit / GPSC / Real Assets at Dec '23
  and Dec '25) are author estimates from disclosed segment data. Reconcile
  against the 10-K segment footnote and rerun.
- The "EBITDA" proxy in Chart 6 is GAAP operating income plus amortization of
  intangibles. Blue Owl reports "fee-related earnings" and "distributable
  earnings" as alternative non-GAAP measures; swap in either if you prefer.
- The sector-software figure of 26% in Chart 9 comes from Morgan Stanley IM.
  Different industry sources put it between 22% and 30%.
- The regulatory-gap rubric in Chart 14 is a Yes / Minimal / No scoring.
  Reasonable people could put "Standardized disclosure" higher for private
  credit (registered BDCs do file 10-Ks) or lower for banks (Pillar 3
  disclosures vary).

## License

- Code (notebooks): MIT
- Data tables and prose: CC-BY-4.0. Attribute Mohammad Ahmadi / Ahmadi
  Research and link back to the post.

## Author

Mohammad Ahmadi
[ahmadiresearch.com](https://ahmadiresearch.com) · [GitHub](https://github.com/mahmad100)
