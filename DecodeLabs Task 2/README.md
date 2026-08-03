# Credit Card Fraud Detection using Machine Learning

A supervised machine learning project focused on detecting fraudulent credit card transactions. The project addresses the challenge of highly imbalanced data through preprocessing, feature engineering, SMOTE oversampling, model comparison, hyperparameter tuning, and comprehensive performance evaluation.

## Project Overview

Financial fraud is a rare but costly event. Traditional accuracy metrics often fail to measure model effectiveness because legitimate transactions greatly outnumber fraudulent ones.

This project develops a complete fraud detection pipeline capable of identifying suspicious transactions while minimizing false alarms.

## Dataset

**Dataset:** `credit_card_fraud_10k.csv`

**Total Records:** 10,000

**Target Variable:** `is_fraud`

### Features

| Feature | Description |
|---------|-------------|
| amount | Transaction amount |
| transaction_hour | Time of transaction |
| merchant_category | Merchant type |
| foreign_transaction | International transaction indicator |
| location_mismatch | Billing and transaction location mismatch |
| device_trust_score | Device reliability score |
| velocity_last_24h | Recent transaction frequency |
| cardholder_age | Customer age |

The dataset is highly imbalanced, with only a small percentage of fraudulent transactions.

---

## Project Workflow

### Data Preparation

The dataset is divided into:

- Features (X)
- Target (y)

An 80:20 train-test split is performed before model development.

### Data Preprocessing

A preprocessing pipeline is created using **ColumnTransformer**.

Numerical features are standardized using:

- StandardScaler

Categorical features are encoded using:

- OneHotEncoder

This ensures that all variables are suitable for machine learning algorithms.

### Handling Class Imbalance

Since fraud cases are rare, the project applies **SMOTE (Synthetic Minority Oversampling Technique)** to generate additional synthetic fraud samples.

Benefits include:

- Better class balance
- Improved fraud detection
- Reduced model bias toward legitimate transactions

### Machine Learning Models

Two supervised learning algorithms are implemented.

**Logistic Regression**

- Fast baseline model
- High interpretability

**Random Forest Classifier**

- Ensemble learning algorithm
- Captures complex fraud patterns
- Produces feature importance scores

### Hyperparameter Optimization

Model parameters are optimized using **GridSearchCV** with cross-validation to improve performance while reducing overfitting.

### Model Evaluation

Multiple evaluation metrics are used instead of relying only on accuracy.

- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Precision-Recall Curve

These metrics provide a better understanding of fraud detection performance on imbalanced datasets.

### Feature Importance

The trained Random Forest model identifies the most influential features contributing to fraud prediction.

This helps explain model behavior and supports business decision-making.

### Model Saving

The final trained model is exported using **Joblib**, making it ready for future deployment.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Imbalanced-Learn

### Machine Learning

- Logistic Regression
- Random Forest Classifier
- SMOTE
- GridSearchCV
- ColumnTransformer
- OneHotEncoder
- StandardScaler

---

## Project Structure

```
Credit-Card-Fraud-Detection/
│
├── credit_card_fraud_10k.csv
├── Fraud_Detection.ipynb
├── fraud_model.pkl
├── README.md
└── images/
```

---

## Results

The project successfully:

- Built a complete fraud detection pipeline
- Addressed class imbalance using SMOTE
- Compared multiple machine learning models
- Optimized model performance through hyperparameter tuning
- Evaluated models using appropriate imbalance-aware metrics
- Saved the best-performing model for deployment

---

## Applications

This project demonstrates techniques commonly used in:

- Banking
- Online Payments
- Digital Wallets
- Financial Risk Analysis
- Fraud Monitoring Systems

---

## Author

**Haseeb**

Machine Learning | Data Science | Artificial Intelligence

GitHub: https://github.com/haseeb89438