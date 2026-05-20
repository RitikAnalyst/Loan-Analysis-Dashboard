# Loan Analysis Dashboard — Power BI
A multi-page interactive Power BI dashboard analyzing loan application data across approval 
trends, applicant demographics, credit risk, loan financials, and income patterns.--
## Project Overview
This dashboard explores a cleaned loan dataset (`Loan_Clean`) to help stakeholders understand 
what drives loan approvals, who is applying, and where financial risk is concentrated. It is 
built as a portfolio project demonstrating end-to-end Power BI skills: data modeling, DAX 
measures, visual design, and interactive filtering.--
## Dashboard Pages
### Page 1 — Overview
High-level summary of loan applications.- KPI cards: Total Applications, Avg Credit Score- Approval Rate % by month (line chart)- Avg Annual Income trend- Loan applications by purpose (clustered bar)- Approval vs. Rejection distribution (donut chart)- Slicers: Year, Employment Status, Approval Status
### Page 2 — Applicant Demographics
Who is applying for loans?- Applications by Age Group- Applications by Education Level- Applications by Employment Status- Home Ownership Status breakdown (donut)- Applications by Marital Status- Slicers: Year, Employment Status, Approval Status
### Page 3 — Credit Risk Analysis
Where does risk concentrate?- Approval Rate % by Credit Band (bar chart)- Credit Score vs. Risk Score scatter plot- KPI cards: Avg Risk Score, High Risk Count- Bankruptcy History vs. Total Approved (bar chart)- Slicers: Year, Employment Status, Approval Status
### Page 4 — Loan Financials
Loan size and interest breakdown.- Avg Loan Amount by Loan Purpose- Avg Interest Rate % by Credit Band- Loan Amount vs. Monthly Payment scatter plot- KPI cards: Total Loan Amount, Avg Loan Amount- Slicers: Year, Employment Status, Approval Status
### Page 5 — Income & Financial Health
Applicant financial standing.- Avg Annual Income by Education Level- Net Worth by Home Ownership Status- Annual Income vs. Credit Score scatter plot- Debt-to-Income Ratio by Income Band- Previous Loan Defaults vs. Approval Rate %- Slicers: Year, Employment Status, Approval Status
### Page 6 — Summary / Notes--
## DAX Measures
| Measure | Description |
|---|---|
| `Total Applications` | Count of all loan applications |
| `Total Approved` | Count of approved applications |
| `Approval Rate %` | Approved / Total Applications × 100 |
| `Avg Credit Score` | Average applicant credit score |
| `Avg Annual Income` | Average applicant annual income |
| `Avg Loan Amount` | Average requested loan amount |
| `Avg Interest Rate %` | Average interest rate across loans |
| `Avg Risk Score` | Average risk score |
| `High Risk Count` | Count of high-risk applicants |
| `Total Loan Amount` | Sum of all loan amounts |--
## Data Model
**Main Table:** `Loan_Clean`
Key columns used across visuals:
| Column | Type | Description |
|---|---|---|
| `ApprovalStatus` | Text | Approved / Rejected |
| `LoanPurpose` | Text | Reason for loan |
| `EmploymentStatus` | Text | Employment type |
| `EducationLevel` | Text | Highest education |
| `HomeOwnershipStatus` | Text | Own / Rent / Other |
| `MaritalStatus` | Text | Marital category |
| `AgeGroup` | Text | Age band (derived) |
| `CreditBand` | Text | Credit score band (derived) |
| `IncomeBand` | Text | Income range band (derived) |
| `CreditScore` | Number | Raw credit score |
| `RiskScore` | Number | Risk score |
| `AnnualIncome` | Number | Annual income |
| `LoanAmount` | Number | Requested loan amount |
| `MonthlyLoanPayment` | Number | Monthly repayment amount |
| `NetWorth` | Number | Applicant net worth |
| `DebtToIncomeRatio` | Number | Debt-to-income ratio |
| `BankruptcyHistory` | Number | Bankruptcy flag |
| `PreviousLoanDefaults` | Number | Number of past defaults |
| `Age` | Number | Applicant age |
**Supporting Table:** `DateTable`- Used for time-based filtering (Year, MonthName)--
## Tools & Technologies- **Power BI Desktop** — Report development- **DAX** — Custom measures and KPIs- **Power Query** — Data cleaning (`Loan_Clean` table)- **Theme:** New Executive--
## How to Open
1. Download `Loan_Analysis_Dashboard.pbix`
2. Open with **Power BI Desktop** (free download from Microsoft)
3. Use the slicers on each page to filter by Year, Employment Status, and Approval Status--
## Author
**Raj** — Aspiring Data Analyst  
GitHub: [github.com/RitikAnalyst](https://github.com/RitikAnalyst)--
## Related Projects- [Superstore Sales Analysis](https://github.com/RitikAnalyst) — Python / Pandas / Matplotlib- Olist [E-commerce SQL Analysis](https://github.com/RitikAnalyst) — PostgreSQL
