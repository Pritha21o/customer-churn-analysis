# Customer Churn Prediction

## 📌 Project Overview

This project predicts whether a customer is likely to churn using Machine Learning.

The project uses the Telco Customer Churn dataset and compares two classification models:

- Logistic Regression
- Random Forest

The models are evaluated using Accuracy, Precision, Recall, F1 Score, and ROC-AUC.

## 🎯 Objective

The main objective is to identify customers who are likely to leave the company so that businesses can take suitable customer retention actions.

## 📂 Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains information about customers, including their services, contract details, payment information, and churn status.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 🔄 Project Workflow

1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis
4. Data Preprocessing
5. Model Training
6. Model Evaluation
7. ROC Curve Analysis
8. Feature Importance Analysis
9. Model Comparison
10. Final Churn Prediction

## 🤖 Machine Learning Models

### Logistic Regression

Logistic Regression was used as one of the classification models for predicting customer churn.

### Random Forest

Random Forest was used as a second classification model and compared with Logistic Regression.

## 📊 Model Results

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 80.34% | 65.20% | 55.62% | 60.03% | 84.24% |
| Random Forest | 76.93% | 55.88% | 62.30% | 58.91% | 82.43% |

## 🏆 Final Model

Based on the overall evaluation, **Logistic Regression** was selected as the final model.

It achieved:

- Accuracy: **80.34%**
- F1 Score: **60.03%**
- ROC-AUC: **84.24%**

## 🔮 Example Prediction

For one sample customer from the test dataset:

- Predicted Churn: **No**
- Churn Probability: **4.6%**

This indicates that the model predicted a low probability of churn for that customer.

## 💡 Conclusion

The project demonstrates how Machine Learning can be used to predict customer churn.

Among the two tested models, Logistic Regression performed better overall based on Accuracy, Precision, F1 Score, and ROC-AUC. The model can potentially help businesses identify customers at risk of leaving and support customer retention strategies.

## 👩‍💻 Author

Pritha Ghosh