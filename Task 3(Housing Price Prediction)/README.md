# 🏠 House Price Prediction

## 📌 Overview
This project predicts **median house prices** in California using the **California Housing Dataset**.  
We applied **Random Forest** and **XGBoost** models, compared their performance, and analyzed **feature importance** to understand which factors impact housing prices the most.

---

## 📂 Features Used
- Median Income  
- Latitude & Longitude  
- Population  
- Rooms per Household  

---

## ⚙️ Steps
1. Data preprocessing & cleaning  
2. Feature engineering (Rooms per Household, etc.)  
3. Train models:
   - **RandomForestRegressor**
   - **XGBoost Regressor**
4. Compare model performance  
5. Analyze **feature importance**  

---

## 📊 Results
- **Random Forest**
  - RMSE: ~0.47  
  - R² Score: ~0.83  

- **XGBoost**
  - RMSE: (slightly better than RF depending on tuning)  
  - R² Score: ~0.84  

👉 **XGBoost performed slightly better than Random Forest.**  
Feature importance analysis showed **Median Income** and **Geographical features (Latitude & Longitude)** are the most important predictors.

---

## 🚀 Future Work
- Perform hyperparameter tuning for better results  
- Try advanced models like LightGBM or CatBoost  
- Add external features (crime rates, school ratings, etc.)

---

## 🛠️ Tools
- Python  
- scikit-learn  
- XGBoost  
- pandas, matplotlib, seaborn
