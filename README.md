# Customer_Segmentation_-_Retention_Strategy_using_RFM_Analysis
This project focuses on analyzing customer purchasing behavior using RFM (Recency, Frequency, Monetary) analysis and identifying retention patterns to support business decision-making.

The goal is to segment customers based on their transaction history and determine which customers are likely to stay, churn, or require targeted marketing strategies.

# Business Problem

Businesses often struggle with:

- Low customer retention
- High churn rates
- Lack of targeted marketing strategies

This project answers:

Which customers are most valuable, and which are at risk of leaving?

📊 Dataset
Source: Kaggle (Online Retail Dataset)
Contains transactional data including:
Customer ID
Invoice Date
Quantity
Price
Country
🧹 Data Cleaning
Removed missing Customer IDs
Filtered out negative quantities (returns)
Removed invalid pricing values
Created TotalPrice column
🧠 Feature Engineering (RFM)
Recency → Days since last purchase
Frequency → Number of purchases
Monetary → Total spending
🔢 RFM Segmentation

Customers were scored (1–5 scale) and grouped into:

🟩 Loyal Customers
🟨 New Customers
🟦 Average Customers
🟥 Lost Customers
📈 Retention Analysis
Defined customers as:
Active → Purchased within last 30 days
Churned → Inactive beyond 30 days
Compared retention across segments
🔬 Statistical Analysis
Performed hypothesis testing using SciPy
Result:
p-value ≈ 0
Purchase frequency significantly impacts retention
📊 Key Insights
Loyal customers show highest retention
Lost customers have extremely high churn
Average customers are the best target for retention strategies
High-frequency customers are more likely to stay active
🚀 Business Recommendations
Target at-risk customers with personalized offers
Introduce loyalty programs for high-value customers
Re-engage inactive customers with campaigns
Encourage repeat purchases early
🛠️ Tech Stack
Python
Pandas
NumPy
SciPy
Matplotlib
Seaborn
📸 Visualizations

(Add screenshots here)

📁 Project Structure
customer_project/
│
├── data/
├── notebook.ipynb
├── README.md
💬 Conclusion

This project demonstrates how data-driven segmentation and retention analysis can help businesses improve customer lifetime value and reduce churn.

⭐ If you found this useful, give it a star!
