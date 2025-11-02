# Renewable Energy Usage Analysis and Visualization

### Dashboard Link : https://app.powerbi.com/links/8_ZntX-y_A?ctid=ee0c014f-76f0-4c50-ba79-351579057b96&pbi_source=linkShare

## Problem Statement

This project analyzes renewable energy usage and cost savings data to provide actionable insights through interactive Tableau dashboards. It demonstrates end-to-end data workflow from loading data into Snowflake, transforming it using SQL, and building informative visualizations to track monthly energy consumption and cost savings.

## Steps Followed

- **Step 1:** Creating & loading data to Amazon S3 bucket for cloud data storage.
- **Step 2:** Creating the appropriate Snowflake role and integration object, updating trust policies for secure data access.
- **Step 3:** Loading data from S3 into Snowflake tables.
- **Step 4:** Gaining data understanding through exploration and profiling in Snowflake.
- **Step 5:** Performing complex data transformations with Snowflake SQL to prepare analytics-ready datasets.
- **Step 6:** Connecting Snowflake with Tableau for live data visualization.
- **Step 7:** Developing charts for monthly renewable energy usage consumption.
- **Step 8:** Creating charts that reflect cost savings driven by renewable adoption.
- **Step 9:** Designing comprehensive dashboards combining all key metrics and trends.
- **Step 10:** Publishing final Tableau workbook to Tableau Cloud for stakeholder sharing and collaborative access.

## Features & Insights

- Fully automated pipeline from cloud storage to data warehouse and visualization layer.
- Detailed time series analysis on renewable energy consumption.
- Cost-saving analysis illustrating financial benefits linked with renewable usage.
- Interactive dashboards to slice and dice the data by time and other dimensions.
- Secure, scalable solution leveraging Snowflake and Tableau cloud services.

## How to Use

1. Ensure AWS S3 bucket is properly configured with the dataset files.
2. Create necessary roles and integrations in Snowflake for data ingestion.
3. Load and transform data inside Snowflake SQL environment.
4. Connect Tableau desktop to Snowflake using provided credentials.
5. Use dashboards to interactively explore renewable energy trends and cost savings.
6. Publish dashboards to Tableau Cloud for wider access.

## Additional Notes

- Proper IAM roles and security policies in AWS and Snowflake are critical for seamless operation.
- Data transformation scripts in Snowflake should be adapted as data evolves.
- Tableau workbook performance depends on data volume and connection configurations.
