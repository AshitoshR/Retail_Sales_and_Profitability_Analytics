# Retail_Sales_and_Profitability_Analytics
Developed an interactive report in Power BI Desktop to analyze sales, profit, discount performance across different categories. Use DAX to create measures to find top products, rank product according to discount. Develop KPI to compare recent complete month net sales with average monthly net sales of 23 complete months.

# Retail Sales & Profitability Analytics Report

## Project Overview

An interactive five-page Power BI report developed to analyze retail sales, profitability, product performance, customer performance, and regional trends.

The project uses Power BI Desktop to transform retail data into meaningful business insights through data modeling, DAX measures, interactive visualizations, and KPI analysis.

## Project Objectives

- Analyze overall sales, net sales, costs, and profitability.
- Track sales and profit trends over time.
- Identify top-performing products and product categories.
- Analyze top customer performance and regional performance.
- Evaluate profit margins and discount rates to understand profitability.
- Develop a KPI to compare the latest complete month's Net Sales against the historical average monthly Net Sales benchmark.
- Create interactive report pages with KPI visuals, charts, slicers, and navigation to support data-driven decision-making.

## Tools & Technologies

- **Power BI Desktop** — Report development, data visualization, KPI implementation, and interactive report creation.
- **Power Query** — Data cleaning, transformation, and preparation.
- **DAX** — Measures for sales, costs, profit, profit margin, discount analysis, monthly benchmarks, and KPI calculations.
- **Microsoft Excel** — Data validation and cross-checking of calculations using formulas and PivotTables.

## Key Features

- **Sales Performance Analysis:** Analyzed Gross Sales, Net Sales, Profit, Total Cost, and Discount Amount.
- **Time-Based Analysis:** Examined monthly sales trends and quarterly and yearly performance.
- **KPI Performance Monitoring:** Developed a native Power BI KPI visual comparing the latest complete month's Net Sales against the average monthly Net Sales benchmark.
- **Benchmark Calculation:** Calculated average monthly Net Sales across 23 complete calendar months, excluding September 2023 and September 2025 because they contain incomplete transaction periods.
- **KPI Performance Evaluation:** Compared August 2025 Net Sales of ₹5.87 lakh against the historical monthly benchmark of ₹5.99 lakh, resulting in performance approximately 1.97% below the benchmark.
- **Product Analysis:** Identified top-performing products and compared profitability across product categories.
- **Customer & Regional Analysis:** Compared the top 10 customers and cities by Net Sales and Profit, and analyzed city-level Profit Margins.
- **Profitability Deep Dive:** Investigated product-category profitability, discount rates, grocery product performance, and Set Dairy performance across cities.
- **Interactive Reporting:** Used slicers, KPI visuals, charts, and Page Navigator to support interactive exploration of the report.

## Dataset

The dataset contains four tables:

- Customers — 200 records
- Products — 50 records
- Stores — 5 records
- Transactions — 5,000 records

## Data Model

- Established relationships between the Customers, Products, Stores, and Transactions tables.
- Connected the DateTable to the Transactions table for time-based analysis.
- Used one-to-many relationships, with dimension tables on the one side and Transactions on the many side.
- Configured single-direction cross-filtering for the relationships.
- Checked key relationships and data quality to ensure reliable reporting.

## DAX Measures

Created DAX measures to calculate and analyze key retail performance metrics:

- **Gross Sales:** Calculated using Quantity and Product Unit Price.
- **Discount Amount:** Calculated to measure the reduction from Gross Sales.
- **Net Sales:** Calculated after deducting Discount Amount from Gross Sales.
- **Total Cost:** Calculated to evaluate the cost of sold products.
- **Profit:** Calculated as Net Sales minus Total Cost.
- **Profit Margin:** Calculated as Profit divided by Net Sales.
- **Discount Rate:** Calculated as Discount Amount divided by Gross Sales.
- **Dynamic Ranking Measures:** Created measures to identify key results, including the top product by Net Sales, the top product by Profit, the highest-profit city, and the top customer by Net Sales.
- **Average Net Sales - Complete Months:** Calculated the arithmetic average of monthly Net Sales across 23 complete calendar months.
- **Latest Complete Month Net Sales:** Identified and calculated Net Sales for the latest fully completed calendar month.
- **KPI Display Measures:** Created separate display measures to convert the Indicator and Target values from rupees into lakhs without modifying the original financial calculation measures.

## KPI Methodology and Validation

- Identified the dataset's transaction date range from September 10, 2023, to September 9, 2025.
- Excluded September 2023 and September 2025 because both months contain incomplete transaction periods.
- Used the remaining 23 complete calendar months to calculate the average monthly Net Sales benchmark.
- Calculated total Net Sales across the 23 months as ₹13,775,950.4585.
- Calculated the average monthly Net Sales benchmark as ₹598,910.8895.
- Compared August 2025 Net Sales of ₹587,098.4135 against the benchmark.
- Achieved a KPI performance result of approximately -1.97%.
- Validated the benchmark, monthly Net Sales values, and latest complete month's Net Sales against Excel.
- Used separate display measures to present the KPI Indicator and Target in Indian lakh notation while retaining the original rupee-based measures.

## Key Business Insights

- **Product Performance:** Identified top-performing products by Net Sales and Profit to compare revenue generation and profitability.
- **Category Profitability:** Compared Electronics, Fashion, and Groceries using Net Sales, Profit, and Profit Margin.
- **Regional Performance:** Identified North Teresashire as the leading city by Profit and Profit Margin in the analysis.
- **Grocery Analysis:** Found that Groceries contributed the highest Profit in North Teresashire, with a Profit Margin of 41.80%.
- **Product-Level Insight:** Set Dairy generated a Profit of 14,519.96 in North Teresashire, with 18 units sold.
- **Discount Analysis:** Compared discount rates across product categories to understand their relationship with sales and profitability.
- **KPI Performance:** August 2025 Net Sales were approximately 1.97% below the historical average monthly Net Sales benchmark.

## Data Validation

- Cross-checked Power BI calculations against Excel formulas and PivotTables.
- Validated Gross Sales, Net Sales, Profit, and Profit Margin calculations.
- Verified all 25 individual monthly Net Sales values against Excel PivotTable results.
- Validated the 23-month average Net Sales benchmark against Excel, with no difference between the results.
- Verified August 2025 Net Sales against the dataset.
- Verified product, category, city, and customer rankings against Excel results.
- Verified data relationships, checked data quality, and tested slicers and filters to ensure the report behaved correctly.
- Reviewed chart titles, axis labels, number formats, KPI visual formatting, and page navigation.

These validation steps helped ensure the accuracy, consistency, and reliability of the report.

## Report Pages

1. Executive Overview
2. Sales & Time Analysis
3. Product Analysis
4. Customer & Regional Analysis
5. North Teresashire – Deep Dive Analysis

## Conclusion

This project demonstrates the practical application of Power BI Desktop, Power Query, DAX, and Excel in developing an interactive retail sales and profitability analytics report.

It combines data preparation, data modeling, financial calculations, KPI development, historical benchmarking, time-based analysis, product performance evaluation, and regional profitability analysis.

The KPI implementation demonstrates the ability to develop a historical performance benchmark, account for incomplete reporting periods, compare actual performance against a target, and validate business calculations against Excel.

The project strengthened practical skills in data preparation, data modeling, DAX calculations, data visualization, KPI development, and business insight generation.
