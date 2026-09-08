# Customer Churn Prediction

A Machine Learning project that predicts whether a customer is likely to leave a telecom service.

The project uses the Telco Customer Churn dataset and compares Logistic Regression and Random Forest classification models to identify customers at risk of churn.

---

## 📌 Project Overview

Customer churn is an important business problem for telecom companies because retaining existing customers is often more valuable than acquiring new ones.

This project analyzes customer information and builds Machine Learning models to predict customer churn.

The workflow includes:

- Data loading and inspection
- Data cleaning
- Exploratory Data Analysis (EDA)
- Categorical feature encoding
- Missing-value handling
- Train-test splitting
- Feature scaling
- Logistic Regression
- Random Forest
- Model evaluation
- ROC-AUC analysis
- Feature importance analysis
- Sample customer prediction

---

## 🎯 Objective

The main objectives of this project are:

1. Understand the factors associated with customer churn.
2. Prepare customer data for Machine Learning.
3. Build classification models to predict churn.
4. Compare different models using multiple evaluation metrics.
5. Select a suitable model for customer churn prediction.

---

## 📊 Dataset

The project uses the **Telco Customer Churn** dataset.

The dataset contains customer information related to:

- Demographics
- Customer account information
- Services used
- Contract information
- Payment methods
- Monthly charges
- Total charges
- Churn status

The target variable is:

**`Churn`**

- `Yes` → Customer churned
- `No` → Customer did not churn

The `customerID` column was removed because it is an identifier and does not provide useful predictive information.

---

## 🔍 Exploratory Data Analysis

Several visualizations were created to understand the dataset and churn patterns.

The analysis includes:

- Customer churn distribution
- Churn by gender
- Churn across different customer characteristics
- Distribution of numerical variables
- Relationship between customer attributes and churn

EDA helped identify patterns and understand the characteristics of customers who are more likely to churn.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Removed the `customerID` identifier.
2. Separated features (`X`) and target (`y`).
3. Converted categorical variables into numerical features using one-hot encoding.
4. Handled missing values.
5. Split the data into training and testing sets.
6. Used stratified sampling to maintain the target-class distribution.
7. Applied `StandardScaler` for Logistic Regression.

The dataset was divided into:

- **80% Training data**
- **20% Testing data**

After encoding, the feature matrix contained **30 features**.

---

## 🤖 Machine Learning Models

Two classification models were developed and compared.

### 1. Logistic Regression

Logistic Regression was used as the primary classification model.

Feature scaling was applied using `StandardScaler` through a Scikit-learn Pipeline.

### 2. Random Forest

Random Forest was used as a second model to capture potentially non-linear relationships between customer characteristics and churn.

---

## 📈 Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

### Model Comparison

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 80.34% | 65.20% | 55.62% | 60.03% | 84.24% |
| Random Forest | 76.93% | 55.88% | 62.30% | 58.91% | 82.43% |

---

## 🏆 Final Model

Based on the overall evaluation, **Logistic Regression** was selected as the final model.

It achieved:

- **80.34% Accuracy**
- **65.20% Precision**
- **60.03% F1-Score**
- **84.24% ROC-AUC**

Random Forest achieved higher recall (**62.30%**) compared with Logistic Regression (**55.62%**).

Therefore, Random Forest could be useful when the primary business objective is to identify as many potential churners as possible. However, Logistic Regression performed better across most of the selected evaluation metrics and was chosen as the final model.

---

## 🔮 Sample Prediction

The final model was also tested on a sample customer from the test dataset.

**Example result:**

```text
Predicted Churn: No
Churn Probability: 4.6%
```

---

## 👤 Author

**Pritha Ghosh**

[GitHub Profile](https://github.com/Pritha21o)