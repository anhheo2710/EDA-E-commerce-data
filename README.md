# 📊 EDA on E-commerce Transaction Data

##  Introduction
This project analyzes a transnational transactional dataset from a UK-based online retail company.  
The goal is to **understand customer behavior** and **segment customers** based on their purchasing patterns.

---

##  Data Source
- Dataset: `data/transaction_data.csv`  
- Contains transaction records from Dec 2010 to Dec 2011  

---

##  Data Cleaning
Steps performed:
- Removed missing/null values  
- Converted negative quantities & unit prices → positive values  
- Created `amount = quantity × unit_price`  
- Extracted time-based features: **month, day, hour, year_month, weekday**

---

##  Exploratory Data Analysis (EDA)
Explored various aspects of customer behavior:
-  Monthly Active Users (MAU) over time  
-  Order counts & revenue trends  
-  Customer activity by weekdays & hours  
-  Top 10 countries by sales & countries with highest Average Order Value (AOV)  
-  New vs. returning customer analysis  
-  Average transaction value of new customers over time  

---

##  Customer Segmentation
Segmentation using **RF (Recency & Frequency) model**:
- **Recency:** Days since last transaction  
- **Frequency:** Number of unique invoices per customer  

Customer groups:
- Loyal  
- Potential Loyal  
- New Customer  
- Losing Loyal  
- Lost Loyal  
- Losing Potential Loyal  
- Low Value  

---

##  Results & Insights
-  **Monthly active users & sales** increased steadily (esp. after Aug 2011)  
-  **UK** = largest revenue, 🇸🇬 **Singapore** = highest AOV  
-  Peak transactions between **10 AM – 3 PM** (lunch hours peak)  
-  Strong **customer retention rate**  
-  **Loyal & Potential Loyal customers** contribute the most to revenue  

---
