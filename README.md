# Dota Data Science

## Problem Description
This repository contains code and data for a hackathon focused on predicting the winner of a Dota&nbsp;2 match. Using public and private match data, the goal is to build a model that predicts whether the **Radiant** team will win.

## Data Overview
The `data/` directory includes:
- `training_features.csv` – game statistics and time-series features for matches used to train models
- `training_targets.csv` – the target variable `radiant_win` for the training set
- `test_features.csv` – features for the unseen matches used for evaluation
- `sample_submission.csv` – example of the required submission format

Each feature file contains thousands of columns describing hero choices, player metrics, and in-game events.

## Evaluation Metric
Submissions are scored using the **F1-score**, which balances precision and recall:

```
F1 = 2 * (precision * recall) / (precision + recall)
```
Participants submit a CSV with columns `match_id_hash` and `radiant_win` representing the predicted probability of a Radiant victory.

## Project Structure
```
.
├── README.md
├── PROJECT_LOG.md      # ongoing record of experiments and findings
├── AGENTS.md           # instructions for contributors
├── requirements.txt    # core dependencies
├── requirements-locked.txt
└── data/
    ├── training_features.csv
    ├── training_targets.csv
    ├── test_features.csv
    └── sample_submission.csv
```
Use `PROJECT_LOG.md` to document hypotheses, experiments, and results as the project progresses.
