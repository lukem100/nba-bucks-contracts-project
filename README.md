# NBA Bucks Contracts Project 
**Project Goal**: Analyze Milwaukee Bucks player contracts to find the best "value for money" deals.

## Folder Structure
- `data/raw/`: Original data files (CSV, etc.)
- `data/processed/`: Processed or cleaned datasets
- `notebooks/`: Jupyter notebooks for exploration and final analysis
- `scripts/`: Python/R scripts for data wrangling or advanced analysis

## Getting Started
1. Clone this repository.
2. Install dependencies using `pip install -r requirements.txt` or via `conda env create -f environment.yml`.
3. Run `jupyter notebook` and open `notebooks/exploration.ipynb`.

## Data Source
I used partial NBA data from a Kaggle dataset:
- [Kaggle Data Source: https://www.kaggle.com/datasets/wyattowalsh/basketball/data?select=csv]
- Specifically, I used game_summary.csv and line_score.csv to extract scoring details quarter by quarter
## Methodology
- Brief overview of steps: data cleaning, metric calculation, visualization, results.
1. Loading Data: I identified which column holds team nicknames, points per quarter, game IDs, etc.
2. I filtered only the games where the Bucks appear, whether home or away
3. I differentiated between home and away games.
4. I then extracted q1_bucks, q1_opp and so on for the first four quarters (no overtime)
5. I computed the total 4-quarter points for the Bucks and the opponent, and then derived average points per quarter.
6. Finally I exported the results to a bucks_quartely_scoring.csv for visualization with R.
Note: The years of the data runs from 1968-2023 
## Results
- Summarize your findings or key takeaways.

## License
- MIT License. 
# nba-bucks-contracts-project
