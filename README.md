## Project Overview
This project performs an end-to-end Customer Churn Analysis on a telecommunications dataset to quantify customer attrition, identify churn drivers and measure revenue impact.  
The objective is to support data driven retention strategies using SQL based transformation and Power BI visualization.

## Power BI Dashboard
![Customer Churn Dashboard](./dashboard_screenshot.png](https://github.com/abhay01pandey/Customer-Churn-Analysis-and-Predictive-Modeling-Dashboard/blob/5dafa73529f26b090a6e7b0baeeff8be7622beda/churn%20dashboard.png)

## Dataset

### Dataset Summary
- Domain: Telecommunications  
- Total Customers: 6,418  
- Total Features: 20+  

### Key Attributes
- Customer Demographics: Gender, Age, Marital Status, State  
- Account Information: Contract Type, Tenure, Monthly Charges  
- Services: Internet Type, Phone Service, Add-ons  
- Billing & Payments: Payment Method, Paperless Billing  
- Target Variable: Customer_Status  

## Tools & Technologies
- MySQL – Data exploration, cleaning, transformation  
- Power BI – KPI calculation and dashboard creation  
- GitHub – Version control and documentation  

## Workflow

### 1. Data Ingestion
- Created database db_churn
- Loaded raw customer dataset into MySQL
- Performed initial sanity checks using SELECT and COUNT queries

### 2. Data Exploration (SQL)
- Analyzed demographic distribution (Gender, State)
- Evaluated contract type distribution
- Examined customer status and revenue contribution
- Identified available service categories

### 3. Data Transformation (SQL)
- Selected relevant analytical columns
- Standardized categorical values
- Created a production-ready table:
  - prod_Churn

### 4. Analytical View Creation (SQL)
- Created churn-focused views to optimize Power BI performance:
  - vw_ChurnData – Churned and Stayed customers
  - vw_JoinData – Newly joined customers

### 5. KPI Calculation (Power BI)
- Total Customers
- Total Churn
- Churn Rate
- New Joiners

### 6. Data Visualization (Power BI)
- Built an interactive dashboard analyzing churn by:
  - Demographics
  - Geography
  - Services
  - Payment Methods
  - Contract Types
  - Tenure Groups

## Dashboard Insights

### Contract Risk
- Month-to-Month contracts account for 46.5% of total churn

### Service-Level Churn
- Fiber Optic internet users show the highest churn rate at 41.1%

### Payment Method Impact
- Mailed Check customers have a churn rate of 37.8%, significantly higher than digital methods

### Customer Lifecycle Risk
- Highest churn occurs within the first 0–6 months of tenure

## Results
- Overall churn rate identified at 27.0%
- High-risk customer segments clearly defined
- Revenue impact of churn quantified

## Business Recommendations
- Target Month-to-Month customers with retention offers
- Conduct service quality review for Fiber Optic internet
- Encourage digital payment adoption
- Improve onboarding experience for new customers

## How to Run the Project
1. Clone the repository
2. Load dataset into MySQL
3. Execute SQL scripts for analysis and transformation
4. Create analytical views
5. Connect Power BI to MySQL
6. Open the dashboard and explore insights

## Author
Abhay Pandey  
LinkedIn: www.linkedin.com/in/abhaypandey18
