Customer Churn Analysis — Data Analytics Internship Task 2

Project Overview:

This project was completed as part of a real-world Data Analytics Internship Task 2. The goal was to analyze customer subscription data to understand why customers leave and what keeps them engaged.

The analysis answers key business questions such as:
    • Why are customers leaving the platform? 
    • Which customer segments are most likely to churn? 
    • How long do customers typically stay active? 
    • What actions can improve customer retention? 
    
🛠️ Tools Used:
Tool	Purpose
Google Sheets	Data exploration, cleaning, and Pivot Table analysis
Tableau Public	Interactive dashboard and data visualization 

📁 Dataset:
    • Source: Telco Customer Churn Dataset — Kaggle 
    • Size: 7,043 rows × 21 columns 
    • Description: Real-world telecom customer data, including demographics, services, contract types, charges, and churn status. 
    
🔍 Project Process:
Phase 1 — Data Exploration
    • Loaded the dataset into Google Sheets 
    • Identified 21 columns, including: CustomerID, Gender, SeniorCitizen, Tenure, Contract, MonthlyCharges, TotalCharges, and Churn 
    • Confirmed each row represents one individual customer 
    • Confirmed Churn column stores (Yes/No) values
    • Confirmed SeniorCitizen column stores (1/0 )values 
    
Phase 2 — Data Cleaning
    • ✅ Checked for empty/blank cells 
    • ✅ Checked for duplicate rows 
    • ✅ Confirmed all numeric columns are properly formatted 
    • ✅ Created readable IsSenior column converting 1/0 to Yes/No 


Phase 3 — Analysis
📸 Screenshot: 01_churn_overall_rate.png
Findings:
    • Month-to-month customers churn at 42.7% 
    • Two year contract customers are extremely loyal at only 2.8% churn 
    • A longer commitment equates to a longer churn— a clear and actionable pattern 

Pivot Table 2 — Churn by Senior Citizen
Findings:
    • Senior citizens churn at almost twice the rate of non-seniors (41.7% vs 23.6%) 
    • Seniors make up only 16.2% of the customer base in its entirety, but represent a high churn risk 
    • This could be caused by fixed incomes and price sensitivity. 
    
Pivot Table 3 — Churn by Internet Service

Pivot Table 4 — Churn by Tenure

Findings:
    • Nearly 1 in 2 new customers (0-11 months) leave within their first year 
    • Churn rate drops tenure increases (consistently)
    • Customers beyond 4 years are extremely loyal, at only 6.7% churn 
      
Pivot Table 5 — Churn by Monthly Charges

Findings:
    • Customers paying more than $64/month are 3x more likely to leave than low-paying customers 
    • High-paying customers have the highest expectations, and it seems as if they are not being met
    • This is very similar to the Fiber Optic finding- high payments with low quality
    
Phase 4 — Tableau Public Dashboard ✅
Built an interactive, client-ready dashboard using Tableau Public covering all churn KPIs and business questions.
Dashboard includes 5 interactive charts:
    • Overall Churn Rate — Bar chart showing 5,174 stayed vs 1,869 churned 
    • Churn by Contract Type — Stacked bar showing month-to-month dominates churn 
    • Churn by Internet Service — Stacked bar showing Fiber Optic critical churn 
    • Churn by Tenure — Full width chart showing churn decreases over time 
    • Churn by Monthly Charges — Bar chart showing high payers churn most 

🔗 View Live Interactive Dashboard
💡 Key Insights & Recommendations
1. Month-to-Month Contracts are the Biggest Churn Drivers:
42.7% of month-to-month customers leave — the highest churn of any segment.
Recommendation: Introduce incentives to convert month-to-month customers to annual or even two months in forms of discounts, free months, or even added benefits for longer commitments.

3. Fiber Optic Service is Critically Underperforming:
Apart from being the premium service, Fiber Optic customers churn at 41.9%, which almost matches the worst contract type.
Recommendation: Urgently investigate Fiber Optic service quality, the reliability, andpricing. Also consider a dedicated Fiber support team to regularly check it out, and loyalty rewards for premium customers.

4. New Customers are Leaving Too Fast:
48.3% of customers in their first year leave, which is a critical early churn problem that is quite expensive to sustain.
Recommendation: Implement a structured debrief session with proactive check-ins at 3 to 6 months. Offer first-year loyalty rewards to encourage customers to stay for longer.

5. Senior Citizens Need Special Attention:
Senior citizens churn at 41.7%,  could likely be due to price sensitivity.
Recommendation: Introduce a senior customer support line dedicated to improve retention in this segment.

6. High Paying Customers are Not Getting the Value the pay for:
Customers paying $64+ per month churn at over 33%, which strongly suggests that premium customers feel they are not getting value for money.
Recommendation: Introduce priority support, faster response times, so they can get value of money(quality) services.


📂 Repository Structure:
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
 ┃ ┗ Tableau Public Link 
 ┗ 📄 README.md

🚀 About This Project:

This analysis was completed as part of a structured Data Analytics Internship program. The goal was to simulate a real client engagement which transforms raw data into actionable retention recommendations, using industry-standard tools and workflows.
Skills demonstrated:
    • Data exploration & quality auditing 
    • Data cleaning & preparation 
    • Customer churn & retention analysis 
    • Business KPI analysis using Pivot Tables 
    • Insight generation and business storytelling
   
Project by: Kganya Lekganyane Internship Program: Future Interns — Data Science & Analytics Date: 20 April 2026

Internship Program: Future Interns — Data Science & Analytics
Date: April 2026
