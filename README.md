# Amazon Sales Dashboard Project

## Overview

This repository contains a Power BI dashboard developed to visualize and analyze Amazon sales data.  The goal of this project is to provide actionable insights into key performance indicators (KPIs) such as overall sales, sales trends by geography and product category, and the status of orders. This dashboard empowers stakeholders to monitor performance, identify opportunities, and make data-driven decisions to optimize sales strategies.

## Key Features & Insights

The dashboard is structured into three primary views:

*   **Overview:**  A high-level summary of key metrics, providing a quick snapshot of overall performance.
    *   Total Sales Revenue: `₹120.5K`
    *   Total Sales: `₹4.0K`
    *   Total unique products sold: `644`
    *   Sales distribution by city and state, showing the top-performing regions (e.g., Maharashtra, Karnataka).
    *   Sales Trends: A detailed time-series visualization of sales by city over time, highlighting peaks and troughs in sales activity.
    *   Order Status Breakdown: Summarized to track the number of orders currently in different stages (Pending, Shipped, Cancelled, and Delivered).
*   **Products:** A product-centric view displaying the performance of different product categories and individual products.
    *   Displays a product selection page to filter specific product analysis.
*   **Product View:** An in-depth analysis of individual product performance
    *   Key metric summary: Sales Amount, Unit Sold, Returned (Loss) and Reviews
    *   Unit sold trends: A detailed time-series visualization of units sold for the specific product.

## Visualizations & Dashboard Elements

The dashboard utilizes a variety of visualizations to effectively communicate the data:

*   **Bar Charts:**  Sales by City and Sales by State are presented as horizontal bar charts for easy comparison of regional performance.
*   **Line Charts:** Sales by City trends are visualized using a line chart to identify patterns, seasonality, and growth or decline over time.
*   **Card Visuals:** Key metrics (Total Sales, Seller Count) are displayed as prominent card visuals for immediate recognition.
*   **Filters/Slicers:**  Interactive filters allow users to drill down into specific product categories (e.g., "Girls Clothing Sets") or order statuses to refine the analysis.
*   **Tooltip Reporting:** Product page contains a tooltip that display key product metrics over time.

## Data Sources

The dashboard is built using data extracted from an Amazon sales dataset. Data source can vary from csv files to direct server connections.

## Technical Details

*   **Tool:** Power BI Desktop
*   **Data Transformation:** Power Query Editor was used for data cleaning, transformation, and shaping, including:
    *   Handling missing values.
    *   Data type conversions (e.g., text to numbers, dates).
    *   Creating calculated columns (if applicable).
*   **Data Modeling:** Power BI's data modeling capabilities were used to establish relationships between tables and create a star schema for efficient querying.
*   **DAX (Data Analysis Expressions):** DAX formulas were used to create calculated measures and columns, such as:
    *   `Total Sales = SUM(Sales[SalesAmount])`  (Example: Replace `Sales` and `SalesAmount` with your actual table and column names)
    *   Creating calculated measures and columns, such as:
        *   `Units Sold = COUNT(Sales[Units])`
        *   `Returned Losts = SUM(Sales[Returned (Loss)])`
*   **Performance Optimization:** Measures taken to optimize the dashboard's performance, such as:
    *   Optimizing data types and sizes.
    *   Minimizing the use of complex DAX calculations where possible.
    *   Ensuring efficient data modeling.

## How to Use/Replicate

1.  **Prerequisites:**
    *   Power BI Desktop installed.
2.  **Download:** Clone or download this repository.
3.  **Open the .pbix file:** Open the `Amazon_Sales_Dashboard.pbix` file (or the name of your Power BI file) in Power BI Desktop.
4.  **Data Source Configuration (Important):**
    *   You will likely need to configure the data source connections to point to *your* local data. Go to "Transform Data" -> "Data source settings" and update the file paths or server connections.
5.  **Explore the Dashboard:** Navigate through the different tabs (Overview, Products, Product View) and interact with the filters and visualizations.

## Future Enhancements

*   **Advanced Analytics:** Incorporate forecasting and predictive analytics using Power BI's AI capabilities to predict future sales trends.
*   **Real-Time Data Integration:** Integrate with Amazon's API (if available) to enable real-time data updates.
*   **Mobile Optimization:** Optimize the dashboard for mobile viewing on the Power BI mobile app.
*   **User Authentication:** Add user roles to limit access to certain product page and functions.
*   **More granular data:** Obtain more granular data to better understand specific product line sales.
*   **Add new features:** Add product sentiment analysis to better assist sales.

## Author

[Himanshu Solanki]

*   [www.linkedin.com/in/himanshu-solanki-88b979288]

