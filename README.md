# ⚽ Football Player Market Value Prediction (Jupyter Notebook)

This Jupyter Notebook project explores the prediction of football players' market values using a full pipeline from data scraping and cleaning to advanced machine learning and neural network modeling.

---

## 📁 Table of Contents

- [Overview](#overview)
- [Data Sources](#data-sources)
- [Notebook Workflow](#notebook-workflow)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling Approaches](#modeling-approaches)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

---

## ✅ Overview

The notebook performs:

- Web scraping of player market values
- Cleaning and merging with performance stats
- Feature engineering (per-90 stats, transformations)
- Visualization of performance and market value trends
- Modeling using:
  - XGBoost Regressor
  - Neural Networks (TensorFlow/Keras)
- Cross-validation and model evaluation

---

## 📊 Data Sources

- `Player_Stats.csv`: Player performance data
- `player_market_values.csv`: Scraped values from [Transfermarkt](https://www.transfermarkt.com)

---

## 🔁 Notebook Workflow

1. **Data Preprocessing**

   - Clean market value format (e.g., €1.5m → 1,500,000)
   - Normalize and aggregate player stats
   - Merge datasets on player names

2. **Feature Engineering**

   - Create per-90-minute metrics
   - Derive features like `Goal_Contrib_per_90`, `Age_squared`

3. **Exploratory Analysis**

   - Distribution plots, bar charts, scatter plots
   - Correlation matrices and heatmaps
   - Top performers visualizations

4. **Modeling**

   - Baseline model using average value by position
   - XGBoost with K-Fold CV and GridSearchCV
   - Neural Networks with dropout, early stopping, tuning

5. **Evaluation**
   - R², MAE, and MSE for each model
   - Actual vs Predicted plots
   - Feature importance charts

---

## 📉 Exploratory Data Analysis

The notebook includes rich visualizations:

- Pairplots & boxplots
- Heatmaps of correlation
- Market value analysis by age, position, and nation
- Feature correlation with market value
- Top 10 rankings (market value, goals, assists, minutes)

---

## 🤖 Modeling Approaches

| Model                  | R² (Test) | MAE | MSE |
| ---------------------- | --------- | --- | --- |
| Baseline               |           |     |     |
| XGBoost (Tuned)        |           |     |     |
| Neural Network (Tuned) |           |     |     |

> _Model results are printed in the notebook after each evaluation step._

---

## 🛠️ Installation

To run this notebook, install the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow beautifulsoup4 requests
```
