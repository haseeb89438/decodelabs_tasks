# Customer Segmentation using PCA & K-Means

A complete unsupervised machine learning project that analyzes customer purchasing behavior using the **Online Retail** dataset. The project transforms raw transactional records into meaningful customer segments through **RFM Analysis**, **Principal Component Analysis (PCA)**, and **K-Means Clustering**, enabling businesses to design data-driven marketing strategies.

---

## Project Overview

Instead of relying on predefined labels, this project discovers hidden customer groups directly from purchase history.

The workflow includes:

- Cleaning and preparing retail transactions
- Engineering RFM (Recency, Frequency, Monetary) features
- Scaling numerical features
- Reducing dimensionality with PCA
- Finding the optimal number of clusters
- Training a K-Means clustering model
- Visualizing customer segments
- Generating business recommendations

---

## Dataset Information

**Dataset:** `Online_Retail.csv`

**Records:** 541,909

### Features

| Column | Description |
|---------|-------------|
| InvoiceNo | Invoice Number |
| StockCode | Product Code |
| Description | Product Description |
| Quantity | Quantity Purchased |
| InvoiceDate | Purchase Date |
| UnitPrice | Price per Unit |
| CustomerID | Unique Customer ID |
| Country | Customer Country |

---

## Workflow

### Data Preparation

The raw dataset is cleaned before analysis.

- Removed cancelled invoices
- Removed missing Customer IDs
- Created a new feature:

```python
Total_Spend = Quantity × UnitPrice
```

---

### RFM Feature Engineering

Each customer is summarized into three important metrics.

| Metric | Meaning |
|---------|----------|
| Recency | Days since last purchase |
| Frequency | Number of purchases |
| Monetary | Total money spent |

These features provide a compact representation of customer behavior.

---

### Data Scaling

Because RFM values have different ranges, all features are standardized using **StandardScaler** before clustering.

---

### Principal Component Analysis (PCA)

PCA is applied to reduce dimensionality while preserving most of the information.

The analysis includes:

- Explained Variance Ratio
- Scree Plot
- Cumulative Variance
- PCA Loading Matrix

---

### K-Means Clustering

To identify the best number of customer groups, the project evaluates multiple values of **K** using:

- Elbow Method
- Silhouette Score

The optimal K is selected before training the final clustering model.

---

### Visualization

Several visualizations are generated to interpret the clusters.

- Distribution plots
- Correlation heatmap
- PCA scatter plot
- 3D cluster visualization
- Cluster heatmap
- Radar chart
- Cluster summary table

---

## Customer Personas

After clustering, each group is interpreted into business-friendly segments.

### Champions

- Recent buyers
- High purchase frequency
- Highest spending customers

**Recommendation**

Reward with loyalty programs and exclusive offers.

---

### At Risk

- Previously valuable customers
- Haven't purchased recently

**Recommendation**

Launch win-back campaigns and personalized discounts.

---

### Casual Customers

- Low purchase frequency
- Low overall spending

**Recommendation**

Increase engagement through promotional campaigns.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

Algorithms:

- PCA
- K-Means
- StandardScaler

---

## Project Structure

```
Customer-Segmentation/
│
├── Online_Retail.csv
├── Customer_Segmentation.ipynb
├── README.md
└── images/
```

---

## Results

The project successfully:

- Extracted customer-level RFM features
- Reduced feature dimensions using PCA
- Identified optimal customer clusters
- Generated meaningful customer personas
- Produced actionable business insights

---

## Business Value

The discovered customer segments can be used for:

- Personalized Marketing
- Customer Retention
- Loyalty Programs
- Targeted Promotions
- Revenue Optimization

---

## Author

**Haseeb**

Machine Learning • Data Science • Artificial Intelligence

GitHub: https://github.com/haseeb89438