# Nobel Prize winners — exploratory analysis

A short Jupyter notebook project that loads Nobel Prize winner data and explores gender, birth country, decades, the first female laureate, and repeat winners.

## Requirements

- Python 3.9 or newer
- [Jupyter](https://jupyter.org/) or [VS Code](https://code.visualstudio.com/) with the Jupyter extension

Packages used in the notebook:

- `pandas`
- `numpy`
- `seaborn`

Install (use a virtual environment if you prefer):

```bash
pip install pandas numpy seaborn jupyter
```

## How to run

1. Clone or download this repository.
2. The notebook reads **`data/nobel.csv`** relative to the notebook folder. Create `workspace/data/` and place `nobel.csv` there (you can copy the `workspace/nobel.csv` file from this repo into `workspace/data/nobel.csv`).
3. Open `workspace/notebook.ipynb` in Jupyter or VS Code and run all cells.

If `workspace/Nobel_Prize.png` is missing, any intro cell that references it may show a broken image until you add the file or update the markdown path.

## Project layout

```
Nobel-Winners-Exploration/
├── README.md
└── workspace/
    ├── notebook.ipynb
    ├── nobel.csv          # copy into data/nobel.csv before running (see How to run)
    └── Nobel_Prize.png    # optional asset for the intro
```

The notebook calls `pd.read_csv("data/nobel.csv")`, so you need `workspace/data/nobel.csv` (create the `data` folder if it is not there yet).

## Data

The laureates CSV is described in the notebook as coming from the [Nobel Prize API](https://www.nobelprize.org/about/developer-zone-2/) (Nobel Foundation dataset). Treat the file as third-party data and respect the Nobel Foundation’s terms for reuse.
