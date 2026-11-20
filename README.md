# Predicting Premier League Home Wins

CT4101 Machine Learning project. The goal is to predict whether the home team wins a
Premier League match using only information available before kick-off - Bet365 odds
and each team's form over their last 5 matches.

## Data
- **Source:** [Football-Data.co.uk](https://www.football-data.co.uk/englandm.php), Premier League results and betting odds, 2015/16 to 2024/25 (3800 matches)
- **Licence:** no formal licence. The data is provided free for match prediction. The CSV files are not included in the repository.
- The notebook downloads the data automatically into a `data/` folder the first time it runs. Internet connection is needed.

## Requirements
- Python 3.11.9 
- Packages listed in `requirements.txt`

## Setup
```
git clone https://github.com/jonesyadam111/CT4101-premier-league-prediction.git
cd CT4101-premier-league-prediction
python -m venv .venv
.venv\Scripts\Activate.ps1        # Windows (PowerShell)
# source .venv/bin/activate       # macOS / Linux
pip install -r requirements.txt
```

## How to run
1. Open `premier_league_prediction.ipynb` in VS Code or Jupyter.
2. Select the `.venv` environment as the kernel.
3. Restart the kernel and click Run All. The notebook runs from top to bottom
   with no other steps needed.

## Progress
- **Milestone 2:** data loading, data audit, form features, time based train/test
  split, preprocessing pipeline and baselines.

- **Milestone 3:** logistic regression and random forest models, random forest
  tuning, results table, confusion matrix, error analysis and draft conclusion. 

- **Milestone 4 (final):** cut off choice, final test on the locked 2023/24 and
  2024/25 seasons, permutation feature importance and final conclusion.

## Project structure
```
CT4101-premier-league-prediction/
|__ premier_league_prediction.ipynb   # full workflow: data, features, models, results
|__ requirements.txt                  # Python packages and versions
|__ README.md                         # this file
|__ .gitignore                        # keeps data/ and .venv/ out of the repo
|__ data/                             # created when the notebook runs (not in repo)
``` 