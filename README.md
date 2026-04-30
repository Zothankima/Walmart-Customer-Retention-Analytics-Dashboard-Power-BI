# Walmart Customer Retention Analytics Dashboard

## Project Overview
This project was developed as part of a Power BI Analytics 
assignment to design an interactive Customer Retention Dashboard 
for Walmart. As a Power BI Analyst, the goal was to consolidate 
fragmented customer data and deliver actionable insights to 
address customer churn, loyalty engagement and regional 
retention strategies.

---

## Problem Statement
Walmart faces increasing competition from Amazon, Target and 
other retailers. Despite collecting vast data on purchases, 
loyalty programs and online interactions, their reporting 
lacked analytical depth to:
- Understand why customers are churning
- Identify loyal vs. at-risk customers
- Measure the impact of loyalty tiers and promotions
- Guide region and channel-specific retention strategies

---

## Datasets Used
| Dataset | Key Columns |
|---|---|
| Customer_Demographics | Customer_ID, Age, Gender, Region, Income_Level, Membership_Since, Preferred_Channel |
| Customer_Transactions | Transaction_ID, Customer_ID, Store_ID, Product_Category, Amount, Promotion_Applied |
| Store_Locations | Store_ID, Store_Type, Region, Opening_Year |
| Loyalty_Program | Customer_ID, Loyalty_Tier, Points_Earned, Points_Redeemed |
| Churn_Labelled_Customers | Customer_ID, Last_Purchase_Date, Churn_Flag, Churn_Reason |

---

## Tasks Performed

### Task 1 — Data Modeling & Cleaning
- Loaded and transformed all 5 datasets in Power Query
- Handled duplicates, missing values and data types
- Created calculated columns: Membership Duration, 
  Transaction Year, Transaction Month
- Built Star Schema data model in Power BI Model View

### Task 2 — Churn & Retention Metrics
- Created Churn Rate KPI = (Churned / Total) * 100
- Visualized churn by Region, Income Group, Channel 
  and Loyalty Tier
- Built Funnel Chart: Total → Repeat → Churned Customers

### Task 3 — Repeat Purchase Analysis
- Segmented customers: Low-Tier (0-3), Mid-Tier (4-8), 
  High-Tier (9+) purchases
- Compared avg purchase frequency by Region, Age Group 
  and Loyalty Tier
- Identified most purchased product categories by 
  loyal customers

### Task 4 — Promotion & Loyalty Impact
- Analyzed % of transactions with promotion applied
- Compared avg purchase amount with vs without promotions
- Measured churn rate across loyalty tiers
- Visualized Points Earned vs Redeemed by Tier
- Generated recommendations to improve redemption 
  and retention

### Task 5 — Store & Channel Performance
- Merged Store Locations with Transactions via Power Query
- Visualized avg transaction amount by Store Type
- Analyzed churn rate by Store Type
- Explored correlation between store opening year 
  and retention rate

### Task 6 — Customer Lifetime Value (CLV) Analysis
- Calculated CLV = Total Amount Spent / Membership 
  Duration (Years)
- Segmented customers into High CLV (above average) 
  and Low CLV (below average)
- Visualized CLV vs Days Since Last Purchase (Scatter)
- Analyzed CLV by Loyalty Tier and Region

### Task 7 — Final Dashboard & Executive Summary
- Built 4-page interactive Power BI Report:
  - Page 1: KPIs (Churn, CLV, Repeat Rate)
  - Page 2: Loyalty & Promotion Impact
  - Page 3: Store & Channel Insights
  - Page 4: Segmentation (Churned, Repeat, High-Value)
- Added Slicers: Region, Channel, Income, Loyalty Tier
- Delivered Top 3 Recommendations for Walmart

---

## Key Findings
- **49.7% churn rate** — nearly half of all customers lost
- **Elite tier** has highest churn (54.7%) despite being 
  top loyalty tier
- **Promotions show zero spend impact** — only $0.07 
  difference with vs without promotion
- **Sam's Club** is strongest store format — highest spend 
  ($534.45) and lowest churn (47.67%)
- **Basic tier** has lowest redemption rate (67.5%) — 
  most disengaged from loyalty program
- Only **26.7% of customers are High CLV** — majority 
  of value concentrated in small customer group

---

## Top 3 Recommendations
1. **Prioritize Elite tier for retention** — highest churn 
   (54.7%) and lowest CLV ($378). Launch personalized 
   re-engagement campaigns immediately
2. **Fix Online channel** — 54% churn rate, higher than 
   Store channel (46%). Implement personalized 
   recommendations and exclusive online loyalty rewards
3. **Redesign loyalty program for Basic tier** — send 
   points expiry notifications and introduce double value 
   redemption events to improve 67.5% redemption rate

---

## Tools & Technologies
- **Power BI Desktop** — Dashboard development
- **Power Query** — Data cleaning and transformation
- **DAX** — Calculated columns and measures
- **Python (pandas)** — Data validation and analysis
- **Excel** — Source data format

---

## Data Model Structure
