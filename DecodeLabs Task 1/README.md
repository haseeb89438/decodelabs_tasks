# Advanced Exploratory Data Analysis & Feature Engineering

This project focuses on performing comprehensive Exploratory Data Analysis (EDA) and feature engineering on an E-commerce Orders dataset. The objective is to transform raw data into a clean, structured dataset by handling missing values, detecting outliers, creating meaningful features, and uncovering business insights through statistical analysis and visualization.

## Project Overview

Raw datasets often contain inconsistencies that reduce the performance of machine learning models. This project demonstrates a complete preprocessing workflow, including data cleaning, feature engineering, encoding, scaling, and visualization to prepare the data for predictive analytics.

## Dataset

**Dataset:** `Dataset for Data Analytics - Sheet1.csv`

**Total Records:** 1,200

### Features

| Category | Columns |
|----------|---------|
| Order Information | OrderID, CustomerID, TrackingNumber |
| Product Details | Product, Quantity, UnitPrice, ItemsInCart |
| Transaction Details | Date, ShippingAddress, PaymentMethod, OrderStatus, CouponCode, ReferralSource, TotalPrice |

---

## Project Workflow

### Data Inspection

The dataset is explored to understand its structure and quality.

Tasks performed:

- Checked data types
- Identified missing values
- Examined duplicate records
- Generated descriptive statistics

### Data Cleaning

Data quality is improved by addressing inconsistencies.

- Removed duplicate records
- Handled missing values
- Corrected data formats
- Verified data consistency

### Missing Value Treatment

Missing values are handled using appropriate preprocessing techniques.

Methods used:

- KNN Imputer
- Statistical imputation where applicable

This helps preserve useful information while minimizing data loss.

### Outlier Detection

Potential outliers are identified using statistical techniques.

Methods include:

- Box Plots
- Interquartile Range (IQR)

Detected outliers are analyzed before treatment to reduce their impact on future modeling.

### Feature Engineering

Several new features are generated to improve analytical value.

Examples include:

- Year
- Month
- Day
- Day of Week

The relationship between Quantity, Unit Price, and Total Price is also validated.

### Data Encoding

Categorical variables are converted into numerical form using:

- One-Hot Encoding

This prepares the dataset for machine learning algorithms.

### Feature Scaling

Numerical variables are normalized using:

- StandardScaler
- MinMaxScaler

Scaling ensures consistent feature ranges for model training.

### Exploratory Data Analysis

The project includes multiple visualizations to understand customer purchasing behavior.

Visualizations include:

- Histograms
- Distribution Plots
- Scatter Plots
- Box Plots
- Correlation Heatmap

These analyses reveal trends, relationships, and potential anomalies within the dataset.

### Feature Selection

Important variables are identified using:

- Mutual Information Scores
- Random Forest Feature Importance

These techniques help determine which features contribute the most valuable information for predictive modeling.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

### Preprocessing Techniques

- KNN Imputer
- One-Hot Encoding
- StandardScaler
- MinMaxScaler

### Machine Learning

- Random Forest

---

## Project Structure

```
Advanced-EDA-Feature-Engineering/
│
├── Dataset for Data Analytics - Sheet1.csv
├── Advanced_EDA.ipynb
├── README.md
└── images/
```

---

## Results

The project successfully:

- Cleaned and prepared the dataset
- Treated missing values and outliers
- Created meaningful engineered features
- Encoded and scaled data
- Identified important variables
- Produced detailed visual insights for business analysis

---

## Applications

The preprocessing techniques demonstrated in this project are applicable to:

- Data Analytics
- Business Intelligence
- Machine Learning
- Customer Behavior Analysis
- Predictive Modeling

---

## Author

**Haseeb**

Machine Learning | Data Science | Artificial Intelligence

GitHub: https://github.com/haseeb89438