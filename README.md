# Property Price Prediction using Machine Learning
This project is focused on predicting real estate property prices using machine learning techniques. The primary objective was to clean and transform the raw housing data, build a predictive model using Linear Regression, and evaluate multiple algorithms to identify the best fit for the dataset.

## Data Cleaning & Preprocessing
The raw data required significant preprocessing to ensure quality and consistency. The following steps were performed:
✅ Handled missing or inconsistent values using techniques like mean imputation
🏷 Renamed and standardized column headers for clarity
🧽 Removed irrelevant or malformed rows from the dataset
📍 Reduced the number of unique locations by grouping rare/low-frequency entries
🚿 Removed unrealistic entries such as:
Properties with unusually high numbers of bathrooms ( more than 2 for each bedroom)
Entries with prices that clearly didn’t make sense (e.g., price per sq. ft. far outside the normal range)

## Model Evaluation & Tuning
To further evaluate model performance and explore alternatives, GridSearchCV was used to compare:

## Model	Description
Linear Regression	Baseline model using ordinary least squares
Lasso Regression	L1-regularized regression for feature selection
Decision Tree	Non-linear tree-based model for price prediction

Each model was evaluated with different hyperparameter settings using cross-validation. The best model was selected based on the highest cross-validation score.

## 🛠 Technologies Used
Python (pandas, numpy, sklearn, matplotlib)

Scikit-learn (LinearRegression, Lasso, DecisionTreeRegressor, GridSearchCV)

Jupyter Notebook

## 📊 Results
Final accuracy with Linear Regression: ~85%

GridSearchCV helped confirm that Linear Regression remained the best-performing model for this dataset, beating Lasso and Decision Tree under the tested conditions.
