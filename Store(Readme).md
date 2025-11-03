# Store-Dashboard

### Dashboard Link :https://app.powerbi.com/links/AZxpz2yjDy?ctid=ee0c014f-76f0-4c50-ba79-351579057b96&pbi_source=linkShare

## Problem Statement

This dashboard helps retail store managers and data analysts understand sales trends, product performance, and customer behavior. Visualizations guide inventory decisions, product assortment planning, and identify growth opportunities and areas of concern for operational improvement.

## Steps Followed

- **Step 1:** Load “Store-Data.xlsx” into Power BI Desktop.
- **Step 2:** Use Power Query Editor:
    - Enable “Column distribution”, “Column quality”, and “Column profile” in the Data Preview.
    - Profile columns based on the entire dataset.
- **Step 3:** Identify missing/erroneous values, especially in sales and product columns. Clean these by filtering, replacing, or excluding as needed.
- **Step 4:** Establish primary and foreign key relationships between tables.
- **Step 5:** Set cardinality to match business data structure (one-to-many, many-to-one, etc.).
- **Step 6:** Model data using Star Schema for optimum analytical efficiency.
- **Step 7:** Review all tables in model view for correctness.
- **Step 8:** Add and test various filters in the Filters Pane.
- **Step 9:** Visualize top and bottom 5 products by sales, quantity, and profit using bar charts and tables.
- **Step 10:** Create time-series analytics for sales trends, using line and column visuals.
- **Step 11:** Implement all business requirements in your report as outlined in documentation.
- **Step 12:** Create and validate DAX measures for KPIs such as total sales, sales percentage, and profit margin.
- **Step 13:** Edit interactions to refine how visuals respond to filters and slicers.
- **Step 14:** Add slicers for product category, store region, and other dimensions relevant to business analysis.
- **Step 15:** Tweak slicer/filter behavior, especially for dimension tables.
- **Step 16:** Enhance report layout using themes, text boxes, store branding, and logos.
- **Step 17:** Publish final report to Power BI Service for sharing and dashboard management.

## Features & Insights

- Top/Bottom 5 Products by key KPIs.
- Sales trends visualized by various time periods.
- Data model organized in Star Schema structure.
- Slicers for custom filtering by product, category, and region.
- Interactive dashboard supporting custom business logic filters.
- Key DAX measures and transformations for advanced analysis.

## Example DAX Expressions

-- Top 5 Products by Sales
Top5Products = 
TOPN(
    5,
    SUMMARIZE(
        'Sales', 
        'Product'[Product Name], 
        "Total Sales", SUM('Sales'[Sales Amount])
    ), 
    [Total Sales]
)

-- Year-Over-Year Sales Growth
YoY Sales Growth = 
VAR PrevYearSales = CALCULATE(
    SUM('Sales'[Sales Amount]), 
    SAMEPERIODLASTYEAR('Date'[Date])
)
RETURN 
DIVIDE(
    SUM('Sales'[Sales Amount]) - PrevYearSales, 
    PrevYearSales
)
