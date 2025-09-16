# 🛒 Sales Forecasting using XGBoost  

This project demonstrates **time series sales forecasting** using **XGBoost** with lagged features.  
The model predicts future sales based on historical sales data and evaluates performance using **RMSE (Root Mean Squared Error)**.  

---

## 📂 Project Structure
├── train.csv # Input dataset containing Order Date & Sales
├── sales_forecast.py # Python script with the ML model
└── README.md # Project documentation



---

## 📊 Dataset
- **File:** `train.csv`  
- **Required Columns:**  
  - `Order Date` → Date of the order (format: `DD/MM/YYYY`)  
  - `Sales` → Sales amount for that date  

---

## ⚙️ Requirements
Install the required Python libraries before running the project:

```bash
pip install pandas matplotlib seaborn scikit-learn xgboost numpy


How It Works

Data Preprocessing

Reads sales data from train.csv

Converts Order Date into datetime format

Aggregates daily sales

Visualization

Plots sales trend over time using Matplotlib

Feature Engineering

Creates lag features (previous sales values as input features)

Model Training

Splits data into train and test sets (time-series split, no shuffle)

Trains an XGBoost Regressor with parameters:

n_estimators=100

learning_rate=0.1

max_depth=5

Evaluation

Predicts sales on test set

Calculates RMSE (Root Mean Squared Error)

Visualization of Predictions

Plots actual vs predicted sales


Results

Model performance is evaluated using RMSE (lower = better).

Example output:

RMSE: 245.37

Visualization:

🔴 Red line → Actual Sales

🟢 Green line → Predicted Sales

🖼️ Sample Plots

Sales Trend Over Time
Shows historical sales patterns.

Forecasting Results
Compares actual sales vs predicted sales.

(You can add generated plots here as images using ![Alt text](path/to/image.png) after saving them.)

🔮 Future Improvements

Use advanced time-series models (ARIMA, Prophet, LSTM)

Hyperparameter tuning with GridSearchCV

Add seasonality and holiday effects

Deploy model with Flask/Django API

Author

Ritesh Kashyap

📧 Email: pixelphhoenixproduction@gmail.com

🌐 GitHub: Riteshgraphic




