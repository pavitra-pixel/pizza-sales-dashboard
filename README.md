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

## Features / Highlights
• Business Problem: Pizzeria owners generate large volumes of raw order data but often lack a quick way to see which products are actually profitable, when demand peaks, and which menu items are underperforming. Questions like "Which pizzas should we push in marketing?", "When do we need more staff on shift?", and "What should come off the menu?" are hard to answer from a transaction log alone.

• Goal of the Dashboard To deliver an interactive visual tool that:

- Tracks overall sales performance through key KPIs at a glance
- Reveals demand patterns by day and month to support staffing and inventory decisions
- Breaks down performance by pizza category and size
- Ranks every pizza by revenue, quantity, and order count to identify best and worst sellers

• Walkthrough of Key Visuals

Page 1 — Home

- KPI Cards (Top): Total Revenue $817,860.05 · Total Orders 21,350 · Total Pizzas Sold 49,574 · Avg Pizzas per Order 2.32 · Avg Order Value $38.31
- Daily Trend (Column Chart): Orders by day of week — Friday is busiest (3,538 orders), followed by Thursday and Saturday, with Sunday quietest (2,624 orders)
- Monthly Trend (Area Chart): Orders by month — July (1,935) and May (1,853) are peak months; September and October are the slowest
- % of Sales by Pizza Category (Donut): Classic leads at 26.9% of revenue, followed by Supreme (25.5%), Chicken (24.0%), and Veggie (23.7%)
- % of Sales by Pizza Size (Donut): Large drives 45.9% of revenue, Medium 30.5%, Small 21.8%, with XL/XXL under 2% combined
- Total Pizzas Sold by Category (Funnel): Classic (14,888) > Supreme (11,987) > Veggie (11,649) > Chicken (11,050)
  
Page 2 — Best / Worst Seller

- Top 5 / Bottom 5 by Revenue: The Thai Chicken Pizza leads at $43,434; The Brie Carre Pizza trails at $11,589
- Top 5 / Bottom 5 by Quantity Sold: The Classic Deluxe Pizza leads at 2,453 units; The Brie Carre Pizza trails at 490 units
- Top 5 / Bottom 5 by Total Orders: The Classic Deluxe Pizza appears in the most orders (2,329); The Brie Carre Pizza appears in the fewest (480)

• Business Impact & Insights

- Menu Strategy: The Brie Carre Pizza ranks last across revenue, quantity, and orders simultaneously — a strong candidate for removal or repositioning — while Classic Deluxe and Thai Chicken are consistent top performers worth featuring in promotions
- Staffing & Inventory Planning: The Friday–Saturday peak and July/January seasonality point to when extra staff and ingredient stock should be scheduled
- Size-Based Upselling: Large pizzas drive nearly half of all revenue despite Medium being ordered almost as often — upselling to Large is a clear revenue lever
- Category Focus: Classic pizzas outsell every other category in both units and revenue share, suggesting core recipes remain the strongest traffic driver even as specialty categories (Chicken, Supreme) are added

## Screenshots / Demos
![Home](https://github.com/pavitra-pixel/powerbi-sales-analytics-dashboard/blob/main/Home.png)
![best/worst seller](https://github.com/pavitra-pixel/powerbi-sales-analytics-dashboard/blob/main/Best_Worst%20seller.png)
