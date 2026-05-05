# Customer_Segmentation_Retention_Strategy_using_RFM_Analysis
# Project Overview

This project builds a data-driven customer intelligence system for a retail business. 

The project has two connected layers:

## Layer 1 — RFM Segmentation

You take raw transaction data and engineer three behavioral scores for every customer:

Recency — how recently did they buy? (customers who bought last week are more valuable than those who bought 8 months ago)

Frequency — how often do they buy? (loyal repeat buyers vs one-time shoppers)

Monetary — how much do they spend? (high-value vs low-value customers)

You combine these three scores to classify every customer into a segment — Champions, Loyal, At-Risk, Lost, New Customers, etc.
## Layer 2 — Retention Strategy

Once you know who your customers are, you analyze why segments behave differently
- which products do Champions buy?
- Which months do At-Risk customers start drifting?
- What's the revenue concentration across segments?
- Determine which customers are likely to stay, churn, or require targeted marketing strategies.

# Business Problem

Businesses often struggle with:

- Low customer retention
- High churn rates
- Lack of targeted marketing strategies

This project answers:

Which customers are most valuable, and which are at risk of leaving?, and what business recommendations we can provide so that customers dont churn out.

# Dataset

Source: Kaggle (Online Retail Dataset)

https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci

The data contains transactional data including:
- Customer ID
- Invoice Date
- Description
- Quantity
- Price
- Country
- Invoice
- StockCode

# Project Workflow
## Data Cleaning
- Removed missing Customer IDs
- Filtered out negative quantities (returns)
- Removed invalid pricing values
- Created TotalPrice column
  
## Feature Engineering (RFM)
- Recency → Days since last purchase
- Frequency → Number of purchases
- Monetary → Total spending

## RFM Segmentation
Customers were scored (1–5 scale) and grouped into:

- Loyal Customers
- New Customers
- Average Customers
- Lost Customers

Retention Analysis defined customers as:
- Active → Purchased within last 30 days
- Churned → Inactive beyond 30 days
- Compared retention across segments

## Statistical Analysis
Performed hypothesis testing using SciPy

- Result:
p-value ≈ 0

Purchase frequency significantly impacts retention


## Key Insights
- Loyal customers show highest retention
- Lost customers have extremely high churn
- Average customers are the best target for retention strategies
- High-frequency customers are more likely to stay active

  
## Business Recommendations
- Target at-risk customers with personalized offers
- Introduce loyalty programs for high-value customers
- Re-engage inactive customers with campaigns
- Encourage repeat purchases early

## Tech Stack
- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn


## Visualizations
Customer_Segments_Distribution


![Customer Segments Distribution](https://raw.githubusercontent.com/sejaln123/Customer_Segmentation_-_Retention_Strategy_using_RFM_Analysis/main/Customer_Segments_Distribution.png)


Retention by Customer Segment


![Retention by Customer Segment](https://github.com/sejaln123/Customer_Segmentation_-_Retention_Strategy_using_RFM_Analysis/blob/main/Retention%20by%20Customer%20Segment.png)


## Project Structure
customer_project/

├── data/

├── notebook.ipynb

├── README.md

## Conclusion

This project demonstrates how data-driven segmentation and retention analysis can help businesses improve customer lifetime value and reduce churn.

# Author

Sejal Naik
- Aspiring Data Analyst and Data Scientist
- Skilled in SQL, Python, Power BI, Machine Learning.
- 🔗 LinkedIn: https://www.linkedin.com/in/sejalnaik-/
- 📧 Email: sejal.naik312003@gmail.com

⭐ If you found this useful, give it a star!
