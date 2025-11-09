# Overview-
This project executes a comprehensive Customer Churn Analysis using a telecommunications dataset. The core business objective was to calculate the overall Churn Rate, identify the primary drivers of customer attrition across demographics, services, and account metrics, and quantify the revenue impact of churn. The final output is a high-level, interactive Power BI Dashboard built on data transformed and aggregated using SQL.

# Dataset & Tools Used
Dataset:

The project uses a sample Telecommunications Customer Records dataset containing 20+ variables related to customer account status, services, contract type, monthly charges, and churn status.

Tools:

Data Processing: MySQL was the primary platform used for initial data exploration, cleaning, transformation, aggregation, and the creation of optimized views (vw_ChurnData, vw_JoinData).

Visualization: Power BI was used to calculate primary KPIs, design the dashboard, and create interactive visualizations of the churn drivers.

# Workflow
Data Ingestion and Exploration (SQL):

Loaded raw customer data into a database (db_churn).

Executed initial queries (SELECT *, COUNT) to understand the distribution of key variables (Gender, State, Contract).

Data Cleaning and Transformation (SQL):

Data Aggregation: Calculated total counts and percentages for demographics, service types, and account breakdown.

Revenue Quantification: Calculated total revenue and revenue percentage by Customer_Status.

Structured Output: Created a final production table (prod_Churn) and analytical views (vw_ChurnData, vw_JoinData) to ensure the data model was optimized for Power BI consumption.

Visualization and Reporting (Power BI):

Connected Power BI directly to the final SQL views for real time reporting.

Calculated primary KPIs, including Total Churn (1,732) and the 27.0% Churn Rate.

Designed the dashboard to visualize patterns across high risk factors like Payment Method, Internet Type, and Tenure Groups.

# Dashboard Insights
The final Power BI dashboard revealed several high-impact insights crucial for retention strategy:

Critical Contract Risk: The Month-to-Month contract type is the highest risk category, accounting for 46.5% of total attrition.

Service Quality Flag: Customers utilizing Fiber Optic internet service showed the highest single-service churn rate at 41.1%, indicating potential quality or pricing issues within that product line.

Payment Method Correlation: The Mailed Check payment method had a disproportionately high churn rate (37.8%) compared to digital methods.

Customer Lifecycle Risk: Churn is highest among customers with shorter tenure (0-6 Months), suggesting poor initial onboarding or early service dissatisfaction.

# Results 
The analysis successfully quantified the scale of the retention problem (27.0% Churn Rate) and identified clear, data-driven targets for intervention.

Key Outcomes:

Retention Focus Shift: Strategically re-focus retention marketing efforts on customers with Month-to-Month contracts and those using Mailed Check payments.

Product Deep Dive: Recommended an immediate technical and customer service review of the Fiber Optic service line to address the high rate of service-related churn.

Onboarding Improvement: Insights highlight the need to improve the customer experience in the first six months of service to combat early attrition.
