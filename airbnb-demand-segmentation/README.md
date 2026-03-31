# 🏡 Airbnb Market Segmentation & Demand Prediction (California)

**Python · Pandas · Scikit-learn · XGBoost · Clustering**

---

## 📌 Project Overview

This project explores whether **clustering-based market segmentation** can improve the prediction of Airbnb listing demand across California.

Using a dataset of **81K+ listings**, we analyzed pricing, host behavior, and property characteristics to understand:
- What drives Airbnb demand  
- How listings differ across market segments  
- Whether segmentation improves predictive performance  

---

## 🎯 Objectives

- Identify key drivers of Airbnb listing demand  
- Compare machine learning models for prediction accuracy  
- Segment listings into meaningful market groups  
- Evaluate whether segmentation improves model performance  

---

## 📊 Dataset

- Source: Inside Airbnb (California markets)  
- Size: 81,000+ listings  
- Features include:
  - Price, availability, reviews  
  - Property type, bedrooms, bathrooms  
  - Host activity and listing behavior  

---

## 🧹 Data Processing

- Merged multiple regional datasets into one unified dataset  
- Cleaned and standardized pricing data  
- Handled missing values (KNN imputation)  
- Removed extreme outliers (top 1% pricing)  
- Created additional features for modeling  

---

## 🤖 Modeling

We compared three regression models:

- Linear Regression  
- Random Forest  
- XGBoost  

### 📈 Results

| Model            | R²     | RMSE  | MAE   |
|------------------|--------|-------|-------|
| Linear Regression| 0.27   | 1.45  | 0.91  |
| Random Forest    | 0.52   | 1.18  | 0.59  |
| XGBoost          | **0.54** | **1.15** | **0.58** |

👉 XGBoost performed best, capturing non-linear relationships in the data.

---

## 🧩 Clustering (Market Segmentation)

We applied **K-Means clustering (k=3)** to segment listings:

- 🟢 **Mainstream Listings (60%)**  
  - Lower price, high ratings  

- 💎 **Luxury Listings (17%)**  
  - High price, larger capacity  

- 🏢 **Commercial Hosts (23%)**  
  - Multiple listings, different behavior patterns  

---

## 🔍 Key Findings

- Airbnb demand is **non-linear** → tree-based models perform better  
- Market is **highly heterogeneous** across segments  
- **Global model outperformed segmented models**  
- Clustering is useful for **insight generation**, not necessarily prediction improvement  

---

## 🚀 Conclusion

While segmentation provides valuable insights into market structure, it does not improve predictive accuracy. A **global model remains more effective** for demand forecasting, while clustering helps inform **strategic and business decisions**.

---

## 📂 Project Structure

