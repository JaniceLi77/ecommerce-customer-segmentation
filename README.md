# E-commerce Customer Analytics (SQL + Python + Machine Learning)

## Overview

This project analyzes e-commerce customer data to understand customer value, identify churn risk, and support data-driven marketing decisions.

The workflow combines SQL for data analysis, Python for data processing and visualization, and machine learning models for customer segmentation and prediction. It simulates a real-world data analytics pipeline from raw data to business insights.

---

## Dataset

The dataset contains customer-level information, including:

* Demographics: Age, Gender, City
* Transaction behavior: Total Spend, Items Purchased
* Engagement metrics: Days Since Last Purchase, Average Rating
* Membership details: Membership Type, Discount Applied

---

## Approach

The project follows a structured analytics workflow:

1. Data loading and cleaning using Python (pandas, numpy)
2. SQL-based analysis using DuckDB
3. Customer segmentation using both rule-based methods and KMeans clustering
4. Churn risk identification using recency metrics
5. Predictive modeling using Random Forest
6. Visualization and insight generation

---

## Key Analysis

### 1. Customer Overview

* Total number of customers
* Average spending and purchase frequency
* Overall customer activity level

### 2. Membership Analysis

* Revenue contribution by membership tier
* Identification of high-value customer groups

### 3. Customer Segmentation

Customers are segmented based on spending behavior:

* High-value customers
* Medium-value customers
* Low-value customers

Additionally, KMeans clustering is applied to identify natural groupings in the data.

### 4. Churn Risk Analysis

* Customers are defined as at risk if they have not purchased for more than 30 days
* Churn rate is calculated
* High-value customers at risk are identified

### 5. Ranking Analysis

* Customers are ranked by total spending using SQL window functions
* Helps identify top contributors to revenue

### 6. Machine Learning Models

* Applied KMeans clustering for customer segmentation
* Built a Random Forest classifier to predict high-value customers
* Split data into training and testing sets using train_test_split
* Evaluated model performance using accuracy, confusion matrix, and classification report

---

## Tools & Technologies

### Programming

* Python

### Libraries

* pandas (data manipulation)
* numpy (numerical operations)
* matplotlib (data visualization)
* seaborn (statistical visualization)
* scikit-learn

  * KMeans (clustering)
  * RandomForestClassifier (prediction)
  * train_test_split (data splitting)
  * classification_report, confusion_matrix, accuracy_score (evaluation)

### Query Engine

* SQL (DuckDB)

### Environment

* Jupyter Notebook

---

## Key Insights

* A small group of high-value customers contributes a large portion of total revenue
* Some high-value customers show signs of inactivity and may churn
* Membership level is strongly associated with spending behavior
* Recency is a strong indicator of customer engagement

---

## Business Impact

This project demonstrates how data analysis can support business decisions:

* Identify valuable customers for targeted marketing
* Detect churn risk early and improve retention
* Optimize resource allocation across customer segments

---

## Project Structure

* `customer_segmentation.ipynb` – Python analysis, visualization, and modeling
* `rfm_analysis.sql` – SQL queries for customer analysis
* `E-commerce Customer Behavior - Sheet1.csv` – dataset

---

## Future Improvements

* Apply more advanced models (e.g., XGBoost, LightGBM)
* Perform feature engineering for better prediction performance
* Build interactive dashboards (e.g., Tableau or Power BI)
* Use real transactional time-series data

---
