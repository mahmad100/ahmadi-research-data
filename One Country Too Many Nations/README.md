# One Country, Too Many Nations — Companion Data

Reproducible data and code for the Ahmadi Research blog post
**["One Country, Too Many Nations: What America Got Wrong in Afghanistan"](https://ahmadiresearch.com/blog/one-country-too-many-nations/)**.

This package lets anyone regenerate every chart in the post from cited sources, change the
assumptions, and rerun. It exists because of the rule on the [Approach
page](https://ahmadiresearch.com/approach.html):

> "If someone with the same data can't get to the same conclusion, the analysis isn't done."

---

## What's in here

```
Afghanistan_Data.ipynb     The notebook. Four charts, all data inline, every claim cited.
README.md                  This file.
requirements.txt           Python dependencies. Standard scientific Python.
```

The original class paper that started this analysis (Tufts EC 184, Number and Size of Nations,
May 2025) is **not part of this public package**. The blog post is the published version.

## Quickstart

```bash
# 1. Clone or download this folder
# 2. Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the notebook
jupyter notebook Afghanistan_Data.ipynb
```

Run the cells top to bottom. Every chart in the live blog post comes from data in this notebook.

## Charts reproduced

| #  | Chart                                              | Source(s)                              |
|----|----------------------------------------------------|----------------------------------------|
| 1  | Marshall Plan vs. Afghanistan spending             | Brown Costs of War; Marshall Plan diplomacy archive |
| 2  | Estimated ethnic composition of Afghanistan        | Minority Rights Group International    |
| 3  | Pashtun rule timeline, 1747–2021                   | Al Jazeera (Kalakani); MRG (Rabbani)   |
| 4  | Federalism vs. post-conflict stability             | Author scoring across cited cases      |

The blog post replaces Chart 2 with a stylized map of Afghanistan rendered in inline SVG. The
country outline used there comes from [djaiss/mapsicon](https://github.com/djaiss/mapsicon) (MIT).
The bar version in this notebook is the cleanest reproducible form for the underlying numbers.

## Sources

Full numbered reference list lives in the final cell of the notebook and matches the citation
numbers in the live blog post. Highlights:

- Marshall Plan: [National Museum of American Diplomacy](https://diplomacy.state.gov/online-exhibits/diplomacy-is-our-mission/development/the-marshall-plan/)
- Afghanistan reconstruction cost: [Brown Costs of War](https://www.brown.edu/news/2021-09-01/costsofwar)
- Ethnic composition: [Minority Rights Group](https://minorityrights.org/country/afghanistan/)
- Centralization critique: [Alex Thier (USIP, 2020)](https://www.usip.org/sites/default/files/Afghanistan-Peace-Process_Nature-of-the-Afghan-State_Centralization-vs-Decentralization.pdf); [The Diplomat (2021)](https://thediplomat.com/2021/08/afghanistans-failed-constitution/)
- Theory: Alesina & Spolaore, *The Size of Nations* (MIT, 2003); Montalvo & Reynal-Querol, "Ethnic Polarization, Potential Conflict, and Civil Wars," AER 2005
- Taliban demographics: [MEI Taliban Leadership Tracker](https://talibantracker.mei.edu/english/taliban/demographics) (~90% Pashtun)
- Comparative cases: India ([Britannica](https://www.britannica.com/topic/States-Reorganization-Act)), Iraq ([EISMENA, 2023](https://eismena.com/en/article/iraqi-federalism-the-second-best-option-for-everyone-2023-10-25)), Ethiopia ([Habtu, 2003](https://scholarworks.wmich.edu/africancenter_icad_archive/79/); [Wilson Center, 2021](https://www.wilsoncenter.org/blog-post/ethiopia-faces-dire-consequences-ethnic-federalism)), Yugoslavia ([Critchley, *International Journal*, 1993](https://journals.sagepub.com/doi/abs/10.1177/002070209304800302))

## What you can change

The point of publishing the data is so you can argue with it. Things worth toying with:

- The 2024-dollar adjustment on Afghanistan spend (currently ~+12% over the cumulative nominal
  total). A year-by-year deflation would be more precise.
- Ethnic-composition shares (no national census since 1979; Minority Rights Group ranges differ
  from CIA Factbook ranges by a few points).
- Federalism / stability scores in Chart 4 are author judgment on a 0–5 rubric. Argue with them.
- Whether Pakistan's $2.3T should be called Afghanistan's $2.3T, since Brown's number includes
  the Afghanistan/Pakistan war zone. The post uses Brown's framing.

## License

- Code (notebook): MIT
- Data tables and prose: CC-BY-4.0 — attribute Mohammad Ahmadi / Ahmadi Research and link back to
  [the blog post](https://ahmadiresearch.com/blog/one-country-too-many-nations/).

The class paper is **not licensed for redistribution** and is not included here.

## Author

Mohammad Ahmadi
[ahmadiresearch.com](https://ahmadiresearch.com) · [GitHub](https://github.com/mahmad100)
