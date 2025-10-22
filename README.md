Medical Insurance Cost Prediction using Linear Regression

This project builds a Machine Learning model using Linear Regression to predict medical insurance charges based on factors like age, BMI, smoking habits, and region. The dataset contains real-world health and cost records and is ideal for practicing regression concepts and model diagnostics.

🔧 Problem Statement

Insurance companies calculate premiums based on risk. People who smoke, are older, or have higher BMI pay more.
Goal: Predict the medical insurance charges based on personal profile data.

📊 Dataset Overview
Column Name	Description	Type
age	Age of the person	Numerical
sex	Male / Female	Categorical
bmi	Body Mass Index (weight/height²)	Numerical
children	Number of dependents	Numerical
smoker	Yes / No	Categorical
region	Residential area in US	Categorical
charges	Medical insurance cost	Target
✅ Project Workflow
1. Load Data
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing
   - Handle skewness with Log Transformation
   - Encode categorical variables
   - Feature scaling
4. Train-Test Split
5. Model Training (Linear Regression)
6. Evaluation (MAE, RMSE, R² Score)
7. Residual Diagnostics
8. Insights & Next Steps

🔎 Key Insights

smoker is the strongest predictor of insurance cost.

age and bmi also show a strong positive relationship with charges.

The original charges column was positively skewed, so we applied log transformation to improve prediction.

The model works well as a baseline, but residuals show heteroscedasticity, meaning non-linear models may perform better.

🧠 Technologies Used

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

📈 Model Performance
Metric	Value (approx)
MAE	~2600
RMSE	~4500
R²	~0.79

✅ Model explains 79% of the variance, but can be improved using feature interactions or non-linear models like Random Forest or Gradient Boosting.

🚀 Next Steps

Add interaction terms (e.g., age * smoker)

Train advanced models (Random Forest, XGBoost)

Hyperparameter tuning

Deploy using Streamlit or Flask
