# ⚽ FIFA22 Player Stats — Exploratory Data Analysis & Missing Value Prediction

This repository explores, cleans, and enhances the **FIFA22 player dataset** obtained from [Kaggle - FIFA 22 Player Stats Database](https://www.kaggle.com/datasets/bryanb/fifa-player-stats-database/data?select=FIFA22_official_data.csv).  
It performs **exploratory data analysis (EDA)** and uses **machine learning models** (Random Forest Regressors) to predict missing values for *Work Rate* and *Player Stats*.

---

## 📁 Project Structure

├── fifa22_eda.ipynb 					          # Data cleaning & exploratory data analysis
├── work rate pred.ipynb 				        # Predicts missing 'Work Rate' using Random Forest
├── missing stat pred.ipynb 			      # Predicts missing player stats using Random Forest
├── fifa22_official_data.csv 			      # Original dataset from Kaggle
├── fifa22_cleaned.csv 					        # Cleaned dataset after preprocessing
├── fifa22_cleaned_with_workrate.csv	  # After predicting missing 'Work Rate'
├── fifa22_null_removed.csv 			      # Final dataset with missing stats filled
└── README.md                           # Project documentation


---

## 🎯 Objective

1. **Clean & Prepare Data** — Handle duplicates, nulls, inconsistent data types, and feature engineering.
2. **Perform EDA** — Visualize player distribution, performance metrics, and correlations.
3. **Predict Missing Work Rates** — Use a Random Forest model to impute missing *Work Rate* values.
4. **Predict Missing Player Stats** — Train another Random Forest model to fill missing numerical attributes.

---

## 🧩 Files Overview

### 1️⃣ `fifa22_eda.ipynb`
- Loads the original **`fifa22_official_data.csv`** and later **`fifa22_null_removed.csv`**
- Performs:
  - Data cleaning (handling nulls, fixing data types, removing irrelevant columns)
  - Feature engineering
  - Exploratory analysis:
    - Distribution plots for key attributes
    - Correlation heatmaps
    - Extracts insights from the dataset
- Saves intermediate outputs:
  - `fifa22_cleaned.csv`

---

### 2️⃣ `work rate pred.ipynb`
- Loads `fifa22_cleaned.csv`
- Identifies missing *Work Rate* values
- Trains a **Random Forest Regressor** model on players with complete data
- Predicts and fills missing work rate values
- Exports dataset as:
  - `fifa22_cleaned_with_workrate.csv`

---

### 3️⃣ `missing stat pred.ipynb`
- Loads `fifa22_cleaned_with_workrate.csv`
- Detects missing numerical attributes (e.g., dribbling, passing, defending)
- Trains a **Random Forest Regressor** for each stat
- Predicts and fills missing stats
- Outputs final dataset:
  - `fifa22_null_removed.csv`

---

## ⚙️ Tools & Libraries

- **Python 3.10+**
- **Jupyter Notebook**
- **Libraries:**
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

---

## 📊 Key Insights
  - see deployment or notebook for insights
