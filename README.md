Agricultural Yield Prediction using Machine Learning
Project Overview
This project aims to predict crop yield (MT per HA) using machine learning models. The goal is to develop a reliable model that helps optimize agricultural productivity based on various environmental and economic factors.

Dataset
The dataset includes features such as:
Precipitation
Temperature anomalies
Economic impact
Adaptation strategies
Soil conditions
The target variable is Crop_Yield_MT_per_HA.
Models Used
We tested multiple models to find the best-performing one:

Model	R² Score	Mean Squared Error (MSE)
Random Forest	0.31	-
XGBoost	0.29	-
LightGBM	0.614	0.407
Steps Followed
1️⃣ Data Preprocessing
✔ Checked for missing values and outliers.
✔ Applied feature encoding for categorical variables (e.g., Adaptation_Strategies).
✔ Performed feature scaling where necessary.

2️⃣ Model Selection & Training
✔ Initially trained Random Forest and XGBoost, but results were not satisfactory.
✔ Switched to LightGBM, which significantly improved performance.

3️⃣ Model Evaluation
The model was evaluated using Mean Squared Error (MSE) and R² score:

LightGBM Performance:
✅ MSE = 0.407 (Lower is better)
✅ R² = 0.614 (Higher is better)
Next Steps & Improvements
✔ Fine-tuning LightGBM hyperparameters (num_leaves, learning_rate, etc.).
✔ Using Stacking or Blending with multiple models to further improve predictions.
✔ Performing Feature Importance Analysis to refine the dataset.

