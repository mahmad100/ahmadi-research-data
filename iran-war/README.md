# The Quiet Winners of the Iran War

**Published:** March 2026
**Blog post:** [ahmadiresearch.com/blog/iran-war/](https://ahmadiresearch.com/blog/iran-war/)

---

## Charts

Five visualizations accompany the blog post. All generated in `iran_war_charts.ipynb`.

| # | Chart | Key Figure |
|---|-------|------------|
| 1 | Brent Crude Oil Price Timeline (Feb-Mar 2026) | $72 pre-war to $126 peak (+55%) |
| 2 | Russia's Additional Budget Revenue (scenarios) | $45B / $97B / $151B (KSE Institute) |
| 3 | U.S. Defense Stocks: Day-1 Gains (March 2) | $200B+ combined market cap surge |
| 4 | Defense Stocks: Cumulative Gains (Jun 2025 baseline) | RTX +110%, ITA ETF +58.5% |
| 5 | China's Oil Import Exposure & Strategic Buffer | 40% via Hormuz, 1.39B bbl SPR |

## Data Sources

- **Oil prices:** CNBC ([Brent record monthly gain coverage](https://www.cnbc.com/2026/03/30/oil-price-today-wti-brent-yemen-houthis-israel-iran-war.html))
- **Russia revenues:** KSE Institute ([scenario analysis](https://kse.ua/about-the-school/news/iran-war-helps-russia-long-conflict-would-fundamentally-undermine-economic-pressure-campaign-sanctions-easing-does-not-resolve-energy-market-challenges-kse-institute)); PIIE — Ribakova & Garcia-Herrero ([How Russia and China are winning the war in Iran](https://www.piie.com/blogs/realtime-economics/2026/how-russia-and-china-are-winning-war-iran))
- **Defense stocks:** MarketMinute ([day-1 record highs](https://markets.financialcontent.com/stocks/article/marketminute-2026-3-2-defense-stocks-surge-to-record-highs-as-iran-conflict-hits-tipping-point)); Motley Fool ([cumulative gains since June 2025](https://www.fool.com/investing/2026/03/29/should-buy-defense-stocks-after-iran-conflct/)); Yahoo Finance for spot prices
- **China energy:** Vortexa — Emma Li ([crude import stress resistance](https://www.vortexa.com/insights/chinas-crude-import-stress-resistance)); Columbia SIPA CGEP — Erica Downs ([implications for China's energy security](https://www.energypolicy.columbia.edu/implications-of-the-conflict-in-the-middle-east-for-chinas-energy-security/))
- **Defense contracts:** RTX press release ([five Pentagon framework agreements](https://www.rtx.com/news/news-center/2026/02/04/rtxs-raytheon-partners-with-department-of-war-on-five-landmark-agreements-to-exp)); Lockheed Martin press release ([THAAD framework](https://investors.lockheedmartin.com/news-releases/news-release-details/lockheed-martin-and-us-department-war-sign-framework-agreement)); Breaking Defense
- **Petroyuan / dollar:** Bloomberg ([Deutsche Bank analysis](https://www.bloomberg.com/news/articles/2026-03-25/iran-war-could-be-making-of-the-petroyuan-deutsche-bank-says)); Asia Times; SCMP; Fortune

## Caveats

- **Chart 3** day-1 stock % gains are approximate; numbers vary by source within ~0.5 percentage points
- **Chart 4** cumulative gains from a June 2025 baseline are directionally confirmed but exact per-stock percentages depend on closing-price source

## Reproducing

```bash
pip install matplotlib numpy
jupyter notebook iran_war_charts.ipynb
```

Charts save to `outputs/` (git-ignored; regenerate locally).
