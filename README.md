# Pizza Sales Analytics Dashboard
An interactive, two-page Power BI report built to analyze a full year of pizza order transactions — surfacing revenue trends, order patterns, and product-level performance to separate best sellers from underperformers.

## Short Description / Purpose
The Pizza Sales Dashboard is a visually engaging and analytical Power BI report designed to help restaurant managers, franchise operators, and data analysts understand how a pizzeria performed across 2015. It tracks core sales KPIs (revenue, orders, pizzas sold), visualizes daily and monthly ordering trends, breaks sales down by pizza category and size, and ranks every menu item by revenue, quantity sold, and order count — making it easy to spot what's driving sales and what belongs on the chopping block.

## Tech Stack
The dashboard was built using the following tools and technologies:
- 📊 Power BI Desktop – Main data visualization platform used for report creation
- 📁 Power Query – Data cleaning and transformation layer for reshaping raw order timestamps into daily/monthly trend fields
- 🧮 DAX (Data Analysis Expressions) – Used for calculated KPI measures: Total Revenue, Total Orders, Total Pizzas Sold, Avg Pizzas Per Order, Avg Order Value
- 📄 Data Modeling – Single fact table (pizza_sales) at the order-line grain, with category, size, and date attributes enabling cross-filtering across all visuals
- 📁 File Format – .pbix for development, .csv for the raw data source, .png for dashboard previews

## Data Source
Source: pizza_sales.csv — a transactional order-line dataset from a pizzeria.

Contains 48,620 order-line records spanning January 1 – December 31, 2015 (21,350 unique orders). Each row represents one pizza within an order, with fields for order ID, pizza ID, quantity, order date/time, unit price, total price, pizza size (S/M/L/XL/XXL), pizza category (Classic/Veggie/Supreme/Chicken), ingredients, and pizza name.

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
