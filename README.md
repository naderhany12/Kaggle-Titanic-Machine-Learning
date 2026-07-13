# 🚢 Titanic - Machine Learning from Disaster (Kaggle)

This repository contains my structured workflow and solution for the famous **Titanic: Machine Learning from Disaster** competition on Kaggle. The goal is to predict which passengers survived the Titanic shipwreck using machine learning techniques.

---

## 📈 Current Project Status
* **Baseline Model:** Logistic Regression ~`81.11%` Validation Accuracy.
* **Current Best Model:** Random Forest (`max_depth=5`) with **`84.44%` Validation Accuracy** and a Kaggle Leaderboard score of **`0.77990`** (Top ~78%).
* **Next Steps:** Implementing advanced Feature Engineering (Title Extraction, Family Size, etc.) to cross the `80%+` mark on the Kaggle Leaderboard.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Jupyter Notebook / Kaggle Notebook
* **Libraries:** 
  * Data Manipulation: `pandas`, `numpy`
  * Machine Learning: `scikit-learn`, `xgboost`

---

## 🧠 Approach & Key Takeaways

1. **Exploratory Data Analysis (EDA) & Cleaning:**
   * Handled missing values for `Age` (Median Imputation) and `Embarked` (Mode Imputation).
   * Applied One-Hot Encoding for categorical features (`Sex`, `Embarked`).

2. **Model Exploration:**
   * **Logistic Regression:** Served as a solid starting baseline.
   * **XGBoost:** Achieved a high validation score (`85.56%`) but faced slight overfitting due to the small size of the Titanic dataset, yielding a Kaggle score of `0.77511`.
   * **Random Forest:** Current champion! Provided the most robust and stable generalization (`84.44%` Val / `0.77990` Kaggle).

3. **Feature Engineering (In Progress):**
   * Extracting passenger titles (`Mr`, `Mrs`, `Miss`, `Master`) from the `Name` column.
   * Creating a `FamilySize` feature by combining `SibSp` and `Parch` to capture family survival dynamics.

---

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/naderhany12/YOUR_REPO_NAME.git](https://github.com/naderhany12/YOUR_REPO_NAME.git)
