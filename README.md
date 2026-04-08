# Egypt-Crop-Yield-Prediction-99.17-XGBoost-
# 🌾 Egypt Crop Yield Prediction (1990-2024)

<p align="center">
  <img src="https://img.shields.io/badge/Accuracy-99.2%25-brightgreen?style=for-the-badge">
  <img src="https://img.shields.io/badge/Model-XGBoost-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Data-FAOSTAT-orange?style=for-the-badge">
</p>

---

## 🎯 Overview
This project provides a data-driven analysis and prediction of agricultural crop yields in Egypt over a **34-year period (1990-2024)**. By merging geographical knowledge with advanced Machine Learning techniques, I developed a model capable of forecasting yields with high precision.

> **Key Achievement:** Reached a **99.2% R² Score** using the XGBoost Regressor.
"The model was validated using 10-Fold Cross-Validation with shuffling, achieving a consistent mean R2 score of 99.12%, ensuring its reliability across different data samples."

## 📊 The Dataset
The data is sourced from the **Food and Agriculture Organization (FAOSTAT)**. 
- **Raw Data:** Comprehensive records of Egyptian agriculture.
- **Processing:** Data was cleaned, and features were engineered using **Pivot Tables** to align 'Area Harvested', 'Production', and 'Yield' for each crop type per year.

## 🛠️ Tech Stack & Tools
- **Language:** Python 🐍
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost.
- **Visualization:** Matplotlib, Seaborn.
- **Environment:** Kaggle Notebooks.

## 🚀 Project Workflow
1. **Data Cleaning:** Handling missing values and filtering for Egypt-specific records.
2. **Feature Engineering:** Reshaping data from long-form to wide-form (Pivoting).
3. **Model Selection:** Comparing different regressors (Random Forest vs. XGBoost).
4. **Hyperparameter Tuning:** Optimizing XGBoost for maximum accuracy.
5. **Serialization:** Saving the final model and encoders using `joblib` for deployment.

## 📂 Repository Structure
- `final_crop_model.pkl`: The trained XGBoost model.
- `crop_encoder.pkl`: Label encoder for crop types.
- `egypt_crop_yield_processed_pivot.csv`: The cleaned dataset used for training.

## 💻 Usage
To use the model in your environment:
```python
import joblib
import pandas as pd


# Load model and encoder
model = joblib.load('final_crop_model.pkl')
encoder = joblib.load('crop_encoder.pkl')


👤 Author
Sayed
AI Engineering Path | Machine Learning & Deep Learning Practitioner

"A Law graduate (Ain Shams University) pivoting into the world of Artificial Intelligence. I leverage my analytical background to build robust Machine Learning solutions, focusing on high-performance models and scalable AI architectures."
