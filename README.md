
# Customer Churn Prediction 📊

A Machine Learning project designed to predict customer churn in the telecommunications industry using the Telco Customer Churn dataset.

The objective is to identify customers who are likely to leave the company and help businesses make better customer-retention decisions.

## 📌 Project Overview

This project covers the main stages of a Machine Learning workflow:

- **Exploratory Data Analysis (EDA):** Analysis of customer distributions, churn rates, numerical variables, and categorical features.
- **Data Cleaning:** Conversion of `TotalCharges` to numeric values and treatment of missing values.
- **Data Preprocessing:** Numerical feature scaling and categorical feature encoding using `StandardScaler` and `OneHotEncoder`.
- **Class Imbalance Analysis:** Examination of the distribution between churn and non-churn customers.
- **Model Training:** Comparison of several classification algorithms.
- **Hyperparameter Optimization:** Model tuning using `GridSearchCV` and `StratifiedKFold` cross-validation.
- **Model Evaluation:** Evaluation using Accuracy, Precision, Recall, F1-score, and ROC-AUC.
- **Model Persistence:** Saving the optimized model using Joblib.

## 🤖 Machine Learning Models

The project compares the following algorithms:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- XGBoost

## 📈 Best Model Performance

After hyperparameter optimization using GridSearchCV, XGBoost achieved the following results on the test dataset:

| Metric | Score |
|---|---:|
| Accuracy | 80.91% |
| Precision | 67.92% |
| Recall | 53.21% |
| F1-score | 59.67% |
| ROC-AUC | 84.76% |

XGBoost achieved the highest ROC-AUC among the optimized models. Random Forest obtained a higher Recall and F1-score, making it another interesting candidate when customer churn detection is the main priority.

## 🛠️ Technologies Used

- Python 3.10+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook
- Joblib

## 📂 Project Structure

```text
Customer-Churn-Prediction/
│

│── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── Customer_Churn_Prediction.ipynb
│   
│
├── .gitignore
├── README.md
└── requirements.txt
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows:**
```bash
venv\Scripts\activate
```

**Linux / macOS:**
```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Prepare the dataset

Download the Telco Customer Churn dataset and place the CSV file.


### 5. Run the notebook

```bash
jupyter notebook
```

Open:

```text
notebooks/customer_churn_prediction.ipynb
```

## 📊 Evaluation Metrics

The models are evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted churn customers who actually churn.
- **Recall:** Proportion of actual churn customers correctly detected.
- **F1-score:** Harmonic mean of Precision and Recall.
- **ROC-AUC:** Ability of the model to distinguish between churn and non-churn customers.

## 🎯 Project Objective

The goal is not only to achieve good prediction accuracy, but also to identify customers at risk of leaving the company. This can help telecommunications businesses develop targeted customer-retention strategies.

---

**Developed with Python and Machine Learning.**
