# Bank-Loan-Customer-Analysis
Bank Loan Customer Analytics project using SQL, Python, Tableau, and Power BI to analyze loan trends, customer behavior, payment patterns, loan status, and home ownership.
# 🏦 Bank Loan Customer Analytics

## 📌 Project Overview

This project focuses on analyzing bank loan customer data to understand loan trends, customer behavior, payment patterns, loan status, credit grades, and home ownership.

The project uses **SQL, Python, Tableau, and Power BI** to perform data analysis and create meaningful business insights.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze year-wise loan amount statistics
- Analyze grade and sub-grade wise revolving balance
- Compare total payments between verified and non-verified customers
- Analyze state-wise and month-wise loan status
- Analyze home ownership and last payment date statistics
- Create interactive dashboards using Tableau and Power BI
- Perform data analysis using Python
- Perform SQL-based business analysis

---

## 📊 Dataset Information

### Domain
**Finance / Banking**

### Project
**Bank Loan Customer Analytics**

### Datasets

- `Finance_1_cleaned.csv`
- `Finance_2_cleaned.csv`

Both datasets contain bank loan and customer-related information.

The datasets are connected using the common **ID** column.

### Dataset Size

- Approximately **39K+ records**
- Multiple customer, loan, payment, and credit-related attributes

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| 🐍 Python | Data cleaning, analysis and visualization |
| 🗄️ SQL / MySQL | Data querying and business analysis |
| 📊 Tableau | Interactive data visualization |
| 📈 Power BI | Interactive dashboard and KPI analysis |
| 📁 Excel / CSV | Dataset storage and preparation |
| 🐙 GitHub | Project documentation and portfolio |

---

# 🔍 Business Questions / KPIs

The project answers the following five major business questions:

### 1️⃣ Year-wise Loan Amount Statistics

Analyze loan amounts across different years.

**Metrics:**
- Total Loan Amount
- Number of Loans
- Average Loan Amount

---

### 2️⃣ Grade & Sub-Grade Wise Revolving Balance

Analyze revolving balance based on customer credit grade and sub-grade.

**Metrics:**
- Total Revolving Balance
- Average Revolving Balance
- Grade
- Sub-Grade

---

### 3️⃣ Verified vs Non-Verified Total Payment

Compare the total payment made by customers based on their verification status.

**Categories:**
- Verified
- Not Verified
- Source Verified

**Metrics:**
- Total Payment
- Average Payment
- Number of Loans

---

### 4️⃣ State-wise & Month-wise Loan Status

Analyze loan status based on customer state and loan issue month.

**Analysis includes:**
- State
- Month
- Loan Status
- Number of Loans
- Total Loan Amount

---

### 5️⃣ Home Ownership vs Last Payment Date

Analyze loan payment behavior based on home ownership.

**Categories include:**
- RENT
- MORTGAGE
- OWN
- OTHER

**Metrics:**
- Number of Loans
- Total Payment
- Average Payment
- Latest Payment Date

---

# 🗄️ SQL Analysis

SQL was used to query the loan data and answer the major business questions.

### SQL Tasks

- Calculate total loan amount by year
- Calculate revolving balance by grade and sub-grade
- Compare payment amounts by verification status
- Analyze loan status by state and month
- Analyze payment behavior by home ownership
- Calculate aggregate and average metrics
- Group and sort financial data

---

#🐍 **Python Analysis**
Python was used for data preparation, exploratory data analysis, aggregation, and visualization.

Python Libraries
import pandas as pd
import matplotlib.pyplot as plt

**Python Workflow**
-Load the datasets
-Check dataset structure
-Check missing values
-Check duplicate records
-Convert data types
-Merge datasets using id
-Perform exploratory data analysis
-Calculate KPIs
-Create visualizations
-Generate business insights

Dataset Merge
df = pd.merge(finance1,finance2,on="id",how="inner")

Example Analysis
year_analysis = df.groupby(
    df["issue_d"].dt.year
).agg(
    total_loans=("id", "count"),
    total_loan_amount=("loan_amnt", "sum"),
    average_loan_amount=("loan_amnt", "mean")
).reset_index()

---

📊** Tableau Dashboard**
Tableau was used to create interactive dashboards for exploring loan and customer data.
Tableau Analysis
The Tableau dashboard includes:
📈 Year-wise Loan Amount
📊 Grade & Sub-Grade Revolving Balance
💰 Verified vs Non-Verified Total Payment
🗺️ State-wise Loan Status
📅 Month-wise Loan Status
🏠 Home Ownership Analysis
💳 Payment Analysis
kjiuytiu
**Tableau Dashboard**
"C:\Users\Pooja\Documents\GitHub\Bank_Loan_Analysis\tableau dashboard.png"

---

📈 Power BI Dashboard
Power BI was used to create an interactive financial analytics dashboard.

Power BI KPIs
-The dashboard includes:
-Total Loans
-Total Loan Amount
-Total Payment
-Average Loan Amount
-Total Revolving Balance
-Power BI Visualizations
-Year-wise loan amount trend
-Grade and sub-grade revolving balance
-Verified vs non-verified payment comparison
-State-wise loan status
-Month-wise loan status
-Home ownership analysis
-Last payment date analysis

**Power BI Dashboard**
1.Year wise loan amount status:
"C:\Users\Pooja\Documents\GitHub\Bank_Loan_Analysis\Year wise loan amnt stats PBI 1.png"

2.Grade & sub grade wise revoling balance:
"C:\Users\Pooja\Documents\GitHub\Bank_Loan_Analysis\Grade sub grade wise revol bal PBI 2.png"

3.Verification payment analysis:
"C:\Users\Pooja\Documents\GitHub\Bank_Loan_Analysis\Verification payment analysis PBI 3.png"

4.State and month wise loan status:
"C:\Users\Pooja\Documents\GitHub\Bank_Loan_Analysis\State and month wise loan status PBI 4.png"

5.Home ownership and payment:
"C:\Users\Pooja\Documents\GitHub\Bank_Loan_Analysis\Home ownership and payment PBI 5.png"


🔗 Data Relationship
The two datasets are connected using the common id column.
Finance_1
   |
   | id
   |
   ↓
Finance_2
This allows loan, customer, and payment information to be analyzed together.
📁 Project Structure
Bank-Loan-Customer-Analytics/
│
├── 📁 data/
│   ├── Finance_1_cleaned.csv
│   └── Finance_2_cleaned.csv
│
├── 📁 sql/
│   └── bank_loan_analysis.sql
│
├── 📁 python/
│   └── bank_loan_analysis.ipynb
│
├── 📁 tableau/
│   └── Bank_Loan_Dashboard.twbx
│
├── 📁 powerbi/
│   └── Bank_Loan_Dashboard.pbix
│
├── 📁 screenshots/
│   ├── tableau_dashboard.png
│   ├── powerbi_dashboard.png
│   └── python_analysis.png
│
└── 📄 README.md
📌 Key Insights
The analysis helps identify:
Loan amount trends across different years
Credit grades with higher revolving balances
Payment differences between verified and non-verified customers
States with different loan status patterns
Monthly loan activity
Payment behavior across home ownership categories

💡 Business Value
This analysis can help financial institutions:
Understand loan demand trends
Monitor customer payment behavior
Identify high-risk and low-risk customer segments
Analyze credit grade performance
Understand geographical loan patterns
Improve lending and customer strategies
Support data-driven financial decision making

🚀 Skills Demonstrated
Technical Skills
-SQL
-MySQL
-Python
-Pandas
-Matplotlib
-Tableau
-Power BI
-DAX
-Data Cleaning
-Data Visualization
-Exploratory Data Analysis
-KPI Development
-Business Analysis
-Analytical Skills
-Data preprocessing
-Data aggregation
-Trend analysis
-Customer segmentation
-Financial analysis
-Dashboard development
-Business insight generation

---

📝 Conclusion
This Bank Loan Customer Analytics project demonstrates the use of SQL, Python, Tableau, and Power BI to analyze financial data and generate meaningful business insights. The analysis explores year-wise loan trends, credit grades, customer verification status, state-wise loan performance, and home ownership patterns. By combining data analysis with interactive dashboards, this project helps transform raw financial data into actionable insights that support better decision-making. Overall, this project enhanced my skills in data cleaning, SQL querying, Python analysis, data visualization, dashboard development, and business analytics.
