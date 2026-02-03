# Customer Segmentation using Unsupervised Machine Learning

This project applies unsupervised machine learning techniques to segment customers based on demographic attributes, purchasing behavior, and marketing interactions. The objective is to identify meaningful customer groups that can support targeted marketing strategies, improve customer engagement, and optimize business decision-making.

---

## Project Overview

Customer segmentation is a fundamental technique in marketing analytics that enables organizations to better understand their customer base. By grouping customers with similar characteristics, businesses can personalize campaigns, improve retention, and maximize revenue.

This project builds a complete clustering pipeline starting from raw marketing data to actionable customer insights.

### Workflow
- Data cleaning and preprocessing  
- Feature engineering (Total Spending, Campaign Acceptance)  
- Exploratory Data Analysis  
- Feature scaling  
- Clustering model implementation  
- Model evaluation using silhouette score  
- Cluster profiling and business interpretation  

---

## Dataset

The dataset contains customer demographic details, income information, purchasing patterns, and responses to marketing campaigns.

### Key Features
- Year of birth (used to derive customer age)  
- Education and marital status  
- Household composition (children and teenagers)  
- Income  
- Product spending across multiple categories  
- Website visits  
- Campaign acceptance history  
- Recency of last purchase  

Additional engineered features include:

- **Total_Spending**: Aggregate spending across product categories  
- **Total_Campaigns_Accepted**: Number of accepted marketing campaigns  

---

## Models Implemented

Multiple clustering algorithms were evaluated to determine the most effective segmentation strategy:

- Affinity Propagation  
- BIRCH  
- DBSCAN  
- MiniBatch K-Means  

Model performance was compared using silhouette scores to ensure well-separated and meaningful clusters.

---

## Customer Segmentation Report

### Sensible Customers (Low Income, Low Expenses)
- Number of Customers: 364 (16.43%)  
- These customers maintain low spending relative to their income and are financially cautious.

### Careless Customers (Low Income, High Expenses)
- Number of Customers: 1 (0.05%)  
- This segment may represent financially risky behavior due to high spending despite limited income.

### High Income, Low Expenses Customers
- Number of Customers: 4 (0.18%)  
- These customers show strong savings potential and may respond well to premium but value-driven offers.

### High Income, High Expenses Customers
- Number of Customers: 410 (18.50%)  
- A high-value segment likely to engage with luxury products and exclusive campaigns.

---

## Overall Customer Insights

### Income Statistics
- Minimum Income: 1,730.00  
- Maximum Income: 666,666.00  
- Average Income: 52,247.25  

### Expense Statistics
- Minimum Expenses: 5.00  
- Maximum Expenses: 2,525.00  
- Average Expenses: 607.08  

### Demographic Insights
- Post-graduate Customers: 97.56%  
- Customers in a Relationship: 64.53%  
- Customers with One Kid: 40.03%  
- Customers Who Rejected Campaigns: 93.59%  
- Average Customer Age: 44.21 years  

---

## Cluster Summary

| Cluster | Customer Count | Mean Income | Mean Expenses | Mean Age |
|--------|---------------|-------------|---------------|-----------|
| 0 | 589 | 38,043.7 | 200.77 | 42.32 |
| 1 | 344 | 76,383.2 | 1370.00 | 46.12 |
| 2 | 432 | 29,774.7 | 113.27 | 40.47 |
| 3 | 440 | 53,120.0 | 474.66 | 47.60 |
| 4 | 411 | 75,087.3 | 1211.59 | 45.62 |

---

## Key Insights

- Income and total spending are strong indicators of customer behavior.
- High-income clusters contribute significantly to overall revenue.
- A large percentage of customers have not accepted previous campaigns, suggesting an opportunity to improve marketing personalization.
- Distinct behavioral segments enable more effective targeting strategies.

---

## Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- SciPy  
- Matplotlib  
- Seaborn  
- Plotly  

---

## How to Run the Project

### Clone the repository
```bash
git clone https://github.com/Ar9ab007cpu/customer-segmentation-clustering-ml.git
```

### Install dependencies
```bash
pip install -r requirements.txt
```

### Add the dataset
Place the dataset file inside the project directory.

### Run the notebook
```bash
jupyter notebook
```

Open:

```
Customer_Segmentation.ipynb
```

---

## Project Highlights

- Implemented multiple clustering algorithms for robust segmentation.
- Engineered behavioral features to improve cluster quality.
- Evaluated models using silhouette scores.
- Translated clustering results into business-friendly insights.
- Built an end-to-end customer analytics workflow.

---

## Future Improvements

- Apply PCA for dimensionality reduction and improved visualization.
- Automate cluster selection using optimization techniques.
- Deploy the segmentation pipeline for real-time analytics.
- Integrate recommendation systems based on cluster behavior.

---

## Author

Arnab
