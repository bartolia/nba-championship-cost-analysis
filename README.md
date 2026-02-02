# How Much Does It Cost to Win in the NBA?

## Overview
This project analyzes historical NBA team payroll data to investigate how much it costs to win an NBA championship and how that cost has changed over time. Using inflation-adjusted team payrolls and championship outcomes, the analysis explores long-term financial trends and the relationship between team spending and championship success.

The primary outputs of this project are exploratory visualizations and summary statistics generated in a Jupyter notebook.

## Project Structure
>nba-championship-cost-analysis/
>├── notebooks/
>│   └── nba_payroll_analysis.ipynb
>├── data/
>│   └── raw/          # empty, gitignored
>├── pyproject.toml
>├── uv.lock
>├── requirements.txt  # optional fallback
>├── .gitignore
>└── README.md



---

## Data
This project uses multiple external datasets related to NBA payrolls, player salaries, and championship results.

This project uses multiple external datasets:

- NBA team payroll and salary data (1990–2023)
- Player statistics and box score data
- NBA championship results by season

The notebook expects files with names such as:
- `NBAPayroll(1990-2023).csv`
- `NBASalaries(1990-2023).csv`
- `NBAPlayerStats(1950-2022).csv`
- `NBAPlayerBoxScoreStats(1950-2022).csv`

These files are not included in the repository but the link is at the top of the notebook

### Data sources
- **Kaggle – NBA Players & Team Data**  
  https://www.kaggle.com/datasets/loganlauton/nba-players-and-team-data

- **Wikipedia – List of NBA Champions**  
  https://en.wikipedia.org/wiki/List_of_NBA_champions

### Expected data location
Downloaded CSV files should be placed in:
data/raw/


The notebook expects files with names such as:
- `NBAPayroll(1990-2023).csv`
- `NBASalaries(1990-2023).csv`
- `NBAPlayerStats(1950-2022).csv`
- `NBAPlayerBoxScoreStats(1950-2022).csv`

**Note:** These data files are not included in the repository due to size and licensing constraints. Links to download the data are provided above and at the top of the notebook.

---

Environment Setup (Recommended: uv)
Why uv?

This project uses uv for fast, reproducible Python environment management.
Using uv.lock ensures everyone runs the exact same dependency versions.

Install uv

macOS / Linux
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
Windows (PowerShell)
```

Windows (powershell)
powershell
irm https://astral.sh/uv/install.ps1 | iex


Set up the environment
```
bash
uv sync
```

Alternative: Traditional venv (Optional)
```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.venv\Scripts\activate      # Windows
pip install -r requirements.txt
```


Note: requirements.txt is provided for compatibility, but uv is preferred.

numpy
pandas
matplotlib
scipy

## Reproducibility
To reproduce one of the key results (e.g., the comparison of championship payrolls vs. league averages):

Clone the repository:

git clone <your-repo-url>
cd <your-repo-name>

Set up the environment (see above).

Download the required datasets and place them in:
data/raw/

This project is fully reproducible using `uv`.

After cloning the repository and downloading the data:
1. Run `uv sync`
2. Open the notebook in Jupyter
3. Run all cells from top to bottom

All dependency versions are pinned in `uv.lock`.


## References

Lauton, Logan. “NBA Players & Team Data.” Kaggle, 6 Apr. 2023.
https://www.kaggle.com/datasets/loganlauton/nba-players-and-team-data

“List of NBA Champions.” Wikipedia, Wikimedia Foundation.
https://en.wikipedia.org/wiki/List_of_NBA_champions

Matplotlib Pie Charts.
https://www.w3schools.com/python/matplotlib_pie_charts.asp

Stack Overflow discussions on data cleaning and visualization.