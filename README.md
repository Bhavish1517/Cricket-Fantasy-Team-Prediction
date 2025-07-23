# Cricket Fantasy Team Prediction

This project implements a machine learning pipeline to predict the top-performing players for future cricket matches, aimed at helping users optimize their fantasy cricket teams. The system uses historical match data to forecast individual player statistics and calculates fantasy points based on predicted and actual performances.

## What's Been Done

- **Data Preparation:**  
  Historical match datasets are processed for both batting and bowling performance. Features include match details (season, venue, teams, etc.), player stats (runs, wickets, economy, etc.), and outcomes.
  
- **Batting Predictions:**  
  - Gradient Boosting models are trained to predict total runs, fours, sixes, and balls faced for each batsman.
  - A custom points system is implemented to convert predicted/actual batting stats into fantasy points, considering factors like scoring rate, ducks, and milestones.
  - Output includes DataFrames storing predicted and actual player stats per match.

- **Bowling Predictions:**  
  - Gradient Boosting models (regression/classification) are used to predict wickets and economy rates for bowlers.
  - Fantasy points are calculated based on predicted/actual bowling stats, factoring in wickets taken, economy rate, and other performance metrics.
  - Results are saved in DataFrames and exported as CSV files.

- **Combining Results and Ranking:**  
  - Predicted and actual batting/bowling points are combined for each player.
  - Players are sorted match-wise by their total predicted points to recommend top picks for fantasy teams.
  - Exported files include sorted lists of player predictions and actual results for validation and comparison.

- **Model Evaluation:**  
  - Mean Squared Error (MSE) and accuracy metrics are reported for model validation.
  - Performance is compared between predicted and actual results for each player and match.

## Workflow Steps

1. **Data Loading & Cleaning:** Load player and match datasets, preprocess features.
2. **Feature Engineering:** Extract relevant attributes for batting and bowling prediction.
3. **Model Training:** Train gradient boosting models for various player statistics.
4. **Prediction:** Generate match-wise predictions for all players.
5. **Fantasy Points Calculation:** Apply custom logic to convert predicted and actual stats to fantasy points.
6. **Ranking & Export:** Sort players by points, export recommendations for fantasy team selection.

## Future Work

- Expand feature set to include contextual factors (weather, player fitness, etc.)
- Integrate real-time data sources and automate prediction pipeline.
- Develop a web or mobile app interface for easier access to predictions.
- Experiment with ensemble models and deep learning approaches for improved accuracy.

## Publication

This work has been published. Do check it out here [https://dl.acm.org/doi/10.1145/3698062.3698091]

---

## 👥 Collaborators

**K Bhavish Raju**  
[![Bhavish](https://img.shields.io/badge/GitHub-Bhavish1517-blue?style=flat-square&logo=github)](https://github.com/Bhavish1517)

**M Govindarajan**  
[![Govind](https://img.shields.io/badge/GitHub-Govindarajannn1-green?style=flat-square&logo=github)](https://github.com/Govindarajannn)

**Kritin Thakur**  
[![Kritin](https://img.shields.io/badge/GitHub-Kritin_Thaur-yellow?style=flat-square&logo=github)](https://github.com/Kritin-Thakur)

**Ishan**  
[![Ishan](https://img.shields.io/badge/GitHub-IshankumarP-red?style=flat-square&logo=github)](https://github.com/IshankumarPr)
