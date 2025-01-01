# BankSmart_End-To-End-Data-Analytics-Project-Czechoslovakia Banking Financial Data Analysis
This project involves a comprehensive analysis of financial data for the Czechoslovakia Bank using a manually created dataset of over 1 million records across 8 tables. The workflow covers data cleaning, transformation, integration with S3 and Snowflake, and dashboard creation for actionable insights.


**Project Overview**
The dataset, representing 5 years of financial activity, includes the following tables:

Account: Customer account details, including ID, opening date, and type.
Card: Issued card details such as ID, issue date, and type.
Client: Demographic details like ID, birthdate, gender, and district.
Disposition: Client-account relationships, indicating roles like owner or authorized user.
District: Socio-economic and demographic indicators for districts.
Loan: Loan details, including ID, issue date, amount, and associated account.
Order: Client orders with ID, linked accounts, date, and description.
Transaction: Account transaction records with ID, date, type, and amount.

**Workflow Highlights**
1. Data Integration
Storage Integration: S3 bucket was used to store datasets, with secure access configured via AWS IAM roles.
Snowflake Integration: Snowflake stages were created to load and manage data using external integration and file formats.
2. Data Cleaning & Transformation
Duplicates, null values, and inconsistencies were addressed during data cleaning.
Dates were transformed for consistency and ease of analysis.
Missing values in critical fields, such as transaction banks, were updated with appropriate data.
Currency conversions were applied (e.g., CZK to USD) for uniform financial reporting.
3. Data Pipeline
Automated Snowflake Snowpipes were implemented to ingest data from S3 into Snowflake tables.
Custom SQL queries were used for transformations and aggregations to support downstream analysis.
4. Dashboard Creation
Dashboards were developed using Tableau and Power BI to visualize key metrics and trends:
Year-over-year and month-over-month performance.
Demographic profiles of clients by district.
Loan portfolio distribution and profitability.
Card usage patterns and credit card profitability.
Transaction trends and anomalies.
Analysis Objectives
The bank aims to derive actionable insights to guide decision-making and explore growth opportunities. Key questions include:

What is the demographic profile of clients, and how does it vary by district?
How has the bank's performance evolved year-over-year and month-over-month?
Which account types are most common, and how do they differ in usage and profitability?
Which card types are most used, and what is the profitability of the credit card business?
What are the bank's significant expenses, and how can they be optimized?
How does the loan portfolio vary by purpose and client segment?
How can customer service and satisfaction be improved?
Can new products or services be introduced to attract customers and enhance profitability?

**Objective**
The project's goal is to provide a detailed analysis of the bank's operations using Snowflake, automated pipelines, and advanced dashboards. The insights will support optimizing financial operations, identifying risks, and discovering growth opportunities.
