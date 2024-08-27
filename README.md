# Business-Insights_360

## Project Overview

AtliQ Hardware has experienced significant growth in recent years and has decided to leverage data analytics through Power BI to stay ahead of its competitors. This project marks their first foray into data-driven decision-making, aiming to address stakeholders' questions across key domains such as finance, sales, marketing, and supply chain management.

I developed this project by following the Codebasics Power BI Course. You can find the course [here](https://codebasics.io/bootcamps/data-analytics-bootcamp-with-practical-job-assistance).

[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiNGEwYmE5NTEtYWNiZS00NTNiLWJjMTktOGU2YzFkYWRkYWU4IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

## Tech Stacks

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## Power BI Techniques Mastered

- Key Questions to Ask Before Starting a Project
- Creating calculated columns
- Creating measures using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- Creating date table using M Language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting of the values in visuals using icons or background color
- Data validation techniques
- PowerBI Service
- Publishing reports to PowerBI Service
- Setting up personal gateway to set up the auto refresh of data
- PowerBI App creation
- Collaboration, workspace, access permissions in PowerBI Service
- And much more 😅

## GitHub

- Uploading Large size files using GitHub LFS
- Tracking the particular type of file extensions for LFS

## Business related terms

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Company's Background

AltiQ Hardware is a rapidly expanding company with a global presence, specializing in the sale of computers and computer accessories through three main channels:

Retailers
Direct Sales
Distributors

Recently, the company faced unexpected losses from opening a store in America, despite relying on surveys, intuition, and Excel analysis. Additionally, competitors have established analytics teams to drive data-informed decisions. To stay competitive, AltiQ Hardware needs to build its own analytics team to gain valuable insights and make data-driven decisions.

Project Kickoff

Before starting the project, it’s crucial to clarify the purpose and scope. Here are some key questions to address:

1. What is the primary objective of building this Power BI dashboard?
2. How will the success of this project be measured?
3. What is the project deadline?
4. Do stakeholders expect a preview before the final release?
5. What are the stakeholders’ expectations from this project?
6. What concerns or fears do stakeholders have regarding the dashboard?
7. Who will be using this dashboard and for what purposes?
8. What are the stakeholders' expectations upon project completion?
9. What potential issues could arise during the project?
10. What resources or data are needed to build this dashboard?
11. Are there any stakeholder inputs on the design and layout of the dashboard?

Following the project kickoff meeting, the data engineering team will provide the requested data to the analytics team. 
Let’s explore the data and begin the analysis.

## Dataset Understanding

Gaining a thorough understanding of the available data is crucial for effective analysis. Before diving into the analysis, take time to familiarize yourself with the data at hand. This includes:

- Identifying the Data Sources: Determine where the data is coming from and its relevance to the project.
- Understanding Data Structure: Review the data format, organization, and relationships between datasets.
- Assessing Data Quality: Check for completeness, accuracy, and consistency of the data.
- Recognizing Data Types: Identify the different types of data (e.g., numerical, categorical) and their implications for analysis.
- Exploring Data Variables: Understand what each variable represents and how it contributes to the analysis.

A clear grasp of these aspects will provide a solid foundation for performing meaningful and accurate analysis.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions

- gdb041:
  - dim_customer
    - 27 distinct markets (eg., India, USA, Spain)
    - 75 distinct customers thorough out the market
    - 2 types of platforms
      - Brick & Motors - Physical/offline store
      - E-commerce - Online Store (Amazon, flipkart)
    - Three channels
      - Retailer
      - Direct
      - Distributors
 - dim_market
  - 27 distinct markets (eg., India, USA, spain)
  - 7 sub-zones
  - 4 regions
   - APAC
   - EU
   - nan
   - LATAM
 - dim_product
  - Divisions
   - P & A
    - Peripherals
    - Accessories
   - PC
    - Notebook
    - Desktop
   - N & S
    - Networking
    - Storage
  - There are 14 different categories, Like Internal HDD, keyboard
  - There are different variants available for the same product
 - fact_forecast_monthly
  - This table is used to forecast the customer’s need in advance, which can help in
   - Higher customer satisfaction
   - Reduced cost in warehouses for storage purpose
  - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
  - All the date of the month will be replaced by the start date of the month
  - It will have all the column names and in the end it will have the forecast quantity need of the customer
 - fact_sales_monthly
  - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.

- gdb056 :
  - freight_cost
   - This table has details of travel cost and other cost for each market with fiscal year
  - gross_price
   - Has the details of gross prices with product code
  - manufacturing_cost
   - Has the details of manufacturing cost with product code with year
  - Pre_invoice_dedutions
   - Has the details of pre invoice deductions percentage for each cutomer with year
  - Post_invoice_deductions
   - Post invoice deductions and other deductions details







