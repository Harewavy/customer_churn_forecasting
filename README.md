# Telecom Customer Churn Prediction

This project was completed as part of the final stage in the machine learning track at TripleTen. The objective was to develop a model for predicting customer churn for Interconnect, a telecom operator. By identifying customers likely to leave, the company can offer special deals and retain them more effectively.

---

## Project Objective

To analyze subscriber behavior and train a binary classification model that predicts customer churn using contract, internet, phone, and personal information.

### Target

* `EndDate`: If `EndDate == 'No'`, the customer has not churned. This is the binary target for churn prediction.

### Evaluation Metric

* Primary: AUC-ROC
* Secondary: Accuracy

---

## Project Steps

### Exploratory Data Analysis

* Investigated all datasets (`contract.csv`, `personal.csv`, `internet.csv`, `phone.csv`)
* Cleaned and merged the datasets on `customerID`
* Identified and handled missing values and anomalies
* Converted categorical variables and dates appropriately

### Work Plan

Outlined and followed a clear plan:

1. **EDA**: Understand data distribution, class imbalance, and data quality
2. **Preprocessing**: Encode, merge, and scale features
3. **Modeling**: Train several models and tune hyperparameters
4. **Evaluation**: Compare models on validation and test sets using AUC-ROC
5. **Reporting**: Document findings and results

### Modeling

Trained and compared multiple models:

* Logistic Regression
* Random Forest
* CatBoost
* LightGBM (Best model)

### Final Model

**LightGBM** was selected for its strong performance and fast training speed.

* **AUC-ROC**: **0.886**
* **Accuracy**: 0.84

---

## Solution Report Summary

* All planned steps were completed
* Main challenge: Ensuring consistent data structure across merged datasets
* Solved via strict preprocessing checks and merging strategy
* LightGBM delivered the best AUC-ROC score, exceeding the 0.88 benchmark

---

## Conclusion

The model can successfully predict customer churn, giving Interconnect an opportunity to proactively retain clients through strategic offers.

This project showcases my ability to:

* Work with multiple related datasets
* Handle data preprocessing and cleaning
* Train, tune, and evaluate classification models
* Communicate results clearly

---

## Author

**Enes Ozturk**

* Email: nsztrk00@icloud.com
* [LinkedIn](https://www.linkedin.com/in/enesoztrkk/)
* [GitHub](https://github.com/enesoztrkk)

---

## Tech Stack

* Python, Pandas, NumPy, Matplotlib, Seaborn
* Scikit-learn, LightGBM, CatBoost
* Jupyter Notebook
