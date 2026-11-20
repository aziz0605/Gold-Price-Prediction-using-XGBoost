# Gold Price Prediction Using XGBoost

## Project Overview

This project focuses on predicting gold price returns using the XGBoost Regression algorithm. Historical gold price data is used to build a machine learning model that learns patterns from previous price movements and predicts returns.

The project uses Python, Pandas, NumPy, Matplotlib, and Scikit-learn for data processing, feature engineering, model training, evaluation, and visualization.

## Dataset Information

- **Dataset:** Gold Price Historical Dataset
- **Total Records:** 8,000 rows
- **Features Available:** Date, Open, High, Low, Close, Volume
- **Selected Column:** Close

The project uses the historical closing price to calculate returns and create additional features.

**Note:** The Excel dataset (`Gold_Price_Prediction_8000_Rows.xlsx`) is required to run the notebook. Make sure the dataset is available in the correct file path.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook

## Project Workflow

1. Import Required Libraries
2. Load Dataset
3. Data Inspection
4. Select Close Price Column
5. Feature Engineering
6. Remove Missing Values
7. Define Features (X) and Target (y)
8. Split Dataset into Training and Testing Sets
9. Create XGBoost Regression Model
10. Train the Model
11. Make Predictions
12. Model Evaluation
13. Actual vs Predicted Visualization

## Feature Engineering

The following features are created from historical closing prices:

| Feature | Description |
|---|---|
| Returns | Percentage change in closing price |
| Lag_1 | Previous day's return |
| Lag_2 | Two days previous return |
| SMA_7 | 7-day Simple Moving Average ratio |
| Volatility | 7-day rolling standard deviation of returns |

## Model Used

**XGBoost Regressor**

The XGBoost Regressor algorithm is used to train the model and predict gold price returns.

Model Parameters:

- n_estimators = 100
- learning_rate = 0.03
- max_depth = 4
- subsample = 0.8
- colsample_bytree = 0.8
- random_state = 42

## Model Evaluation

The model is evaluated using the following regression metrics:

| Metric | Result |
|---|---:|
| R² Score | 0.6237 |
| MSE | 0.000003 |
| MAE | 0.0014 |

These results represent the output obtained from the current notebook execution.

## Visualization

The project includes an Actual vs Predicted visualization to compare the actual gold price returns with the model's predicted returns.
<img width="1039" height="547" alt="image" src="https://github.com/user-attachments/assets/fe3c63da-62dd-4a14-8fa0-00be64542901" />


## Installation

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn xgboost openpyxl
```

## How to Run

1. Clone this repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

2. Open the project folder.

3. Make sure the Excel dataset is available.

4. Open the Jupyter Notebook:

```bash
jupyter notebook
```

5. Run the notebook cells sequentially.

**Note:** Update the dataset file path in the notebook according to your system if required.

## Project Objective

The main objective of this project is to apply machine learning techniques to historical gold price data and predict gold price returns using the XGBoost Regression algorithm.

## Author

A. ABDUL AZIZ
