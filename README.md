# Rossman Sales Prediction
This project builds a predictive model to forecast sales for 1,115 Rossmann stores across Germany. The model helps with inventory planning and revenue forecasting by analyzing historical sales data, store information, and promotional activities.

# Pipeline
* Data Loading 
* Feature Engineering
* Data Cleaning - Remove closed stores, handle missing values, validate data quality
* Data Visualization - Plot daily sales trends over time to understand patterns
* Feature Encoding - Label encode StateHoliday, one-hot encode StoreType and Assortment
* Train-Validation Split - Time-based split with last 6 weeks as validation set
* Hyperparameter Tuning - Optimize 9 parameters using Optuna
* Model Training - Train XGBoost regressor with optimized parameters
* Model Evaluation - Calculate RMSE, MAE, R², MAPE on validation set
* Prediction - Generate predictions for test set and export to CSV

#Key Results
* 32% reduction in RMSE compared to baseline model
* 39% reduction in MAPE through hyperparameter optimization
* R² Score: 0.94 on validation set

## How to Run
1. Clone the repo
```
git clone https://github.com/keerv13/rossmann-sales-prediction.git
```
2. Create and activate python virtual environemnt
```
python -m venv venv
venv\Scripts\activate
```
3. Install python dependencies
```
pip install -r requirements.txt
```
4. Run the notebook ``` rossmann_sales.ipynb ```
