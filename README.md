# Customer-Segmentation-RFM-Analysis-
RFM Customer Segmentation Project (Online Retail II)
1. Project Overview

This project focuses on performing RFM (Recency, Frequency, Monetary) analysis on the Online Retail II dataset to understand customer purchasing behavior and segment customers into meaningful business categories such as Champions, Loyal Customers, At Risk, and Lost. The goal is to help businesses improve customer retention, targeted marketing, and revenue growth using data-driven insights.

2. Dataset Description
Dataset Name: Online Retail II
Source: UCI Machine Learning Repository / Kaggle
Data Type: Transactional retail data
Time Period: 2009–2011

Key Columns Used:
Invoice – Unique transaction ID (canceled invoices start with 'C')
InvoiceDate – Date and time of transaction
Customer ID – Unique customer identifier
Quantity – Number of items purchased
Price – Unit price of product

3. Tools & Technologies Used
Google Colab – Data processing and analysis
Python (Pandas, Matplotlib) – Data cleaning, RFM analysis, visualization
Excel – Data inspection and validation
CSV – Data storage and export format
Git & GitHub – Version control and project submission

4. Project Workflow & Steps
Step 1: Load Dataset and Data Cleaning
Loaded the dataset into Pandas.
Removed records with null Invoice values.
Removed canceled orders (Invoices starting with 'C').
Filtered out rows with missing Customer IDs.
Removed invalid transactions with zero or negative quantity/price.

Step 2: Convert Invoice Date
Converted InvoiceDate column to datetime format for time-based analysis.

Step 3: RFM Metric Computation
Recency: Number of days since the customer’s last purchase.
Frequency: Number of unique invoices per customer.
Monetary: Total amount spent by each customer.

Step 4: RFM Score Bucketing
Used quantile-based segmentation (1–5) for R, F, and M scores.
Recency scoring was reversed (lower days = higher score).
Combined R, F, and M scores to form an RFM score.

Step 5: Customer Segmentation
Customers were classified into business segments:
Champions
Loyal Customers
Potential Loyalists
Recent Customers
At Risk
Cannot Lose Them
Hibernating
Lost

Step 6: Data Visualization
Created a bar chart to visualize the number of customers in each segment.
Helped identify dominant and weak customer groups.

Step 7: Export Results
Exported the final customer segmentation table to CSV format for use in BI tools and reporting.

5. Key Insights Identified
Champions and Loyal Customers contribute significantly to repeat purchases and revenue.
A notable portion of customers fall into At Risk and Hibernating segments, indicating churn risk.
Lost customers represent a segment with minimal recent engagement and low purchase frequency.
Recent and Potential Loyalists show strong potential for conversion into loyal customers.

6. Business Actions & Recommendations
Champions
Offer exclusive rewards and early product access.
Encourage referrals and customer advocacy.
Provide premium personalized offers.

Loyal Customers
Strengthen loyalty programs.
Upsell and cross-sell related products.
Maintain personalized engagement.

Potential Loyalists
Provide targeted discounts.
Recommend products based on history.
Nurture via follow-up campaigns.

At Risk
Launch re-engagement campaigns.
Offer limited-time incentives.
Collect feedback to understand churn reasons.

Hibernating & Lost
Run win-back campaigns with special offers.
Reduce marketing spend on unresponsive customers.
Analyze churn patterns for prevention strategies.

7. Business Improvement Suggestions
Implement segment-based marketing strategies instead of mass campaigns.
Focus retention efforts on Champions and Loyal Customers.
Use targeted promotions to recover At Risk customers.
Monitor RFM scores periodically to track customer movement across segments.

8. Final Outcome
This project successfully demonstrates how RFM analysis can transform raw transactional data into actionable customer insights. The segmentation enables businesses to optimize marketing strategies, improve customer retention, and increase overall profitability.
