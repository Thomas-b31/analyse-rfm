# Customer segmentation using RFM analysis 

🎯 Objective

The goal of this project is to analyze customer behavior using RFM segmentation (Recency, Frequency, Monetary) in order to:
- Identify high-value customers
- Detect customers at risk of churn
- Support data-driven marketing decisions
- Improve customer retention and revenue growth

🛠️ Tools & Technologies

- Google BigQuery Studio (SQL)
- Power BI (Data visualization & dashboard)

📁 Data Preparation (SQL - BigQuery)

*Data Source*

- 12 monthly sales tables (January → December 2025)
- Each table contains customer transactions (OrderID, CustomerID, OrderDate, OrderValue)

*Data Processing Steps*

- Merged all monthly tables into a single dataset
- Cleaned and validated the data
- Computed RFM metrics for each customer:
  - Recency → days since last purchase
  - Frequency → number of transactions
  - Monetary → total revenue per customer

*RFM Scoring*

- Created R, F, M rankings using SQL window functions
- Converted rankings into deciles (1 to 10)
- Computed a global RFM score (3 to 30)

*Segmentation*

- Customers were segmented into business groups such as:
  - Champions
  - Loyal Customers
  - Potential Loyalists
  - Engaged
  - At Risk
  - Lost/Inactive
 
*Output*

Final dataset includes:
  - CustomerID
  - Recency, Frequency, Monetary
  - RFM scores
  - Segment labels
  - Marketing action recommendations

📊 Dashboard (Power BI)

***Overview Page***
<img width="1457" height="818" alt="Overview" src="https://github.com/user-attachments/assets/658fdbe3-7c77-4a61-99e4-c019c0667200" />

***Deep RFM Analysis***
<img width="1451" height="817" alt="Deep dive" src="https://github.com/user-attachments/assets/5409a154-032d-44c3-9d2f-e26c1d3825c3" />

📈 Key Insights

- High-value customers generate a significant share of total revenue
- A portion of customers shows signs of inactivity (0.02 %)
- Mid-tier segments represent strong growth opportunities

🚀 Business Recommendations

- Retain high-value customers through personalized offers
- Re-engage at-risk customers with targeted campaigns
- Increase frequency for mid-tier customers
- Focus marketing efforts on segments with the highest ROI potential

🧠 Business Questions Answered

- Who are the most valuable customers?
- Which segments generate the most revenue?
- Which customers are at risk of churn?
- Where should marketing efforts be prioritized?

Conclusion

This project demonstrates how data can be leveraged to:
- Segment customers effectively
- Drive marketing strategies
- Improve business performance through analytics


