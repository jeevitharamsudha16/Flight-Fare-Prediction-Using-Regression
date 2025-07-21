# ✈️ Flight Fare Price Prediction

This project predicts the prices of airline tickets using historical data. It involves data cleaning, feature engineering, model building, and performance evaluation using regression algorithms.

---

## 📌 Objective

Develop a machine learning regression model that can accurately predict flight fares based on multiple input features such as airline, journey date, source, destination, stops, and duration.

---

## 📂 Dataset

- 📥 **Source**: Kaggle (uploaded manually)
- 📄 **Format**: CSV
- 🎯 **Target Variable**: `Price`

### ✅ Features Used
- Airline  
- Date_of_Journey  
- Source and Destination  
- Route  
- Dep_Time and Arrival_Time  
- Duration  
- Total_Stops  
- Additional_Info

---

## 🧼 Data Preprocessing

- Converted date and time columns to datetime format
- Extracted day, month, hour, minute from relevant columns
- Processed `Duration` column into numeric hours and minutes
- Dropped irrelevant or duplicate columns
- Handled missing values
- Label encoded categorical variables

---

## 🛠️ Feature Engineering

- One-hot encoding of nominal variables
- Created new numerical features from time-based columns
- Dropped unnecessary columns like `Route`, `Additional_Info`

---

## 🤖 Model Building

- Used `ExtraTreesRegressor` to identify important features
- Applied **Random Forest Regressor** as the primary model
- Performed **Hyperparameter Tuning** using `RandomizedSearchCV`

---

## 📊 Model Evaluation

- ✅ R² Score: `0.80+` (based on the tuned model)
- Evaluated using:
  - R² Score
  - MAE (Mean Absolute Error)
  - MSE (Mean Squared Error)
  - RMSE (Root Mean Squared Error)
