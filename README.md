# Financial Sales Performance Dashboard
# Project Overview
This project is an interactive Power BI dashboard designed to analyze sales, profitability, product performance, customer segments, discount levels, and country-level results.

The dashboard helps answer the following business questions:
- Which products and customer segments generate the highest sales?
- Which segments are profitable or loss-making?
- How are discount levels related to profit margins?
- Which countries generate the highest sales and profit?
- How do sales and profit change over time?

# Dataset
The project uses the Microsoft Financial Sample dataset.
- 700 records
- Reporting period: September 2013 to December 2014
- 5 countries
- 6 products
- 5 customer segments
- 4 discount bands

Each row represents an aggregated sales record for a combination of country, product, customer segment, discount band, and reporting month.

# Business Calculations
- Gross Sales = Units Sold × Sale Price
- Net Sales = Gross Sales − Discounts
- Profit = Net Sales − COGS
- Profit Margin = Profit ÷ Net Sales
  
# Key Performance Indicators
- Total Net Sales: $118.73M
- Total Profit: $16.89M
- Total COGS: $101.83M
- Overall Profit Margin: 14.23%

# Key Insights
- Paseo generated the highest net sales at approximately $33.01M.
- The Government segment generated approximately $52.50M in sales and $11.39M in profit.
- The Enterprise segment generated approximately $19.61M in sales but recorded an overall loss of approximately $614.5K.
- The United States generated the highest sales.
- France generated the highest total profit.
- Germany recorded the highest profit margin among the five countries.
- High-discount records had a profit margin of approximately 9.1%, compared with 17.9% for low-discount records and 21.9% for records without discounts.

# Dashboard Features
- KPI overview for net sales, profit, COGS, and profit margin
- Monthly sales and profit analysis
- Product-level sales and COGS comparison
- Customer segment profitability analysis
- Country-level sales and profit comparison
- Discount-band profitability analysis
- Interactive filters for year, country, segment, and product

# DAX Measures
- Total Sales = SUM(Financials[Sales])

- Total Profit = SUM(Financials[Profit])

- Total COGS = SUM(Financials[COGS])

- Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

The table name may differ depending on the Power BI data model.

# Tools Used
- Power BI Desktop
- DAX measures
- Data validation
- Interactive data visualization

# Data Limitations

The dataset is a fictional financial sample and does not represent a real company.

The 2013 data covers only September through December, while 2014 contains a complete year. Therefore, direct full-year growth comparisons between 2013 and 2014 may be misleading.

The available reporting period is also not sufficient to establish reliable seasonality.

# Future Improvements
- Add a dedicated calendar table
- Add comparable-period year-over-year analysis
- Add drill-through pages for products and customer segments
- Add dynamic tooltips and report-navigation buttons
- Add budget or target data for variance analysis

# Repository Contents
- Power BI report (.pbix)
- Dashboard preview (.pdf)
- Source dataset (.xlsx)
