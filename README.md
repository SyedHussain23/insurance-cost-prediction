# 💰 insurance-cost-prediction

This project predicts **medical insurance charges** using machine learning and feature engineering on a healthcare dataset.

It demonstrates a complete **end-to-end regression pipeline**, including:

* Exploratory data analysis (EDA)
* Categorical encoding and feature engineering
* Target transformation
* Training multiple regression models
* Model evaluation and comparison
* Best model selection and prediction

The objective is to predict **insurance charges** using demographic and health attributes.

---

## 📌 Project Overview

* **Problem Type:** Regression
* **Domain:** Healthcare / Insurance Analytics
* **Dataset Size:** 1338 records, 7 features
* **Target Variable:** charges
* **Best Model:** LightGBM Regressor

---

## 📊 Dataset

Features used:

* age → age of beneficiary
* sex → gender
* bmi → body mass index
* children → number of dependents
* smoker → smoking status
* region → residential area
* charges → medical insurance cost (target)

---

## 🔍 Exploratory Data Analysis

Key findings:

* No missing values in dataset
* Target variable highly right-skewed
* Smoking strongly increases insurance cost
* Age and BMI positively correlate with charges
* Balanced categorical distributions except smoker

---

## 🔧 Data Preprocessing

* One-hot encoding of categorical features
* Log transformation of target variable (charges_log)
* Train-test split (80-20)
* Feature normalization via transformation

---

## ⚙️ Feature Engineering

New features created:

* **bmi_smoker_interaction** → captures smoker impact on BMI cost
* **charges_log** → reduces skewness in target variable
* **age_squared** → captures non-linear age relationship

---

## 🧠 Models Trained

* Linear Regression
* Ridge
* Lasso
* Elastic Net
* Decision Tree
* Random Forest
* LightGBM
* XGBoost
* Support Vector Regressor

---

## 📈 Model Evaluation

Metrics used:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* R² score

### 🏆 Best Model

**LightGBM Regressor**

* Highest R² ≈ 0.8457
* Lowest MSE
* Strong ability to capture non-linear relationships

---

## 🚀 Prediction

The best model is used to generate predictions on unseen data after log transformation of the target.

---

## ⚠️ Challenges & Solutions

* Skewed target → log transformation
* Feature interaction complexity → engineered interaction feature
* Model selection → multi-model comparison
* Overfitting risk → train-test split

---

## 💡 Business Insights

* Smokers incur significantly higher insurance costs
* Higher BMI increases risk and cost
* Older individuals generally pay higher premiums
* BMI + smoking interaction is a major cost driver

---

## 🚀 How to Run

```bash
git clone https://github.com/SyedHussain23/insurance-cost-prediction
cd insurance-cost-prediction
pip install -r requirements.txt
jupyter notebook insurance-cost-prediction.ipynb
```

---

## 👨‍💻 Author

**Syed Hussain Abdul Hakeem**

* GitHub: [https://github.com/SyedHussain23](https://github.com/SyedHussain23)
* LinkedIn: [https://www.linkedin.com/in/syed-hussain-abdul-hakeem](https://www.linkedin.com/in/syed-hussain-abdul-hakeem)

---

## ⭐ Support

If you found this project useful, give it a ⭐.
