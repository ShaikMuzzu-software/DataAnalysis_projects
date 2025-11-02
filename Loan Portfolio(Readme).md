
# Loan Portfolio Analytics & Default Risk Dashboard

### Dashboard Link :https://app.powerbi.com/links/o_OLDKMDYk?ctid=ee0c014f-76f0-4c50-ba79-351579057b96&pbi_source=linkShare

## Problem Statement

This project creates a comprehensive Power BI report analyzing loan portfolio performance and default risk. It integrates SQL Server data, performs extensive data profiling and transformation, and leverages advanced DAX measures to highlight key metrics such as loan amounts by purpose, average income by employment type, default rates segmented by various categories, and year-over-year trends. The report also uses visualizations like donut charts, line charts, decomposition trees, and clustered column charts for insightful storytelling and decision-making.

## Steps Followed

- **Step 1:** Downloading, installing, and configuring the Standard Mode Gateway and Microsoft SQL Server.
- **Step 2:** Importing data into SQL Server.
- **Step 3:** Creating dataflows using Power BI Service and importing data into Power BI Desktop.
- **Step 4:** Defining columns and datasets, performing data types setup and profiling in Power Query Editor.
- **Step 5:** Adding shapes and renaming pages for clarity.
- **Step 6:** Developing DAX measures including:
  - Loan Amount by Purpose (using SUMX, FILTER, NOT, ISBLANK)
  - Average Income by Employment Type (CALCULATE, AVERAGE, ALLEXCEPT)
  - Default Rate by Employment Type (ALL, ALLEXCEPT, COUNTROWS, DIVIDE, FILTER)
  - Average Loan by Age Groups (AVERAGE, AVERAGEX, VALUES)
  - Default Rate by Year and Median Loan Amount by Credit Score category.
- **Step 7:** Creating and validating visualizations including donut charts, line charts, clustered column charts, and decomposition trees.
- **Step 8:** Setting up schedule and incremental refresh for dataflows.
- **Step 9:** Publishing the final report to Power BI Service and scheduling refresh.
- **Step 10:** Sharing the report for stakeholder access and collaboration.

## Features & Insights

- Interactive visuals provide detailed views on loan distribution, income levels, default risks, and credit categories.
- Advanced DAX logic enables year-over-year and median calculations driving precise insights.
- Drill-through filters and decomposition trees support deep-dive analysis.
- Incremental refresh optimizes performance for large datasets.
- Secure and scalable architecture with Power BI Service and Gateway support.

## How to Use

1. Configure the Standard Mode Gateway and install SQL Server.
2. Import and transform data using Power BI dataflows and Power Query Editor.
3. Implement and test DAX measures for accurate aggregations and trend analysis.
4. Build detailed visuals following the project design.
5. Set up scheduled and incremental data refreshes in the Power BI Service.
6. Share the report link with stakeholders for interactive data exploration.
7. Periodically update the dataset and maintain DAX and visual enhancements as needed.

## Notes

- Validate SQL Server connection and Gateway configurations to ensure seamless data import.
- Review DAX formulas for efficiency and accuracy.
- Monitor refresh schedules and performance metrics on Power BI Service.
- Customize visuals and filters based on evolving business requirements.
