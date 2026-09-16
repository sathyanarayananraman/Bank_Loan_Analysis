# 🏦 Bank Loan Analytics

### Python | SQL | MySQL | Power BI | DAX

An end-to-end **Bank Loan Analytics** project focused on analyzing loan applications, loan quality, funding, repayment performance, customer characteristics, and portfolio trends.

---

## 📌 Project Overview

The objective of this project is to analyze a bank's loan portfolio and transform raw loan data into meaningful business insights.

The project follows an end-to-end analytics workflow:

**Raw Dataset → Python Data Cleaning → MySQL → Power BI → DAX → Interactive Dashboard → Business Insights**

The analysis focuses on:

- Loan application trends
- Good vs Bad loan performance
- Funded amount
- Amount received
- Loan status
- Loan terms
- Home ownership
- Loan purposes
- Interest rates
- Debt-to-income (DTI) ratio
- Overall loan portfolio performance

---

## 🎯 Business Objectives

The project aims to answer the following business questions:

1. How many loan applications were received?
2. What is the total amount funded?
3. What is the total amount received?
4. What percentage of loans are classified as Good vs Bad?
5. How does loan performance vary by loan status?
6. Which loan purposes have the highest application volume?
7. Which loan term is most common?
8. How are loan applications distributed by home ownership?
9. How does loan application volume change over time?
10. What are the average interest rate and DTI ratio?
11. How do funded and received amounts vary across loan statuses?
12. How does loan grade impact the rate of interest?

---

## 📊 Dataset

### Source

The dataset was obtained from **Kaggle**.

### Dataset Information

| Attribute | Details |
|-----------|---------|
| Domain | Banking / Financial Services |
| Geography | United States |
| Rows | 38,576 |
| Columns | 14 |
| Data Type | Bank Loan Data |

The dataset contains information related to loan applications, loan status, funded amounts, amounts received, interest rates, DTI ratios, loan purposes, home ownership, loan terms, and other loan-related attributes.

---

## 🛠️ Tools & Technologies

| Technology | Purpose |
|------------|---------|
| Python | Data cleaning and analysis |
| Pandas | Data manipulation and analysis |
| SQL | Database analysis |
| MySQL | Data storage |
| SQLAlchemy | Loading cleaned data into MySQL |
| Power BI | Data modeling and visualization |
| DAX | Business calculations and measures |

---

## 🔄 Project Workflow

```text
Raw Kaggle Dataset
        ↓
Python Data Cleaning
        ↓
Exploratory Data Analysis
        ↓
Load Cleaned Data into MySQL
        ↓
SQL / MySQL
        ↓
Connect MySQL to Power BI
        ↓
Power BI Data Modeling
        ↓
DAX Calculations
        ↓
Interactive Dashboard
        ↓
Business Insights

---

Insights

🐍 1. Python Data Cleaning & EDA

Python was used as the initial data preparation and analysis layer.

Data Cleaning

The cleaning process included:
-Checking for missing values
-Checking for duplicate records
-Standardizing column names
-Preparing the dataset for further analysis

Python and Pandas were used for data manipulation and analysis.

---

🗄️ 2. MySQL & SQL

After cleaning the dataset in Python, the data was loaded into MySQL using SQLAlchemy.

MySQL was used as the database layer before connecting the data to Power BI.

Data Flow

Python
   ↓
Cleaned Dataset
   ↓
SQLAlchemy
   ↓
MySQL
   ↓
Power BI

This created a structured workflow between data preparation, database storage, and business intelligence reporting.

---

📊 3. Power BI Dashboard

The MySQL data was connected to Power BI for visualization and further analysis.

The Power BI solution contains two main dashboard pages.

📈 Page 1 — Overview

The Overview page provides a high-level view of the loan portfolio.

-Key Performance Indicators
-Total Loan Applications
-Total Funded Amount
-Total Amount Received
-Average Interest Rate
-Average DTI Ratio
-Analysis
-Monthly Loan Applications
-Loan Applications by State
-Loan Applications by Term
-Loan Applications by Home Ownership
-Loan Applications by Loan Purpose

📋 Page 2 — Summary

The Summary page focuses on loan quality and portfolio performance.

Analysis
-Good vs Bad Loan Applications
-Good vs Bad Loan Funded Amount
-Good vs Bad Loan Amount Received
-Loan Status
-Average Interest Rate by Loan Status
-Average DTI by Loan Status

---

📐 4. Power BI Data Modeling & DAX

Power BI was used for data modeling and business calculations.

The project includes:

-Calculated columns
-Conditional loan classification
-DAX measures
-KPI calculations
-Good Loan analysis
-Bad Loan analysis
-Good vs Bad Loan Classification

Loans were classified into two categories:

Good Loan
Bad Loan

This classification was used to analyze:

-Loan applications
-Funded amounts
-Amount received
-Key Metrics

The dashboard includes calculations for:

-Total Loan Applications
-Total Funded Amount
-Total Amount Received
-Good Loan Applications
-Bad Loan Applications
-Good Loan %
-Bad Loan %
-Good Loan Funded Amount
-Bad Loan Funded Amount
-Good Loan Amount Received
-Bad Loan Amount Received
-Average Interest Rate
-Average DTI Ratio

---
📈 Dashboard
Overview Dashboard

The Overview dashboard provides a consolidated view of the bank's lending activity.

It allows users to analyze loan applications across different dimensions:

Time
State
Loan Term
Home Ownership
Loan Purpose

The dashboard also provides key portfolio-level KPIs.
---
Summary Dashboard

The Summary dashboard focuses on loan quality and financial performance.

It compares:

Good Loans vs Bad Loans
Funded Amount vs Amount Received
Loan Status
Interest Rate
DTI Ratio

This provides a more detailed view of the portfolio's performance.

---

🔍 Key Insights

1. Overall Loan Portfolio
   KPI	                           Value
   Total Loan Applications    	      38,576
   otal Funded Amount	              $435.8M
   Total Amount Received	          $473.1M
   Average Interest Rate	           12.05%
   Average DTI Ratio	               13.33%
     ---

2. Good vs Bad Loans
   Loan Category	   Applications	   Percentage
   Good Loans	      33,243	         86.18%
   Bad Loans	      5,333       	   13.82%
   Total	            38,576      	   100%

Good Loans

   Metric	            Value
   Applications	      33,243
   Percentage	         86.18%
   Funded Amount	      $370.2M
   Amount Received	   $435.8M

Bad Loans
   Metric	            Value
   Applications	      5,333
   Percentage	         13.82%
   Funded Amount	      $65.5M
   Amount Received	   $37.3M

The Good vs Bad loan analysis provides a view of loan quality and financial performance within the portfolio.

---

3. Monthly Loan Application Trend

Loan application volume increased over the year represented in the dataset.

Period	   Applications
January	   ~2.3K
December	   ~4.3K

This provides a view of changes in loan application activity throughout the year.
---
4. Loan Term Distribution

The majority of loan applications were associated with a 36-month term.

Loan Term	   Applications	Percentage
36 Months	   ~28K	         73.2%
60 Months	   ~10K	         26.8%
---
5. Home Ownership

Rent	      18,439
Mortgage	   17,198
Own	      2,838
Other	      98
None	      3

Rent and mortgage categories account for the majority of loan applications.
---
6. Loan Purpose

Debt Consolidation represents the largest loan-purpose category in the dataset.

Other loan purposes include:

   -Credit Card
   -Other
   -Home Improvement
   -Major Purchase
   -Small Business
   -Car
   -Medical
   -Moving
   -Wedding
   -Vacation

This allows the bank's lending portfolio to be analyzed based on the intended purpose of borrowing.
---
7. Loan Status Analysis

The dashboard analyzes loan performance across the following loan statuses:

Fully Paid
Charged Off
Current
Funded Amount vs Amount Received

Loan Status	   Funded Amount	   Amount Received
Fully Paid	   ~$351.4M	         ~$411.6M
Charged Off	   ~$65.5M	         ~$37.3M
Current	      ~$18.9M	         ~$24.2M

---
8. Average Interest Rate by Loan Status
Loan Status	   Average Interest Rate
Current	         15.10%
Charged Off	      13.88%
Fully Paid	      11.64%

This provides a descriptive comparison of average interest rates across loan statuses.
---
9. Average DTI by Loan Status
Loan Status	   Average DTI
Current	      14.72%
Charged Off	   14.00%
Fully Paid	   13.17%

This provides a descriptive comparison of average DTI across loan statuses.
---
💡 Business Takeaways

The analysis provides several useful views of the lending portfolio:

   -The dataset contains 38,576 loan applications.
   -86.18% of applications are classified as Good Loans.
   -13.82% of applications are classified as Bad Loans.
   -The total funded amount is approximately $435.8M.
   -The total amount received is approximately $473.1M.
   -Loan application activity increased during the year represented in the dataset.
   -36-month loans account for the majority of applications.
   -Rent and Mortgage are the largest home ownership categories.
   -Debt Consolidation is the largest loan-purpose category.
   -Loan status can be analyzed alongside funded amount, amount received, interest rate, and DTI.

---
📁 Repository Structure
Bank_Loan_Analysis/
│
├── output/
│
├── power_bi_file/
│
├── source-files/
│
└── README.md
---
🎯 Skills Demonstrated

   -Data Analytics
   -Data Cleaning
   -Data Preparation
   -Business Analysis
   -KPI Development
   -Financial Data Analysis
   -Python
      Pandas
      Data Manipulation
   -SQL & Database
      MySQL
      SQLAlchemy
      Database Integration
      Business Intelligence
   -Power BI
      DAX
      Data Modeling
      Dashboard Development
      Data Visualization
