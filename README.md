# Dota Data Science

This repository contains materials for a Kaggle style hackathon focused on predicting the outcome of Dota 2 matches. Participants build machine learning models using provided match statistics to determine whether the Radiant team will win. The event is designed to introduce and grow machine learning skills across the organization.

## Competition Description
The challenge uses a mix of public and professional match data from the Dota 2 game. Your goal is to train a model that can accurately predict match outcomes based on game features available at a particular point in time. Teams of up to five participants may collaborate, and the contest runs for a limited time window.

## Objective
Predict the binary target `radiant_win` for each match in the test set.

## Evaluation Metric
Submissions are scored using the F1-score which balances precision and recall:

```
F1 = 2 * (precision * recall) / (precision + recall)
```

## Data Description
Training and test CSV files contain numerous engineered features describing hero picks, game state, and other match statistics. A sample submission file is included to illustrate the expected format.

## Submission Format
Create a CSV file with two columns:

```
match_id_hash,radiant_win
abcdef1234567890abcdef1234567890abcdef12,True
...
```
The file must contain a prediction for each match in the provided test set.

## Important Dates / Timeline
* **Start:** April 21, 2025 at 11:00 MT
* **Close:** May 9, 2025 at 12:00 MT
* Results and awards will be announced shortly after the competition closes.

## Project Structure
- `data/` – competition datasets
- `notebooks/` – exploratory notebooks
- `src/` – reusable modules and scripts

## Getting Started
Instructions for setting up the environment and running notebooks will be added here. For now, install dependencies with `make setup`.
