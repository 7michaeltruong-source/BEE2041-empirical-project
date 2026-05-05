# BEE2041 Empirical Project — How Strongly Do Rating Differences Affect Chess Outcomes?

## Overview
This project analyses how rating differences affect chess game outcomes using two datasets: a personal Chess.com game archive (scraped via API) and a Lichess population dataset. The analysis uses correlation, logistic regression, and ROC curve analysis to quantify the relationship between rating differences and win probability.

**Blog post:** [link to your HackMD/published blog here]

## Data Sources
- **Personal Chess.com data:** Scraped automatically from the Chess.com public API (username: op_michael)
- **Lichess dataset:** 20,058 games from the Lichess platform via Kaggle — https://www.kaggle.com/datasets/datasnaek/chess

## Requirements
- Python 3.9+
- pandas
- numpy
- matplotlib
- statsmodels
- scikit-learn
- scipy
- requests

## How to Replicate

1. Clone the repository:
```
git clone https://github.com/7michaeltruong-source/BEE2041-empirical-project.git
cd BEE2041-empirical-project
```

2. Install the dependencies:
```
pip install pandas numpy matplotlib statsmodels scikit-learn scipy requests
```

3. Download the Lichess dataset from https://www.kaggle.com/datasets/datasnaek/chess and place `lichessgames.csv` in the root folder.

4. Launch Jupyter:
```
jupyter lab
```

5. Open and run the notebook:
   - Open `blog.ipynb`
   - Click Kernel → Restart Kernel and Run All Cells
   - The scraper will automatically collect your Chess.com data
   - All figures will be saved to the root folder

## Expected Output
Running the notebook will produce:
- `my_chess_games_scraped.csv` — personal game archive
- `fig1_comparison.png` — outcome comparison
- `fig2_my_win_probability.png` — personal win probability vs rating difference
- `fig3_lichess_win_probability.png` — Lichess population win probability
- `fig4_logistic_curve_lichess.png` — logistic regression curve
- `fig5_roc_comparison.png` — ROC curve comparison
