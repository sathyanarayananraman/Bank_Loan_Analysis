# 🏦 Bank Loan Analytics | Python • MySQL • Power BI

An end-to-end **Bank Loan Analytics** project focused on analyzing loan applications, loan quality, funding, repayment performance, customer characteristics, and portfolio trends using **Python, SQL, and Power BI**.

---

## 📌 Project Overview

The objective of this project is to analyze a bank's loan portfolio and transform raw loan data into meaningful business insights.

The project follows an end-to-end analytics workflow:

**Raw Dataset → Python Data Cleaning  → MySQL → Power BI → DAX → Interactive Dashboard → Business Insights**

The analysis focuses on understanding:

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

# 🎯 Business Objectives

The project aims to answer key business questions related to the bank's lending portfolio:

1. How many loan applications were received?
2. What is the total amount funded?
3. How much amount has been received?
4. What percentage of loans are classified as Good vs Bad?
5. How does loan performance vary by loan status?
6. Which loan purposes have the highest application volume?
7. Which loan term is most common?
8. How are loan applications distributed by home ownership?
9. How does loan application volume change over time?
10. What are the average interest rate and DTI ratio?
11. How do funded and received amounts vary across loan statuses?
12. How loan grades impacts the Rate Of Interest?

---

# 📊 Dataset

### Source

The dataset was obtained from **Kaggle**.

### Dataset Information

| Attribute | Details |
|---|---|
| Domain | Banking / Financial Services |
| Geography | United States |
| Rows | 38,576 |
| Columns | 14 |
| Data Type | Bank Loan Data |

The dataset contains information related to loan applications, loan status, funded amounts, amounts received, interest rates, DTI ratios, loan purposes, home ownership, loan terms, and other loan-related attributes.

---

# 🛠️ Tools & Technologies

| Technology | Purpose |
|---|---|
| 🐍 Python | Data cleaning  |
| 🐼 Pandas | Data manipulation and analysis |
| 🐬 MySQL | Data storage |
| 🔗 SQLAlchemy | Loading cleaned data into MySQL |
| 📊 Power BI | Data modeling and visualization |
| 📐 DAX | Business calculations and measures |

---

# 🔄 Project Workflow

```text
              Raw Kaggle Dataset csv file
                       │
                       ▼
              Python Data Cleaning
                       │
                       ▼
          Load Cleaned Data into MySQL
              using SQLAlchemy
                       │
                       ▼
                  SQL / MySQL
                       │
                       ▼
             Connect MySQL to Power BI
                       │
                       ▼
             Power BI Data Modeling
                       │
                       ▼
               DAX Calculations
                       │
                       ▼
              Interactive Dashboard
                       │
                       ▼
                Business Insights
```
 1. Python Data Cleaning & EDA

Python was used as the initial data preparation and analysis layer.

Data Cleaning: 
The cleaning process included:

-Checking for missing values,
-Checking for duplicate records,
-Standardizing column names,
-Preparing the dataset for further analysis,
-Python and Pandas were used for data manipulation and analysis.

2. MySQL & SQL

- After cleaning the dataset in Python
- the data was loaded into MySQL using SQLAlchemy.
- MySQL was used as the database layer before connecting the data to Power BI.

Workflow
Python ➡ Cleaned Dataset ➡ SQLAlchemy ➡ MySQL ➡ Power BI

This created a structured workflow between data preparation, database storage, and business intelligence reporting.

3. Power BI

The MySQL data was connected to Power BI for visualization and further analysis.

The Power BI solution contains two main dashboard pages:

Page 1 — Overview

The Overview page provides a high-level view of the loan portfolio.

It includes:

- Total Loan Applications
- Total Funded Amount
- Total Amount Received
- Average Interest Rate
- Average DTI Ratio
- Monthly Loan Applications
- Loan Applications by State
- Loan Applications by Term
- Loan Applications by Home Ownership
- Loan Applications by Loan Purpose

Page 2 — Summary
The Summary page focuses on loan quality and portfolio performance.

It includes:

- Good vs Bad Loan Applications
- Good vs Bad Loan Funded Amount
- Good vs Bad Loan Amount Received
- Loan Status
- Average Interest Rate by Loan Status
- Average DTI by Loan Status

4. Power BI Data Modeling & DAX

Power BI was used for data modeling and business calculations.

The project includes:

-Calculated columns
-Conditional loan classification
-DAX measures
-KPI calculations
-Good Loan analysis
-Bad Loan analysis
-Good vs Bad Loan Classification

Loans were classified into:

-Good Loan
-Bad Loan

This classification was then used to analyze loan applications, funded amounts, and amounts received.

Key Metrics

The dashboard includes calculations for:

1.  Total Loan Applications
2.  Total Funded Amount
3.  Total Amount Received
4.  Good Loan Applications
5.  Bad Loan Applications
6.  Good Loan %
7.  Bad Loan %
8.  Good Loan Funded Amount
9.  Bad Loan Funded Amount
10. Good Loan Amount Received
11. Bad Loan Amount Received
12. Average Interest Rate
13. Average DTI Ratio

--- 

📈 Dashboard
Overview Dashboard

The Overview dashboard provides a consolidated view of the bank's lending activity.

It allows users to analyze loan applications across different dimensions such as:

-Time
-State
-Loan term
-Home ownership
-Loan purpose

The dashboard also provides key portfolio-level KPIs.

---

Summary Dashboard

The Summary dashboard focuses on loan quality and financial performance.

It compares:

1. Good Loans vs Bad Loans
2. Funded Amount vs Amount Received
3. Loan Status
4. Interest Rate
5. DTI Ratio

This provides a more detailed view of the portfolio's performance.

---

🔍 Key Insights
1. Overall Loan Portfolio

-The dataset contains: 38,576 loan applications

-The total funded amount is approximately: $435.8M

-The total amount received is approximately: $473.1M

-The portfolio has an average interest rate of: 12.05%

-The average DTI ratio is: 13.33%

--- 

2. Good vs Bad Loans

The portfolio contains:

  |Loan Category  |	Applications   |	Percentage |
  |Good Loans	   |  33,243	      |86.18%       |
  |Bad Loans	   |  5,333	         |13.82%       |
  |Total	         |  38,576	      |100%         |

 Good Loans
-  Applications: 33,243
-  Percentage: 86.18%
-  Funded Amount: $370.2M
-  Amount Received: $435.8M

 Bad Loans
-  Applications: 5,333
-  Percentage: 13.82%
-  Funded Amount: $65.5M
-  Amount Received: $37.3M

The Good vs Bad loan analysis provides an important view of the portfolio's loan quality and financial performance.

---

📅 3. Monthly Loan Application Trend

Loan application volume increased over the year represented in the dataset.

Approximate monthly applications ranged from: January: ~2.3K  to December: ~4.3K

This provides a view of how loan application activity changed throughout the year.

---

⏳ 4. Loan Term Distribution

The majority of loan applications were associated with a 36-month term.

| Loan Term |	Applications |	Percentage |
|36 Months  |	~28K	       |    73.2%   |
|60 Months	|  ~10K	       |    26.8%   |

The 36-month loan term represents the larger share of applications in the dataset.

---

🏠 5. Home Ownership

Loan applications were concentrated among customers who either rent or have a mortgage.

-Home Ownership	Applications
-Rent	18,439 
-Mortgage	17,198 
-Own	2,838 
-Other	98 
-None	3

Rent and mortgage categories account for the majority of loan applications.

---

💳 6. Loan Purpose

Debt Consolidation represents the largest loan-purpose category in the dataset.

Other loan purposes include:

-  Credit Card
-  Other
-  Home Improvement
-  Major Purchase
-  Small Business
-  Car
-  Medical
-  Moving
-  Wedding
-  Vacation

This allows the bank's lending portfolio to be analyzed based on the intended purpose of borrowing.

---

📋 7. Loan Status Analysis

The dashboard analyzes loan performance across different loan statuses, including:

-Fully Paid  
-Charged Off  
-Current  

The analysis compares funded amounts and amounts received across these loan statuses.

-Fully Paid
   -Funded Amount: approximately $351.4M
   -Amount Received: approximately $411.6M
-Charged Off
   -Funded Amount: approximately $65.5M
   -Amount Received: approximately $37.3M
-Current
   -Funded Amount: approximately $18.9M
   -Amount Received: approximately $24.2M

 ---

📊 8. Interest Rate by Loan Status

The dashboard compares average interest rates across loan statuses.

|Loan Status | 	Average Interest Rate |
|Current	    |    15.10%                |
|Charged Off | 	13.88%                |
|Fully Paid	 |    11.64%                |

This provides a descriptive comparison of interest rates across different loan statuses.

---

📊 9. DTI Ratio by Loan Status

The dashboard also compares average DTI ratios across loan statuses.

|Loan Status	|  Average DTI |
|Current	      |  14.72%      |
|Charged Off	|  14.00%      |
|Fully Paid	   |  13.17%      |

These values provide a descriptive view of DTI across different loan-status groups.

---

💡 Business Takeaways

The analysis provides several useful views of the lending portfolio:

-The dataset contains 38,576 loan applications.
-Approximately 86.18% of applications are classified as Good Loans.
-Approximately 13.82% are classified as Bad Loans.
-The portfolio contains approximately $435.8M in funded loans.
-The total amount received is approximately $473.1M.
-Loan application activity increased during the year represented by the dataset.
-36-month loans account for the majority of applications.
-Rent and Mortgage are the largest home ownership categories.
-Debt Consolidation is the largest loan-purpose category.
-Loan status can be analyzed alongside funded amount, amount received, interest rate, and DTI.

---

📁 Repository Structure
Bank_Loan_Analysis/
│
├── output/
│   └── Analysis outputs
│
├── power_bi_file/
│   └── Power BI dashboard files
│
├── source-files/
│   └── Project source files
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
   -Pandas
   -Data Manipulation
-SQL & Database
   -MySQL
   -SQLAlchemy
   -Database Integration
   -Business Intelligence
-Power BI
   -DAX
   -Data Modeling
   -Dashboard Development
   -Data Visualization

---

🚀 Future Improvements

The project can be extended with additional analytics and data engineering capabilities, including:

-Automated data ingestion
-Automated ETL pipelines
-Additional loan risk metrics
-Customer segmentation
-Loan default prediction
-Advanced SQL analysis
-Automated Power BI data refresh
-Integration with additional financial datasets
-Machine learning-based loan risk analysis
