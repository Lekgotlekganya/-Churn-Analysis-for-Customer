📉 Customer Churn Analysis — Data Analytics Internship Task 2

📌 Project Overview
This project was completed as part of a real-world Data Analytics Internship Task 2. The goal was to analyze customer subscription data to understand why customers leave and what keeps them engaged — just like a data analyst would for a real SaaS or telecom company.
The analysis answers key business questions such as:

Why are customers leaving the platform?
Which customer segments are most likely to churn?
How long do customers typically stay active?
What actions can improve customer retention?


🛠️ Tools Used
ToolPurposeGoogle SheetsData exploration, cleaning, and Pivot Table analysisTableau PublicInteractive dashboard and data visualization (coming soon)

📁 Dataset

Source: Telco Customer Churn Dataset — Kaggle
Size: 7,043 rows × 21 columns
Description: Real-world telecom customer data including demographics, services, contract types, charges, and churn status.


🔍 Project Process
Phase 1 — Data Exploration

Loaded the dataset into Google Sheets
Identified 21 columns including: CustomerID, Gender, SeniorCitizen, Tenure, Contract, MonthlyCharges, TotalCharges and Churn
Confirmed each row represents one individual customer
Confirmed Churn column stores Yes/No values
Confirmed SeniorCitizen column stores 1/0 values

Phase 2 — Data Cleaning

✅ Checked for empty/blank cells — none found
✅ Checked for duplicate rows — none found
✅ Confirmed all numeric columns are properly formatted
✅ Created readable IsSenior column converting 1/0 to Yes/No
Dataset was confirmed clean and ready for analysis


📸 Screenshot: 01_churn_clean_dataset.png

Phase 3 — Analysis
Headline KPI — Overall Churn Rate
MetricNumberTotal Customers7,043Customers Who Stayed5,174Customers Who Left1,869Churn Rate26.5% 🚨

⚠️ The industry benchmark for telecom churn is 15-20%. This company is significantly above average and requires urgent attention.


📸 Screenshot: 01_churn_overall_rate.png


Pivot Table 1 — Churn by Contract Type
ContractStayedChurnedTotalChurn RateMonth-to-month2,2201,6553,87542.7% 🔴One year1,3071661,47311.3% 🟡Two year1,647481,6952.8% 🟢

📸 Screenshot: 02_churn_by_contract.png

Key Finding:

Month-to-month customers churn at a massive 42.7% — nearly 1 in 2 leave
Two year contract customers are extremely loyal at only 2.8% churn
The longer the commitment, the lower the churn — a clear and actionable pattern


Pivot Table 2 — Churn by Senior Citizen
Senior CitizenStayedChurnedTotalChurn RateNo4,5081,3935,90123.6%Yes6664761,14241.7% 🔴

📸 Screenshot: 03_churn_by_senior.png

Key Finding:

Senior citizens churn at nearly double the rate of non-seniors (41.7% vs 23.6%)
Seniors make up only 16.2% of the customer base but represent a disproportionately high churn risk
Likely driven by fixed incomes, price sensitivity, and complex billing


Pivot Table 3 — Churn by Internet Service
Internet ServiceStayedChurnedTotalChurn RateDSL1,9624592,42119% 🟡Fiber Optic1,7991,2973,09641.9% 🔴No Internet1,4131131,5267.4% 🟢

📸 Screenshot: 04_churn_by_internet.png

Key Finding:

Fiber Optic customers churn at an alarming 41.9% — almost identical to month-to-month contracts
Customers with no internet service are the most loyal at 7.4% churn
Premium service customers are clearly not receiving premium value


Pivot Table 4 — Churn by Tenure
TenureStayedChurnedTotalChurn Rate0-11 months1,0709992,06948.3% 🔴12-23 months7383091,04729.5% 🟠24-35 months68319387622% 🟡36-47 months60214674819.5% 🟡48-59 months69712382015% 🟢60-72 months1,384991,4836.7% 🟢

📸 Screenshot: 05_churn_by_tenure.png

Key Finding:

Nearly 1 in 2 new customers (0-11 months) leaves within their first year
Churn rate drops consistently as tenure increases
Customers beyond 4 years are extremely loyal at only 6.7% churn
The first year is the most critical retention period for this business


Pivot Table 5 — Churn by Monthly Charges
Monthly ChargesStayedChurnedTotalChurn Rate$0-331,5231801,70310.6% 🟢$34-631,0333291,36224.2% 🟡$64-931,6488792,52734.8% 🔴$94-1249704811,45133.1% 🔴

📸 Screenshot: 06_churn_by_charges.png

Key Finding:

Customers paying more than $64/month are 3x more likely to leave than low paying customers
High paying customers have the highest expectations — and are clearly not being met
This directly connects to the Fiber Optic finding — premium price, poor experience

Phase 4 — Dashboard (Coming Soon)

Interactive Tableau Public dashboard covering all churn KPIs
Visuals: Overall churn rate, churn by contract, churn by tenure, churn by service type


💡 Key Insights & Recommendations
1. Month-to-Month Contracts are the Biggest Churn Driver
42.7% of month-to-month customers leave — the highest churn of any segment.

Recommendation: Introduce incentives to convert month-to-month customers to annual or two year contracts — discounts, free months, or added benefits for longer commitments.

2. Fiber Optic Service is Critically Underperforming
Despite being the premium service, Fiber Optic customers churn at 41.9% — nearly matching the worst contract type.

Recommendation: Urgently investigate Fiber Optic service quality, reliability, and pricing. Consider a dedicated Fiber support team and loyalty rewards for premium customers.

3. New Customers are Leaving Too Fast
48.3% of customers in their first year leave — a critical early churn problem that is expensive to sustain.

Recommendation: Implement a structured onboarding program with proactive check-ins at 3, 6, and 9 months. Offer first year loyalty rewards to encourage customers to stay past the critical early period.

4. Senior Citizens Need Special Attention
Senior citizens churn at 41.7% — nearly double the rate of non-seniors — likely due to price sensitivity and complex billing.

Recommendation: Introduce dedicated senior discount plans, simplified billing, and a dedicated senior customer support line to improve retention in this vulnerable segment.

5. High Paying Customers are Not Getting Value
Customers paying $64+ per month churn at over 33% — suggesting premium customers feel they are not getting value for money.

Recommendation: Introduce priority support, faster response times, and exclusive loyalty rewards for high paying customers to justify their premium spend.


📂 Repository Structure
📦 customer-churn-analysis
 ┣ 📊 data/
 ┃ ┗ telco_customer_churn.csv
 ┣ 📸 screenshots/
 ┃ ┣ 01_churn_clean_dataset.png
 ┃ ┣ 01_churn_overall_rate.png
 ┃ ┣ 02_churn_by_contract.png
 ┃ ┣ 03_churn_by_senior.png
 ┃ ┣ 04_churn_by_internet.png
 ┃ ┣ 05_churn_by_tenure.png
 ┃ ┗ 06_churn_by_charges.png
 ┣ 📋 dashboard/
 ┃ ┗ Tableau Public Link (coming soon)
 ┗ 📄 README.md

🚀 About This Project
This analysis was completed as part of a structured Data Analytics Internship program. The goal was to simulate a real client engagement — from raw data to actionable retention recommendations — using industry-standard tools and workflows.
Skills demonstrated:

Data exploration & quality auditing
Data cleaning & preparation
Customer churn & retention analysis
Business KPI analysis using Pivot Tables
Insight generation and business storytelling


Project by: Kganya Lekganyane
Internship Program: Future Interns — Data Science & Analytics
Date: April 2026
