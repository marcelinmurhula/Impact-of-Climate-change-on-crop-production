
---

# **Agricultural Yield Prediction using Machine Learning**

## **Project Overview**
This project aims to predict **crop yield (MT per HA)** using machine learning models. The goal is to develop a reliable model that optimizes agricultural productivity based on various environmental and economic factors.

## **Dataset**
The dataset includes the following features:
- **Precipitation**
- **Temperature anomalies**
- **Economic impact**
- **Adaptation strategies**
- **Soil conditions**

**Target Variable:** `Crop_Yield_MT_per_HA`

## **Models Used & Performance**
We tested multiple models to find the best-performing one:

| Model          | R² Score | MSE  |
|---------------|---------|------|
| Random Forest | 0.31    | -    |
| XGBoost      | 0.29    | -    |
| **LightGBM** *(Best Model)* | **0.614** | **0.407** |

## **Steps Followed**
### **1️⃣ Data Preprocessing**
✔ Checked for missing values and outliers  
✔ Applied feature encoding for categorical variables *(e.g., Adaptation_Strategies)*  
✔ Performed feature scaling where necessary  

### **2️⃣ Model Selection & Training**
✔ Initially trained **Random Forest** and **XGBoost**, but results were unsatisfactory  
✔ Switched to **LightGBM**, which significantly improved performance  

### **3️⃣ Model Evaluation**
We used the following metrics to evaluate model performance:  
- **Mean Squared Error (MSE):** `0.407` *(Lower is better)*  
- **R² Score:** `0.614` *(Higher is better, indicating better predictive power)*  

## **Conclusion**
The **LightGBM model** demonstrated the best performance with an **R² score of 0.614** and **MSE of 0.407**. Future improvements may include hyperparameter tuning and incorporating additional relevant features.

---
