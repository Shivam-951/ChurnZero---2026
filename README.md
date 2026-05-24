# ChurnZero 26 – AI-Powered Customer Churn Prediction System

An advanced machine learning solution developed for the ChurnZero 26 competition to predict customer churn in the banking sector using behavioral, transactional, financial, and digital engagement data.

This project focuses on identifying high-risk customers and enabling proactive retention strategies through intelligent churn prediction and risk scoring.

---

# Problem Statement

Customer churn is one of the biggest challenges in the banking industry. Losing existing customers directly impacts revenue, customer lifetime value, and brand loyalty.

The objective of this project is to build a robust machine learning system capable of:

- Predicting whether a customer is likely to churn
- Estimating churn probability
- Identifying behavioral and financial risk patterns
- Supporting data-driven customer retention strategies

---

# Project Highlights

- End-to-end ML pipeline
- Advanced feature engineering
- Banking behavioral analytics
- Customer risk scoring
- LightGBM-based predictive modeling
- Automated predictions CSV generation
- Competition-ready notebook and submission workflow

---

# Dataset Features

The dataset contains multiple banking-related attributes including:

- Customer demographics
- Transaction history
- Login activity
- Digital banking usage
- Credit utilization
- Complaint and escalation records
- Financial risk indicators
- Customer engagement metrics
- Sentiment-related features

---

# Feature Engineering

Several domain-driven engineered features were created to improve predictive performance.

| Feature | Description |
|---|---|
| `digital_depth_score` | Measures customer digital engagement |
| `financial_stress_index` | Estimates customer financial pressure |
| `service_friction_index` | Captures complaint and escalation intensity |
| `balance_txn_decline_score` | Detects transaction and balance decline patterns |
| `avg_txn_value` | Average transaction amount |
| `login_inactive_flag` | Identifies inactive digital users |

---

# Machine Learning Models Explored

The following models were evaluated:

- Logistic Regression
- Random Forest
- XGBoost
- LightGBM

## Final Selected Model

### LightGBM Classifier

### Why LightGBM?

- High predictive performance
- Fast training speed
- Better handling of feature interactions
- Excellent performance on structured banking datasets

---

# Workflow Pipeline

```text
Raw Dataset
   ↓
Data Cleaning & Preprocessing
   ↓
Feature Engineering
   ↓
Categorical Encoding
   ↓
Model Training (LightGBM)
   ↓
Evaluation & Validation
   ↓
Predictions on Test Dataset
   ↓
submission.csv Generation
```

---

# Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

The primary focus was minimizing false negatives to better identify customers at risk of churn.

---

# Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# Repository Structure

```text
├── ChurnZero_Final_Notebook.ipynb
├── ChurnZero_dataset_v1.csv
├── ChurnZero_test_v1.csv
├── ChurnZero_Predictions.csv
├── README.md
└── requirements.txt
```

---

# Installation & Usage

## Clone the Repository

```bash
git clone <repository-link>
cd churnzero26
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run the Notebook

Open:

```text
ChurnZero_Final_Notebook.ipynb
```

Run all cells sequentially.

---

# Output

The system generates:

```text
ChurnZero_Predictions.csv
```

Containing:

- `customer_id`
- `churn_prediction`
- `churn_probability`

---

# Real-World Applications

This solution can help banks:

- Reduce customer attrition
- Improve retention campaigns
- Identify high-risk customers early
- Optimize customer engagement
- Enhance CRM decision-making
- Enable AI-driven banking analytics

---

# Challenges Faced

- Handling imbalanced data
- Managing missing values
- Preventing feature leakage
- Optimizing model performance
- Creating meaningful domain-specific features

---

# Future Improvements

- Real-time churn prediction APIs
- Explainable AI dashboards
- Deep learning integration
- Personalized retention recommendation systems
- Cloud deployment support

---

# Team

Developed as part of the ChurnZero 26 competition submission.

---

# License

This project is intended for educational and competition purposes only.
