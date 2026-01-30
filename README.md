# How Much Does It Cost to Win in the NBA?

## Overview
This project analyzes historical NBA team payroll data to investigate how much it costs to win an NBA championship and how that cost has changed over time. Using inflation-adjusted team payrolls and championship outcomes, the analysis explores long-term financial trends and the relationship between team spending and championship success.

The primary outputs of this project are exploratory visualizations and summary statistics generated in a Jupyter notebook.

## Data
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

## Project Structure
├── notebooks/
│ └── nba_payroll_analysis.ipynb
├── data/
│ └── raw/ # External CSV files (not tracked in Git)
├── results/
│ └── figures/ # Generated plots (optional)
├── README.md
├── requirements.txt
└── .gitignore


---

## Data
This project uses multiple external datasets related to NBA payrolls, player salaries, and championship results.

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

Environment Setup (uv)

This project uses uv for fast and reproducible Python environment management.

Create and activate the virtual environment using both lines:
```bash
uv venv
source .venv/bin/activate
```

Install dependencies:

```bash
uv pip install -r requirements.txt
```

numpy
pandas
matplotlib
scipy

## Reproducing Results
To reproduce one of the key results (e.g., the comparison of championship payrolls vs. league averages):

Clone the repository:

git clone <your-repo-url>
cd <your-repo-name>


Set up the environment (see above).

Download the required datasets and place them in:
data/raw/


Open the notebook:
jupyter notebook notebooks/nba_payroll_analysis.ipynb


Run all cells from top to bottom.

## References

Lauton, Logan. “NBA Players & Team Data.” Kaggle, 6 Apr. 2023.
https://www.kaggle.com/datasets/loganlauton/nba-players-and-team-data

“List of NBA Champions.” Wikipedia, Wikimedia Foundation.
https://en.wikipedia.org/wiki/List_of_NBA_champions

Matplotlib Pie Charts.
https://www.w3schools.com/python/matplotlib_pie_charts.asp

Stack Overflow discussions on data cleaning and visualization.