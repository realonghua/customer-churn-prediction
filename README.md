# customer-churn-prediction
Customer churn prediction using RFM features and machine learning models (Logistic Regression, Random Forest, XGBoost, LightGBM) with focus on recall optimization.
# 📊 Customer Churn Prediction

This project focuses on predicting customer churn using RFM-based features and machine learning models. The goal is to identify customers at risk of leaving and support data-driven retention strategies.

---

## 🎯 Objective

- Predict customer churn (0 = Active, 1 = Churned)
- Focus on **Recall** to minimize missed churn cases
- Compare multiple machine learning models
- Provide actionable business insights

---

## 📁 Project Structure
customer-churn-prediction/
│
├── notebooks/
│ ├── 1_data_preprocessing.ipynb
│ └── 2_modeling.ipynb
│
├── data/
│ └── sample_data.csv
│
├── images/
│ ├── confusion_matrices.png
│ ├── roc_curves.png
│ └── feature_importance.png
│
├── README.md
└── requirements.txt


---

## 🧠 Feature Engineering

RFM-based features are created for each customer:

- **Recency**: Days since last purchase
- **Frequency**: Number of transactions
- **Monetary**: Total spending
- **Avg Order Value**: Average value per order
- **Purchase Interval**: Time gap between purchases

---

## 🤖 Models Used

- Logistic Regression
- Random Forest
- XGBoost
- LightGBM

---

## 📊 Model Performance

### 🔍 Confusion Matrix

![Confusion Matrix](images/confusion_matrices.png)

The confusion matrices show that tree-based models (Random Forest, XGBoost, LightGBM) achieve near-perfect classification, with extremely low false negatives.

This is critical in churn prediction because:
- Missing a churned customer (False Negative) leads to high business loss
- Predicting churn incorrectly (False Positive) only results in minor marketing cost



---

### 🧠 Feature Importance


Key drivers of churn:

- **Recency**: Customers inactive for a long time are more likely to churn
- **Frequency**: Less frequent purchases indicate weaker engagement
- **Monetary**: Low spending customers have higher churn risk

---

## 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall ⭐ (priority)
- F1-score
- ROC-AUC

> In churn prediction, **Recall is the most important metric** because missing a churned customer leads to significant business loss.

---


## ⚠️ Important Note

- Dataset is not fully included due to size constraints
- A sample dataset is provided for demonstration
- Train/test split is applied before modeling to avoid data leakage

---

## 💡 Business Insights

- High recency → strong indicator of churn risk
- Low frequency and spending → weak customer engagement
- At-risk high-value customers should be prioritized for retention campaigns

---

## 🚀 Future Improvements

- Add behavioral data (clickstream, browsing)
- Hyperparameter tuning
- Deploy model as API or dashboard
- Implement real-time churn prediction

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost, LightGBM
- Matplotlib, Seaborn

---

## 👤 Author

**Long Hua**
