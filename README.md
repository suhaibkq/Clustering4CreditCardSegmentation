# 🚗 Cars4U: Used Car Price Prediction

## 📌 Problem Statement

Cars4U is a budding tech start-up aiming to find a foothold in the fast-growing Indian used car market. The pre-owned car segment has surpassed the new car market in volume. In this project, the goal is to use machine learning to build a predictive model that estimates the resale price of used cars.

## 🎯 Objective

Develop a regression model that predicts the selling price of used cars based on historical data of car features and sales. The project explores data preprocessing, feature engineering, model training, and evaluation to build an accurate price prediction tool.

## 📊 Dataset

- **File**: `used_cars_data.csv`
- **Target Variable**: `Selling_Price` — the price the owner expects to sell the car for.
- **Features Include**:
  - `Year` — year of manufacture
  - `Present_Price` — current ex-showroom price
  - `Kms_Driven` — distance driven in kilometers
  - `Fuel_Type`, `Seller_Type`, `Transmission`, `Owner`
  - Additional engineered features: `Car_Age`, etc.

## 🧪 Project Workflow

1. **Data Cleaning & Feature Engineering**
   - Derived `Car_Age` from `Year`
   - Removed irrelevant features such as `Car_Name`
   - Converted categorical variables using One-Hot Encoding
   - Handled outliers and missing values

2. **Exploratory Data Analysis (EDA)**
   - Visualized distribution of prices, age, and driven kilometers
   - Used heatmaps and pairplots to explore feature correlation

3. **Model Building**
   - Models used:
     - Linear Regression
     - Decision Tree Regressor
     - Random Forest Regressor
   - Performance evaluated using:
     - R² Score
     - Mean Absolute Error (MAE)
     - Root Mean Squared Error (RMSE)

4. **Model Tuning & Evaluation**
   - Cross-validation with GridSearchCV for optimal hyperparameters
   - Feature importance analysis from Random Forest

## 🏆 Results

- **Best Model**: Random Forest Regressor
- **Top Predictive Features**:
  - `Present_Price`, `Car_Age`, `Kms_Driven`, `Fuel_Type_Diesel`
- **Key Insight**:
  - Newer cars with higher showroom price and lower mileage tend to have better resale value.

## 📁 Project Structure

├── ML_MLS1_Cars4u.ipynb # Main notebook with analysis and model training
├── used_cars_data.csv # Dataset used for training and evaluation
├── README.md # Project documentation


## 🔍 Takeaways

- Feature engineering plays a crucial role in model performance
- Ensemble methods like Random Forest provide strong baseline results for tabular data
- EDA reveals important business insights, like diesel cars having higher resale value

## 🚀 Future Work

- Deploy the model via Streamlit or Flask for real-time prediction
- Integrate external data such as location and service history
- Add image-based condition assessments for more accurate valuation

## 👨‍💻 Author

**Suhaib Khalid**  
Machine Learning Enthusiast
