# Procurement Spend and Budget Variance Analysis
## 🎯 Problem Statement
XYZ Tech is currently facing a ₱9.34M overspend, representing a 13.6% variance over the approved budget. This analysis investigates the drivers of overspending across departments and fiscal years and identifies areas where management can improve spending control and accountability.

## 📈 Data
Source: Simulated 3-year enterprise procurement dataset covering 2023–2025
Transaction Data: Cleaned and validated approved procurement transactions from ERP_Cleaned
Budget Data: Department-level approved budgets from Dim_Budgets
Key variables: Fiscal Year, Department, Expense Category, Raw Amount, Approval Status, Vendor, and Transaction Date
Final approved expenditure: ₱78.06M
Approved budget: ₱68.72M

## 🛠️ Tools & Methodology
### 1️⃣ Python — Data Cleaning & Preparation
Standardized transaction dates and monetary values
Removed duplicate records
Standardized department names and expense categories
Classified missing department values as Unassigned
Prepared the cleaned transaction dataset for Power BI analysis

<p align="center">
 <img width="1278" height="1230" alt="data cleaning_procurement spend analysis_python" src="https://github.com/user-attachments/assets/74105d2d-a729-4ca2-a32d-656f70611086" />
</p>

### 2️⃣ Power BI — Data Modeling & Dashboard
Built a relationship between budget and transaction data using a Year + Department composite key
Created DAX measures for:
Approved Budget
Total Expenditure
Total Variance
Overspend Total
Variance % of Total Overspend
Developed an interactive executive dashboard with department and fiscal-year filters
Added a Clear Filters control for dashboard navigation

## 📊 Dashboard

Budget and Expenditure Analysis Dashboard

<p align="center">
<img width="1352" height="767" alt="image" src="https://github.com/user-attachments/assets/50cf5ede-ad25-4a87-9a25-73852fbc6cbb" />
</p>

The dashboard provides an executive-level view of budget performance, expenditure trends, departmental overspending, and expense-category composition.

Key Dashboard Views
Approved Budget vs Total Expenditure by Department
Actual Spend vs Budget Timeline
Budget Allocation by Department
Department Expenditure by Expense Category

## 💡 Key Insights
1. Overall Budget Overspend
- Approved expenditure reached ₱78.06M against an approved budget of ₱68.72M, resulting in a ₱9.34M overall variance or 13.6% over budget and a overspend total of ₱13.1M.
<p align="center">
<img width="1514" height="109" alt="image" src="https://github.com/user-attachments/assets/0e67d89f-7502-4d1a-9e9b-c9b47bf73eb2" />
</p>

2. Overspending is concentrated
- The largest departmental expenditure pressures are concentrated in **Facilities & Ops and Marketing & Sales**, making these departments the primary areas for cost-control investigation. Further, approximately ₱2.96M of approved expenditure is classified as Unassigned, meaning the transactions cannot currently be attributed to a department.

<p align="center">
<img width="633" height="409" alt="image" src="https://github.com/user-attachments/assets/8b629955-a33a-4758-90ac-ca1577c42079" />
</p>

- HR & Admin spent approximately ₱9.55M against a ₱13.04M budget, indicating substantial unused budget capacity compared with other departments.

3. 2024 was the highest-spending year
- Total expenditure peaked in 2024 at approximately ₱28.45M, compared with an approved budget of approximately ₱22.88M.
<p align="center">
<img width="613" height="408" alt="image" src="https://github.com/user-attachments/assets/401be3a1-6371-448c-b663-ac32f494f3a2" />
</p>

4. Major cost categories
- Hardware Procurement and Software Licenses are the two highest-spending expense categories across the three-year period.
- Office Supplies and Digital Advertising are the next largest contributors to overall expenditure.
- The concentration of spending in these categories suggests opportunities to review vendor pricing, purchasing volumes, recurring contracts, and procurement controls.
- Hardware Procurement is particularly worth investigating because it represents the largest overall category spend and may offer opportunities for bulk purchasing, vendor consolidation, or contract renegotiation.
<p align="center">
<img width="1710" height="354" alt="image" src="https://github.com/user-attachments/assets/a49f7922-e00e-4c97-a698-938125dd9926" />
</p>

## 🚀 Strategic Recommendations
1. Prioritize cost controls in high-overspend departments

Focus procurement reviews on Facilities & Ops and Marketing & Sales rather than applying uniform cuts across all departments.

2. Investigate the 2024 spending spike

Review the transactions, vendors, and expense categories behind the 2024 increase to determine whether the spike resulted from one-time purchases, project requirements, or procurement-control issues.

3. Eliminate Unassigned expenditure

Make department classification mandatory for financial transactions to improve budget accountability and reporting accuracy.

4. Review major expense categories

Analyze high-spend categories such as Hardware Procurement and Software Licenses for opportunities involving vendor negotiations, consolidation, or purchasing controls.
