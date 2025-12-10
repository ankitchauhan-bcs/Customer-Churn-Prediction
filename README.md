# 📊 Customer Churn Prediction – Machine Learning Project

This project builds a **complete end-to-end Customer Churn Prediction Model** using Python and Machine Learning. The goal is to help companies identify customers who are likely to leave (churn) so they can take action to improve retention.

---

## 🚀 Project Overview

Customer churn is a key metric for subscription-based businesses. In this project, I:

* Created a **synthetic churn dataset** (`customer_churn.csv`)
* Performed **data cleaning**
* Conducted **EDA (Exploratory Data Analysis)**
* Built and trained **machine learning models**
* Evaluated models with accuracy, confusion matrix & classification report
* Saved the dataset and source code for reuse

---

## 📁 Project Structure

```
📦 Customer-Churn-Prediction
├── 📄 customer_churn.csv
├── 📄 churn_model.ipynb
├── 📄 README.md
└── 📄 requirements.txt
```

---

## 🧪 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📥 Dataset

This project contains a synthetic dataset: **`customer_churn.csv`**

Columns include:

| Column Name      | Description                    |
| ---------------- | ------------------------------ |
| customer_id      | Unique ID                      |
| gender           | Male/Female                    |
| age              | Customer age                   |
| monthly_charges  | Monthly bill                   |
| tenure_months    | Months since subscription      |
| internet_service | DSL / Fiber / No               |
| contract_type    | Type of contract               |
| payment_method   | UPI / Credit Card / Auto Debit |
| total_charges    | Total amount spent             |
| churn            | 1 = Yes, 0 = No                |

---

## 📈 Exploratory Data Analysis (EDA)

EDA includes:

* Churn distribution
* Contract type vs. churn
* Tenure vs. churn
* Monthly charges comparison
* Correlation heatmap

Example Plot:

```python
sns.countplot(data=df, x='churn')
plt.title("Churn Count")
plt.show()
```

---

## 🤖 Model Building

Steps performed:

1. **Label encoding & feature transformation**
2. **Train-test split**
3. **Model training**

   * Logistic Regression
   * Random Forest
4. **Model Evaluation**

   * Accuracy
   * Confusion Matrix
   * Classification Report

Example Code:

```python
from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier()
model.fit(X_train, y_train)
pred = model.predict(X_test)
```

---

## 📊 Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | ~85%     |
| Random Forest       | ~90%     |

(Random values — based on synthetic dataset)

---

## 🛠 How to Run the Project

#### 1️⃣ Clone the repo

```bash
git clone https://github.com/ankitchauhan-bcs/Customer-Churn-Prediction.git
```

#### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

#### 3️⃣ Run Notebook

```
jupyter notebook churn_model.ipynb
```

---
