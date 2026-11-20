# Supervised Learning Essentials

A 2-hour beginner lesson: understand core supervised learning models and build basic predictors in Python.

## What's in this repo

| Path | What it is |
|---|---|
| `slides/index.html` | The lesson slide deck (38 slides, with speaker notes) |
| `notebooks/supervised_learning_handson.ipynb` | Hands-on for section 7: classify breast cancer with 3 models, see overfitting |
| `notebooks/regression_basic.ipynb` | Regression lesson: train, keep significant features (p-values), measure RMSE |
| `notebooks/real_estate_starter.ipynb` | Starter notebook for the Kaggle real-estate competition |
| `competition/competition_text.md` | Competition description, evaluation, data and rules text |
| `competition/kaggle_competition_notes.md` | Similar Kaggle competitions for reference |

## Presenting the slides

1. Download the repo (**Code → Download ZIP**) or clone it.
2. Double-click `slides/index.html` to open it in a browser (needs an internet connection for the slide library and fonts).
3. Keys: **→ / ←** move between slides · **S** opens the speaker view with notes and a timer · **F** full screen · **Esc** slide overview.

## Running the notebooks

Open [Google Colab](https://colab.research.google.com) → **File → Upload notebook** → pick a notebook → **Runtime → Run all**.
All datasets load inside the notebooks; nothing to download.

## Lesson outline (2 hours)

| Time | Section |
|---|---|
| 0:00 | 1. What is supervised learning? + self-check |
| 0:12 | 2. Regression vs. classification + self-check |
| 0:22 | 3. The workflow + self-check |
| 0:33 | 4. Core models + self-check |
| 0:50 | 5. Measuring success + self-check |
| 1:07 | Break |
| 1:12 | 6. Overfitting vs. underfitting + self-check |
| 1:25 | 7. Hands-on in Colab |
| 1:50 | 8. Discussion |
| 1:55 | 9. Exit quiz |

## Data sources

- Breast Cancer Wisconsin (Diagnostic) dataset, via scikit-learn's `load_breast_cancer`.
- Diabetes dataset, via scikit-learn's `load_diabetes`.
- Real-estate competition: Yeh, I. (2018). Real Estate Valuation [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5J30W (CC BY 4.0).

> The competition's hidden answers (`solution.csv`) and the file builder are intentionally **not** in this repo.
