# Customer Segmentation using K-Means Clustering 🚀

## Overview

This project uses **K-Means clustering** to segment customers based on their purchasing behaviors and financial activity. By identifying customer groups, the company can design targeted marketing campaigns to enhance engagement and profitability. 🎯

### Key Objectives
- Segment customers based on their financial and purchasing data.
- Identify optimal clusters using the **Elbow Method** and **Silhouette Score**.
- Provide marketing insights to improve customer retention and business growth.

## Project Structure 🛠️

1. **Data Preprocessing**:
   - Cleaned and scaled the dataset for accurate model performance.
   - Handled missing values and outliers effectively.
   
2. **K-Means Clustering**:
   - Applied the **K-Means algorithm** to identify 5 clusters.
   - Evaluated clustering performance using the **Silhouette Score**.

3. **Cluster Analysis**:
   - Analyzed the clusters based on the average values of the original variables.
   - Visualized the clusters using **t-SNE** for a two-dimensional representation.

## Dataset 📊

The dataset includes various features that describe customer financial behavior. Below is a list of the key features used for clustering:

- **CUST_ID**: Customer's credit card ID (Categorical) 🆔
- **BALANCE**: The remaining balance on the account 💳
- **BALANCE_FREQUENCY**: How often the balance is updated, ranging from 0 to 1 (1 = frequent, 0 = infrequent) 🔄
- **PURCHASES**: Total amount spent by the customer 🛍️
- **ONEOFF_PURCHASES**: Maximum amount spent in a single purchase 💸
- **INSTALLMENTS_PURCHASES**: Amount of purchases made in installments 🛒
- **CASH_ADVANCE**: Cash advance taken by the customer 💵
- **PURCHASES_FREQUENCY**: Frequency of purchases, ranging from 0 to 1 (1 = frequent, 0 = infrequent) 📅
- **ONEOFFPURCHASESFREQUENCY**: Frequency of one-off purchases, ranging from 0 to 1 📦
- **PURCHASESINSTALLMENTSFREQUENCY**: Frequency of installment purchases, ranging from 0 to 1 🔢
- **CASHADVANCEFREQUENCY**: Frequency of cash advances taken by the customer 💰
- **CASHADVANCETRX**: Number of cash advance transactions 💲
- **PURCHASES_TRX**: Number of purchase transactions completed 💳
- **CREDIT_LIMIT**: The credit limit of the cardholder 📈
- **PAYMENTS**: Total payments made by the customer 💳
- **MINIMUM_PAYMENTS**: Minimum amount paid by the customer 🧾
- **PRCFULLPAYMENT**: Percentage of full payments made by the customer 💯
- **TENURE**: Duration of the customer’s credit card service ⏳

The goal is to segment the current customer base into distinct clusters, each of which will receive targeted marketing campaigns from the company. 📣

## Results

### Clustering Summary

The K-Means clustering identified 5 unique customer segments:

1. **Cluster 0**: High balance, frequent cash advances, low full payment rate (riskier customers) 🚨
2. **Cluster 1**: High spending, minimal cash advances, low full payment rate (growth opportunity) 📈
3. **Cluster 2**: High spending, low balance, high full payment rate (most profitable customers) 💎
4. **Cluster 3**: Low spending, frequent cash advances, low full payment rate (high risk) ⚠️
5. **Cluster 4**: Moderate spending, moderate balances, and reasonable full payment rate (potential for growth) 🌱

### Visualizations

- **t-SNE Plot**: The t-SNE visualization confirms the separation between clusters, suggesting that the K-Means algorithm has effectively segmented the customer base. 🔍

## Marketing Insights 💡

Based on the clustering results, here are the recommendations for marketing strategies:

1. **Cluster 2**: Focus on this group for premium offers and loyalty programs. These are the most valuable customers. 🌟
2. **Cluster 1 & Cluster 4**: These customers show potential for growth. Offer promotions to increase spending and encourage full payments. 🎁
3. **Cluster 0 & Cluster 3**: These are high-risk customers. Introduce financial management tools and flexible payment plans to help reduce risk. 🛡️

## How to Run the Project 🖥️

### Prerequisites

- Python 3.x
- Required libraries can be installed via `requirements.txt`:

```bash
pip install -r requirements.txt

