# powerbi--financial-sales-dashboard
: Power BI dashboard analyzing financial sales, profit, margin, products, countries, customer segments, and discount bands. 
# Financial Sales & Profit Dashboard

An interactive Power BI report for exploring sales and profitability across products, countries, customer segments, and discount bands.

## Dashboard KPIs

- Total Sales
- Total Profit
- Profit Margin
- Total Units Sold

## Visuals

- Monthly sales trend
- Sales by product
- Sales by country map
- Sales by customer segment
- Sales by product and segment treemap
- Profit by country
- Profit margin gauge with target

## Filters and navigation

Slicers let users filter by:

- Year
- Segment
- Country
- Discount Band

The report also includes an Overview bookmark for returning to a saved report view.

## Data fields

The report uses fields from the financials dataset, including `Date`, `Product`, `Country`, `Segment`, `Discount Band`, `Sales`, `Profit`, and `Units Sold`.

## Measures

```DAX
Total Sales = SUM(financials[Sales])

Total Profit = SUM(financials[Profit])

Total Units Sold = SUM(financials[Units Sold])

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
