# 🌍 Carbon Emissions Prediction Using Machine Learning

## 👤 Student Details
- **Name:** Abhishek Kanade
- **Student AICTE ID:** STU682d9fec69f801747820524

---

## 📌 Project Overview
This project predicts **CO₂ emissions per capita** for different countries using historical economic, demographic, and environmental indicators. The goal is to help **policymakers** anticipate future emissions trends and implement effective measures to combat **climate change**.

---

## 🎯 Learning Objectives
- Apply **machine learning** for time-series based forecasting.
- Use **feature selection (RFECV)** to improve model efficiency.
- Perform **hyperparameter tuning** using `RandomizedSearchCV`.
- Visualize data trends and forecast results for interpretability.
- Develop insights into **CO₂ emission drivers** like urbanization, energy use, and land protection.

---

## 🛠️ Tools & Technologies
- Python, Pandas, NumPy
- Scikit-learn (Random Forest, Feature Selection, Grid Search)
- Matplotlib & Seaborn for visualization
- Joblib for model serialization
- Stramlit

---

## 🔍 Problem Statement
Forecasting country-wise CO₂ emissions based on past trends can aid in **early identification** of environmental risks. This helps governments **design policies** to minimize the harmful effects of emissions like **global warming**, and prepare for future **abnormalities** in emissions levels.

---

## ✅ Solution
A **Random Forest Regressor** model was trained using historical development indicators (e.g., energy consumption, population growth, urbanization, cereal yield). After careful **feature selection** and **hyperparameter optimization**, the model forecasts CO₂ emissions from **2010 to 2030**. These forecasts can guide policy decisions to mitigate environmental impact.

---

## 📈 Methodology
1. **Data Preprocessing**: Cleaned, filtered (e.g. removed outliers like ARE), and selected relevant features.
2. **Feature Selection**: Applied `RFECV` with cross-validation to identify top predictors.
3. **Model Training**: Used `RandomForestRegressor` with `RandomizedSearchCV` for best hyperparameters.
4. **Model Evaluation**:
   - 10-fold Cross-validation on training set.
   - R² Score: **0.986**
   - RMSE & MSE analyzed on test set.
5. **Forecasting**:
   - Used **CAGR** to project features.
   - Predicted CO₂ emissions per year till 2030.

---

## 📊 Results & Visualizations

- **R² Score on Test Set**: 0.986
- **CAGR Analysis**: Projected yearly growth of selected features (1991–2008).
- **Forecasts**: CO₂ emissions per country for 2010–2030.
- **Regression Plot**: Predicted vs Actual emissions.
- **Line Chart**: Forecasted trends per country.



---
## 📲 Live Application

Explore the live app for real-time country-wise forecasts:

🔗 [**Launch the App**](https://projects-fuufzehbnggmzltaari9hj.streamlit.app)

---

## 💾 Model Saving
The trained model was saved using `joblib`:
```python
joblib.dump(rf_best_model, 'forecasting_co2_emmision.pkl')


