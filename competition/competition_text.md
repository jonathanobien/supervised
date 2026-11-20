# Competition text (copy each section into Kaggle)

---

## Title
Real Estate Price Prediction: Regression Challenge

## Subtitle
Predict house prices in New Taipei City with multiple linear regression

---

## Overview / Description

Can you predict what a house is worth?

In this competition you will use **real housing sales** from Sindian District, New Taipei City, Taiwan,
to predict each house's **price per unit area**.

Follow the regression process from class:

1. Split the training data into your own train and test parts
2. Train a model with all features and read the summary: **coefficients, t-statistics, p-values, R², adjusted R²**
3. Keep the significant features (p < 0.05) and retrain
4. Check your **RMSE**
5. Retrain on all of `train.csv`, predict `test.csv`, and submit

A starter notebook that follows these steps is provided. Can you beat it?

**Hint:** plot price against each feature. Is every relationship a straight line?

---

## Evaluation

Submissions are scored with **Root Mean Squared Error (RMSE)** between the predicted and actual
`price_per_area`. Lower is better.

RMSE = √( average of (predicted − actual)² )

### Submission file
For each `id` in `test.csv`, predict `price_per_area`. The file must have a header and this format:

```
id,price_per_area
332,38.15
333,38.15
334,38.15
...
```

`sample_submission.csv` shows the correct format (it predicts the average price for every house).

### Leaderboard
- The **public leaderboard** is scored on about 30% of the test data and is visible during the competition.
- The **private leaderboard** is scored on the other 70% and is revealed when the competition closes.
  **Final rankings use the private leaderboard**, so don't tune your model just to climb the public one.

---

## Timeline
- **Final submission deadline:** December 2, 2026, 11:59 PM UTC

---

## Data description

### Files
- `train.csv`: 331 houses **with** prices. Use this to build your model.
- `test.csv`: 83 houses **without** prices. Predict these.
- `sample_submission.csv`: a correctly formatted example submission.

### Columns

| Column | Meaning | Unit |
|---|---|---|
| id | house ID | |
| transaction_date | date of sale (2013.250 = March 2013, 2013.500 = June 2013) | year |
| house_age | age of the house | years |
| distance_to_mrt | distance to the nearest MRT (metro) station | meters |
| convenience_stores | number of convenience stores within walking distance | count |
| latitude | location, north–south | degrees |
| longitude | location, east–west | degrees |
| **price_per_area** (target) | house price per unit area | 10,000 New Taiwan Dollars per ping (1 ping = 3.3 m²) |

### Source and license
Yeh, I. (2018). Real Estate Valuation [Dataset]. UCI Machine Learning Repository.
https://doi.org/10.24432/C5J30W. Licensed under CC BY 4.0. Column names were shortened and rows
re-numbered for this competition.

---

## Rules

1. **Individual competition**: one account per person, no teams.
2. **Up to 5 submissions per day.** Select up to **2 final submissions** for scoring.
3. **No looking up the answers.** This is a public dataset. Using the original dataset to find the true
   prices of test houses is not allowed. Your model must learn only from `train.csv`.
4. **Submit your notebook.** Your notebook must show the regression process: model summary with
   p-values and t-statistics, R² and adjusted R², the features you kept and why, and your RMSE.
5. Be respectful and help each other in the Discussion tab, but don't share full solutions before the deadline.

---

## Grading (optional; for the host)

| Part | Weight |
|---|---|
| Regression process shown (summary, p-values, t-statistics, R², adjusted R²) | 40% |
| Feature choices explained | 20% |
| RMSE check and correct train/test workflow | 20% |
| Leaderboard score (private) | 20% |

---

## Kaggle settings checklist (host)
- Competition type: **Community**
- Visibility: **private, join by invitation link**
- Metric: **Root Mean Squared Error (RMSE)**
- Solution file: `solution.csv` (columns `id`, `price_per_area`, `Usage`)
- Sample submission: `sample_submission.csv`
- Data files for participants: `train.csv`, `test.csv`, `sample_submission.csv` (**never** `solution.csv`)
- Max daily submissions: **5**; final submissions selected: **2**; max team size: **1**
- Deadline: **December 2, 2026, 11:59 PM UTC**
