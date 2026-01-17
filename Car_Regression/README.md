# 🚗 Car Price Prediction (End-to-End Machine Learning Project)

This project is an **end-to-end Machine Learning regression pipeline** for predicting car selling prices based on vehicle features.  
It covers the complete workflow starting from raw data to a fully trained and saved production-ready pipeline.

---

## 📌 Project Overview

The goal of this project is to predict the **selling price of cars** using historical car data and machine learning models.  
The project demonstrates best practices in:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model comparison and selection
- Pipeline building
- Cross-validation
- Model persistence

---

## 🧠 Workflow Steps

1. Import libraries  
2. Load data and perform a quick inspection  
3. Data cleaning:
   - Remove duplicates  
   - Handle null values  
   - Treat outliers using IQR  
   - Fix column types  
4. Save cleaned dataset  
5. Exploratory Data Analysis (EDA)  
6. Data preprocessing (scaling & encoding)  
7. Build preprocessing pipelines  
8. Train and compare multiple models  
9. Create a full pipeline and save it  

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas & NumPy**
- **Matplotlib & Seaborn**
- **Scikit-learn**
- **XGBoost**
- **Joblib**

---

## 📊 Exploratory Data Analysis (EDA)

Key analysis performed:
- Distribution of selling prices
- Price trends across manufacturing years
- Transmission type distribution
- Average selling price by brand
- Relationship between mileage, year, and price

---

## 🧹 Data Preprocessing

- **Numerical features**
  - Standard Scaling
- **Categorical features**
  - One-Hot Encoding
- **Outlier treatment**
  - IQR-based clipping
- **Feature Engineering**
  - Extracted `brand` from car name

All preprocessing steps are handled using **Scikit-learn Pipelines**.

---

## 🤖 Models Trained

The following models were trained and evaluated:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- XGBoost Regressor  

### 📈 Model Performance (Test Set)

| Model | R² Score |
|------|----------|
| Linear Regression | 0.70 |
| Decision Tree | 0.53 |
| Random Forest | 0.72 |
| **XGBoost (Best)** | **0.73** |

---

## 🔁 Cross Validation Results (Best Model)

- **Mean R² Score:** 0.73  
- **Standard Deviation:** 0.03  

This indicates good generalization and stable performance.

---

## 🧩 Full Pipeline

The final pipeline includes:
- Data preprocessing (scaling + encoding)
- Best performing model (XGBoost)

The pipeline is saved using `joblib` and can be loaded directly for inference.

---

## 💾 Model Saving

```python
joblib.dump(full_pipeline, "Model/full_pipeline.pkl")

---

## 🚀 How to Run

Clone the repository

git clone https://github.com/YourUsername/Car-Price-Prediction.git


Install dependencies

pip install -r requirements.txt


Run the notebook or script to train the model and generate predictions

---

## 📌 Future Improvements

Hyperparameter tuning (GridSearch / RandomizedSearch)

Feature importance analysis

Model explainability (SHAP)

Deployment using Flask or FastAPI

---

👤 Author

Mohammed
Machine Learning & Data Science Enthusiast