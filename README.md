# video-game-revenue-prediction-
CatBoost + Optuna based ML model to predict video game revenue (RMSLE metric) for the ML.ai Hackathon 2026 on Kaggle. Includes EDA, feature engineering, OOF target encoding, and hyperparameter tuning. Achieved Rank 19 with score 0.70382
.

##  About the Hackathon

This project was built for the **ML.ai Hackathon 2026**, hosted on Kaggle. The challenge was to predict the **estimated revenue of video games** based on various features such as publisher information, genre, platform, and other game-related metadata.

The competition was evaluated using **RMSLE (Root Mean Squared Logarithmic Error)** as the scoring metric, which penalizes underestimation and overestimation errors on a logarithmic scale — making it well-suited for revenue/price prediction tasks where values can span several orders of magnitude.

## Problem Statement

Given a dataset of video games with associated features (genre, platform, publisher, release details, etc.), the goal was to build a regression model that accurately predicts each game's **estimated revenue**.

## Results

| Metric | Value |
|--------|-------|
| **Leaderboard Rank** | 19 |
| **Best Score (RMSLE)** | 0.70382 |
| **Model Used** | CatBoost with Optuna Hyperparameter Tuning |

##  Approach

1. **Exploratory Data Analysis (EDA)**
   - Analyzed the target variable (Estimated Revenue) distribution
   - Studied feature relationships and identified key predictors

2. **Feature Engineering**
   - Applied **Out-of-Fold (OOF) Target Encoding** for categorical variables to prevent data leakage while capturing target-related signal

3. **Model Building**
   - Used **CatBoost**, a gradient boosting algorithm well-suited for datasets with categorical features
   - Tuned hyperparameters using **Optuna**, an automated hyperparameter optimization framework, to minimize RMSLE

4. **Validation**
   - Used cross-validation to ensure the model generalizes well and avoids overfitting

##  Repository Structure
##  How to Run

1. Clone this repository
2. Open the notebook on Kaggle or Jupyter
3. Ensure the competition dataset is available in the expected input path
4. Run all cells sequentially to reproduce the pipeline (EDA → Feature Engineering → Model Training → Prediction)

##  Tech Stack

- **Python**
- **Pandas, NumPy** – Data manipulation
- **CatBoost** – Gradient boosting model
- **Optuna** – Hyperparameter tuning
- **Matplotlib/Seaborn** – Visualization

##  Future Improvements

- Ensemble with other boosting models (XGBoost, LightGBM)
- Feature selection to reduce noise
- Try stacking/blending for improved RMSLE

## Author

**Naman Khorwal**
B.Tech, Bioscience & Bioengineering (BSBE), IIT Guwahati

-  Kaggle: [namankhorwal](https://www.kaggle.com/namankhorwal)
-  LinkedIn: [Naman Khorwal](https://www.linkedin.com/in/naman-khorwal-561b0a374/)
