# ml-electricity-forecast

⚡ Electricity Demand Forecasting with Machine Learning
This project uses historical electricity demand data to forecast future demand using machine learning techniques. It applies time series feature engineering, lag variables, and a Random Forest Regressor to build a predictive model. The goal is to support better planning and grid management by accurately anticipating electricity consumption patterns.

📊 Project Overview
Dataset: National electricity demand dataset (continuous dataset.csv)

Forecast Target: nat_demand (national electricity demand)

Approach: Supervised machine learning with time-series-aware train/test split

Model: Random Forest Regressor

Tools: Python, Pandas, Scikit-learn, Matplotlib, Seaborn

🧠 Machine Learning Workflow
Import Libraries & Load Data

Explore and Visualize Trends

Feature Engineering

Lag features (1h, 2h, 3h, 1d, 2d)

Time-based features (hour, weekday, month)

Categorical encoding (holiday, school)

Train-Test Split based on time (cutoff_date = 2017-01-01)

Model Training with RandomForestRegressor

Prediction and Evaluation

Metrics: MAE, RMSE, MAPE

Visualization of predicted vs actual demand

Feature Importance Analysis

📁 How to Use This Repository
🔧 Requirements
Python ≥ 3.8

Libraries:
pandas, numpy, matplotlib, seaborn, scikit-learn

pip install pandas numpy matplotlib seaborn scikit-learn
📥 Load the Data
Download or upload the dataset (continuous dataset.csv)

Make sure it includes a column named datetime in date-time format

Place it in your working directory or adjust the path in:

df = pd.read_csv('continuous dataset.csv', parse_dates=['datetime'])
📈 Sample Output
Forecast chart of electricity demand over time

Feature importance ranking

Model evaluation metrics (MAE, RMSE, MAPE)

✅ Results
The model achieved:
MAE: 19.88
RMSE: 31.47
MAPE: 1.70%

(Replace these with your actual values after training.)

🔍 Future Improvements
Try other models (XGBoost, LSTM)

Add weather or temperature data

Tune hyperparameters for improved accuracy

📌 License
This project is for educational and demonstration purposes.
