# Ahmadi Research — Data & Process

Public companion to [ahmadiresearch.com](https://ahmadiresearch.com). Charts, notebooks,
and data behind published research.

> "If someone with the same data can't get to the same conclusion, the analysis isn't done."
> — [ahmadiresearch.com/approach](https://ahmadiresearch.com/approach.html)

The site publishes the analysis. This repo shows the work.

## Projects

```
iran-war/                          The Quiet Winners of the Iran War (March 2026)
                                   ahmadiresearch.com/blog/iran-war/

One Country Too Many Nations/      One Country, Too Many Nations: What America Got Wrong
                                   in Afghanistan (April 2026)
                                   ahmadiresearch.com/blog/one-country-too-many-nations/
```

More folders will be added as new research is published.

## What's in each project folder

- A Jupyter notebook that regenerates every chart in the live blog post
- A README documenting the data, sources, and any caveats
- A `requirements.txt` for the Python environment

Run a notebook by cloning the repo, installing dependencies, and opening it:

```bash
git clone https://github.com/mahmad100/ahmadi-research-data.git
cd ahmadi-research-data/iran-war
pip install -r requirements.txt   # if a requirements file is present in the folder
jupyter notebook
```

## Tools

Python 3, pandas, numpy, matplotlib, Jupyter. Off-the-shelf, no proprietary data.

## What's not here

Drafts, working spreadsheets, brand guides, and unfinished projects stay private.
Each blog post links here once the analysis is published.

## Contact

Mohammad Ahmadi
- [ahmadiresearch.com](https://ahmadiresearch.com)
- [LinkedIn](https://linkedin.com/in/mo-ahmadi-)

*Nothing here is investment advice.*
