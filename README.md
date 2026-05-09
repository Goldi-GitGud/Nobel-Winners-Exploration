# Nobel Prize winners — exploratory analysis

A small Jupyter project on Nobel laureate data: dominant gender and birth country, US-born share by decade, female representation, the first female laureate, and repeat winners.

## Requirements

- Python 3.9+
- Jupyter or VS Code with the Jupyter extension

```bash
pip install pandas numpy seaborn jupyter
```

## How to run

1. Clone or download the repo.
2. Open `workspace/notebook.ipynb` and run all cells. The notebook expects `nobel.csv` and optional `Nobel_Prize.png` in the same `workspace/` folder.

## Layout

```
Nobel-Winners-Exploration/
├── README.md
└── workspace/
    ├── notebook.ipynb
    ├── nobel.csv
    └── Nobel_Prize.png   # optional intro image
```

## Data

Laureates CSV is attributed in the notebook to the [Nobel Prize API](https://www.nobelprize.org/about/developer-zone-2/). Treat it as third-party data and follow the Nobel Foundation’s terms for reuse.

## What you get from this exploration

Working through this dataset reinforces a few practical skills:

- **Exploratory workflow** — load a real table with `pandas`, inspect distributions with `value_counts`, and derive decade-level aggregates from a year column.
- **Framing questions as code** — turn prompts (“which country dominates?”, “when was the US share highest?”, “who won more than once?”) into filters, ratios, and sorted subsets.
- **Reading results in context** — raw counts show historical imbalance (e.g. gender); decade slices show how geography and representation shift over time; repeat winners highlight individuals and institutions that appear multiple times in the record.

Together, that is a compact template for any similar CSV: define columns, group or filter, then interpret—not just print—what the numbers imply about the domain.
