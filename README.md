# ⚙️ Predictive Maintenance – Machine Failure Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting potential machine failures using Machine Learning classification algorithms.

Using the **AI4I 2020 Predictive Maintenance Dataset**, the project analyzes machine operating conditions and sensor readings to identify whether a machine is likely to fail.

The objective is to support proactive maintenance, reduce unexpected machine downtime, and minimize unnecessary maintenance costs.

## 🎯 Project Objective

- Analyze industrial machine operating conditions.
- Identify patterns associated with machine failures.
- Build and compare multiple Machine Learning classification models.
- Select the best-performing model based on evaluation results.
- Predict machine failures using new, unseen data.

## 📂 Dataset Description

- **Dataset:** AI4I 2020 Predictive Maintenance Dataset
- **Source:** UCI Machine Learning Repository
- **Records:** 10,000
- **Columns:** 14
- **Tables:** 1
- **Missing Values:** None (as reported by UCI)

🔗 **Dataset Link:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset)

### Input Features (X)

| Feature | Description |
|---|---|
| Type | Product quality type (L, M, H) |
| Air temperature [K] | Air temperature |
| Process temperature [K] | Operating process temperature |
| Rotational speed [rpm] | Machine rotational speed |
| Torque [Nm] | Machine torque |
| Tool wear [min] | Tool usage duration |

### Target Variable (y)

**Machine failure**

- `0` – No Machine Failure
- `1` – Machine Failure

Identifier columns and failure-mode indicators were excluded from model training to avoid unnecessary features and target leakage.

## 🛠️ Methodology

The project follows these steps:

1. **Data Loading** – Imported the dataset and required Python libraries.
2. **Data Inspection and Cleaning** – Examined the dataset, checked data quality and prepared the data.
3. **Feature Selection** – Selected six relevant input features and the target variable.
4. **Train-Test Split** – Divided the dataset into 80% training and 20% testing data.
5. **Model Building** – Trained multiple classification algorithms.
6. **Model Evaluation** – Compared model performance using evaluation metrics.
7. **Model Selection** – Selected the best-performing model based on testing accuracy.
8. **New Data Prediction** – Applied the selected model to predict machine failures on unseen data.

## 🤖 Applied Machine Learning Algorithms

The following classification algorithms were implemented:

1. Logistic Regression (LR)
2. Decision Tree Classifier (DTC)
3. Random Forest Classifier (RFC)
4. Support Vector Classifier (SVC)
5. K-Nearest Neighbors Classifier (KNNC)

## 📊 Model Evaluation and Results

The models were compared based on their testing accuracy.

| Algorithm | Testing Accuracy |
|---|---:|
| Decision Tree Classifier | **98.35%** |
| Random Forest Classifier | 97.80% |
| Logistic Regression | 97.05% |
| Support Vector Classifier | 97.05% |
| K-Nearest Neighbors | 96.60% |

### 🏆 Best Performing Model

**Decision Tree Classifier (DTC)** achieved the highest testing accuracy of **98.35%** among the five models.

The selected model was further applied to predict machine failures using new, unseen data.

*Note: Since the dataset is highly imbalanced, accuracy alone is not sufficient to establish the best model. Failure-class precision, recall, F1-score and confusion matrix should also be considered.*

## 💡 Key Findings

- Machine failure prediction can be approached as a binary classification problem.
- Different classification algorithms produce different prediction performances.
- Decision Tree Classifier achieved the highest testing accuracy among the models compared.
- Machine operating conditions and sensor readings provide useful information for identifying potential failures.
- Machine Learning predictions can support proactive maintenance decisions.

## 🧰 Tools and Technologies

- **Programming Language:** Python
- **Environment:** Jupyter Notebook / Google Colab
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Machine Learning:** Classification Algorithms

## 🚀 Conclusion

This project demonstrates how Machine Learning can be used to predict industrial machine failures based on operating conditions.

By comparing five classification algorithms, the Decision Tree Classifier achieved the highest testing accuracy of 98.35%.

The selected model was successfully applied to new, unseen data to predict potential machine failures, demonstrating the practical application of predictive maintenance.

---

## 👨‍💻 Author

**Mohammed Shadil P.K.**

Aspiring Data Analyst | Machine Learning Enthusiast

---
⭐ If you find this project interesting, feel free to explore the repository!
