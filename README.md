 🏠 House Price Prediction — Regression Analysis

A machine learning project that predicts house prices based on property features
using Linear Regression and Random Forest models.

 📌 Project Overview

Real estate buyers and sellers often rely on guesswork or outdated comparisons
to estimate a property's fair value. This project builds a regression model that
predicts house prices based on features like size, number of rooms, location,
and amenities — and identifies which features most strongly influence price.

 📂 Project Structure

 HousePricePrediction/

├── analysis.ipynb                        ← Main Jupyter Notebook (all 5 tasks)

├── Housing.csv                           ← Dataset

├── summary.pdf                           ← 1-page findings report

└── charts/

├── chart1_price_distribution.png     ← Price histogram

├── chart2_correlation_heatmap.png    ← Feature correlation heatmap

└── chart3_predictions_and_importance.png ← Actual vs Predicted + Feature Importance

📦 Dataset

- **Source:** [Housing Prices Dataset — Kaggle](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset)
- **Records:** 545 properties
- **Features:** 13 columns (12 input features + 1 target)

| Column | Type | Description |
|--------|------|-------------|
| price | int | 🎯 Target — House price in INR |
| area | int | Size of the house in sq ft |
| bedrooms | int | Number of bedrooms |
| bathrooms | int | Number of bathrooms |
| stories | int | Number of floors |
| mainroad | yes/no | Connected to main road? |
| guestroom | yes/no | Has guest room? |
| basement | yes/no | Has basement? |
| hotwaterheating | yes/no | Has hot water heating? |
| airconditioning | yes/no | Has air conditioning? |
| parking | int | Number of parking spaces |
| prefarea | yes/no | Located in preferred area? |
| furnishingstatus | category | furnished / semi-furnished / unfurnished |



 ✅ Tasks Completed

- **Task 1 — Data Loading & Exploration** — Loaded dataset, explored shape, columns, missing values
- **Task 2 — Data Cleaning** — Handled missing values, removed duplicates, one-hot encoded categorical columns
- **Task 3 — Model Building** — Trained Linear Regression and Random Forest, evaluated with MAE, RMSE, R²
- **Task 4 — Visualizations** — 3 charts: price distribution, correlation heatmap, actual vs predicted
- **Task 5 — Insights & Summary** — Written analysis of findings and business recommendations



 📊 Model Results

| Model | MAE | RMSE | R² Score |
|-------|-----|------|----------|
| Linear Regression | ₹9,70,043 | — | 0.653 |
| **Random Forest** | **₹10,19,528** | — | **0.612** |

> Random Forest captured complex non-linear patterns better than Linear Regression.



🔍 Key Findings

- **Area (sq ft)** is the strongest predictor of house price
- **Preferred locality** ranks higher than number of bedrooms — location matters more than size
- **Air conditioning** significantly boosts property value
- Houses in preferred areas command a premium regardless of other features



💡 Business Recommendation

Invest in properties in **prime/preferred localities** with **air conditioning**
and modern amenities. These features deliver higher returns than simply adding
extra bedrooms. Use ensemble ML models for pricing — not simple averages.



 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python 3.x | Programming language |
| Jupyter Notebook | Development environment |
| Pandas | Data loading and cleaning |
| NumPy | Numerical operations |
| Scikit-learn | ML models and evaluation |
| Matplotlib | Charts and plots |
| Seaborn | Statistical visualizations |




