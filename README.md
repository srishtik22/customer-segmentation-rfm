Customer Segmentation & Retention Analysis using RFM
Project Overview

This project focuses on analyzing customer purchase behavior using RFM (Recency, Frequency, Monetary) analysis to segment customers, understand retention patterns, and identify revenue-driving customer groups for targeted business decisions.

Dataset

Dataset: Online Retail Transaction Data

Initial size: ~500,000+ transaction records

Final analyzed data: 400,000+ clean transaction rows

Customers analyzed: 4,000+ unique customers

The dataset contains transactional information such as invoice numbers, purchase dates, quantities, prices, customer IDs, and country.

Data Cleaning & Preparation

The following steps were performed before analysis:

Removed transactions with missing CustomerID

Filtered out cancelled invoices

Ensured correct data types for dates and numerical fields

Created a TotalAmount column for monetary analysis

After cleaning, the dataset was reduced to ~400K valid transactions used for analysis.

RFM Metrics Calculation

For each customer:

Recency (R): Number of days since the customer’s most recent purchase

Frequency (F): Total number of purchases made

Monetary (M): Total amount spent by the customer

These metrics were calculated using the most recent invoice date as the reference point.

RFM Scoring

Customers were scored on a 1–5 scale for each RFM metric using quantile-based thresholds:

R Score: 5 = most recent customers

F Score: 5 = most frequent buyers

M Score: 5 = highest spenders

This resulted in an RFM score for each customer, which was then used for segmentation.

Customer Segmentation

Based on RFM scores, customers were grouped into meaningful business segments such as:

Champions

Loyal Customers

New Customers

At-Risk Customers

Lost Customers

Each segment represents a distinct behavioral pattern that can be targeted with different business strategies.

Retention & Revenue Analysis

Key findings from the analysis:

Champions contributed ~70% of total revenue, despite being a smaller portion of customers

Loyal and New customers showed consistent repeat purchasing behavior

At-risk and Lost customers contributed minimal revenue, highlighting churn risk

A significant portion of customers were one-time buyers, indicating scope for retention strategies

Revenue contribution was analyzed segment-wise to understand where business value is concentrated.

Tools & Technologies

Python

Pandas

NumPy

Matplotlib / Seaborn

Key Business Insights

Revenue is highly concentrated among high-value customers

Retention efforts should prioritize Champions and Loyal customers

Targeted campaigns can be designed to convert New customers into Loyal customers

At-risk customers can be re-engaged with personalized offers

Conclusion

This project demonstrates how RFM analysis can be used on large-scale transactional data (400K+ rows) to derive actionable customer insights, improve retention strategies, and support data-driven marketing decisions without relying on predictive modeling.# customer-segmentation-rfm
customer-segmentation-rfm
