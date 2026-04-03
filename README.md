# Pizza Sales Analytics Dashboard

An end-to-end Power BI dashboard analyzing pizza sales data to uncover revenue trends, peak periods, and product performance.

## Dashboard Preview
![Dashboard](<img width="1179" height="649" alt="image" src="https://github.com/user-attachments/assets/e74d9b55-0f4c-46c7-a502-63c3a2369cac" />
)
![Best Worst Seller](<img width="1178" height="643" alt="image" src="https://github.com/user-attachments/assets/fc29ce96-bf3d-4bcd-982b-438553cdd71e" />
)

## Dataset
- Size: 48,621 rows | Jan 2015 – Dec 2015
- Fields: Order ID, Pizza name, Category, Size, Quantity, Price, Date

## Key Insights
- Total Revenue: $817.86K | Total Orders: 21,350 | Pizzas Sold: 49,574
- Peak Day: Friday (3.5K orders) | Peak Month: July (1,935 orders)
- Top seller by revenue: Thai Chicken Pizza ($43K)
- Worst seller: Brie Carre Pizza ($12K)
- Classic category leads with 26.91% of total sales
- Large size contributes 45.89% of total quantity sold

## Features
- DAX KPIs: Total Revenue, Orders, Avg Order Value, Pizzas Sold
- Daily and monthly trend analysis
- Best/Worst Seller page (Top 5 & Bottom 5 by revenue, quantity, orders)
- Dynamic slicers filterable by Pizza Category and Date Range
- Drill-down navigation across two report pages

## Tools Used
| Tool | Purpose |
|------|---------|
| Power BI | Dashboard development |
| DAX | KPI calculations |
| Excel | Data cleaning & preparation |

## How to Use
1. Download `pizza_sales.pbix` from the `dashboard/` folder
2. Open in Power BI Desktop
3. Use slicers to filter by category and date
