# Kaggle regression competitions (reference for our own competition)

Process we want: pick features → check p-value / t-statistic / R² / adjusted R² →
add or remove features → finalize → train → measure RMSE.

Kaggle only auto-scores predictions (RMSE). The p-value / feature-selection work
has to be graded separately (notebook or short report).

## Best matches

### Regression challenge (CU Boulder, CSCI 4622), 2020
https://www.kaggle.com/c/cu-regression-challenge
- Community (class) competition: predict King County house prices from 20 features
- Metric: RMSE
- Hidden extra test set, so rankings can change when the competition closes (public/private leaderboard)
- Teams of 2–3; students also submitted code + a 1–2 page report (that's what got graded)
- Best template for structuring our own class competition
- Watch out: its evaluation text mentions "taking logs", which doesn't match plain RMSE

### Predicting Student Test Scores (Playground Series S6E1), Jan 2026
https://www.kaggle.com/competitions/playground-series-s6e1/overview
- Run by Kaggle, tagged Beginner, metric: RMSE
- Synthetic data (generated to keep test answers private)
- Late submissions still accepted, good for practice
- Very large dataset, so nearly every feature gets a tiny p-value; not ideal for practicing p-value selection

## Other options
- IEEE GUC Linear Regression Competition (housing, RMSE):
  https://www.kaggle.com/competitions/ieee-guc-linear-regression-competition
- Linear regression simple challenge (scored by R², not RMSE):
  https://www.kaggle.com/competitions/linear-regression-simple-challenge
- LHS ML Club Challenge #1: Linear Regression (scored by MAE, not RMSE):
  https://www.kaggle.com/competitions/lhs-ml-club-kaggle-challenge-1-linear-regression
- Regression of Used Car Prices (Playground S4E9, RMSE):
  https://www.kaggle.com/competitions/playground-series-s4e9
- Some Playground regression competitions use RMSLE (log variant) instead; check each Evaluation tab.

## Ideas for our own competition
- Host via Kaggle: Host a Competition → Community (free, can be invite-only)
- Use a few hundred rows so p-values actually separate useful vs. useless columns
- Synthetic "real-life" dataset with planted useless + correlated columns (no answers online)
- Public/private leaderboard split (~30/70), ~5 submissions per day
- Grade: leaderboard RMSE + notebook rubric (feature selection, no leakage, residual check)
