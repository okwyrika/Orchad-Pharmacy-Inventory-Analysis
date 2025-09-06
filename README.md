# Orchad-Pharmacy-Inventory-Analysis

## Project Overview
This project focuses on analyzing pharmacy inventory data from Orchad Pharmacy.
The goal was to clean, transform, and analyze the dataset to generate insights into drug sales, inventory management and overall business performance.
The analysis was carried out using Excel/power query for cleaning/transformation and PowerBI for visualisation.

## Objectives
- Clean raw pharmacy data for accuracy and consistency.
- To build an interactive dashboardto monitor sales and inventory.
- To analyze the Orchad pharmacy inventory to identify underperforming assets (slow-moving, low-profit 
items) and key profit drivers (fast-moving, high-profit items).
- To propose data-driven recommendations for optimizing purchasing decisions 
to improve overall profitability and inventory efficiency.

## Tools Used
- Microsoft Excel/Power Query -> Data cleaning, transformation, preprocessing.
- PowerBI -> Data modelling, visualization, and dashboard creation.

## Dataset
- Source: proprietory Orchad pharmacy inventory data.
- Size: 3482 rows, 32 columns.
- Key Columns:
     - `Department` - Name of drug group.
     - `On-Hand Qty`- Total number of Units at hand.
     - `On-Order Qty` - Total number of Units ordered.
     - `Ext Cost` - Total Cost of Units
     - `Ext Price`- Total Price of Units.
     - `Profit`- Total Profit of Units.
     - `Vendor`- Name of Vendor.
     - `Item Name` - Name of Medication.
     - `Quantity` - Total amount of Units.
     - `Order cost`- Total amount of Order.
     - `Margin`- Margin at which Units are sold.
     - `Regular Price`- Amount a unit is sold.
     - `Unit Profit`- Profit made for a Unit.
     - `Profit margin`- Margin at which profit is made.
 

# Data Cleaning and Transformation
## In PowerQuery
- Standardized data formats
- Created calculated fields.
- Removed Negative numerical values.
- Removed fields that are not needed for my analysis.

## In Power BI
- Imported cleaned Excel File.
- Created KPIs using DAX:
     - `Total Sales = SUM(Sheet1[Ext Price])`
     - `Total Quantity = SUM(Sheet1[Quantity])`
     - `Total Profit = SUM(Sheet1[Profit])`
     - `Average Profit Margin = AVERAGE(Sheet1[Profit Margin %])`
     - `Total Profit Margin = SUM(Sheet1[Profit Margin %])`



## Dashboard Features
- KPIs: Total Sales, Total Quantity, Total Profit, Average Profit Margin, Total profit Margin.
- Visualization:
    - On-Order Qty By Vendor Name.
    - 10 Most Costly Items.
    - Top 5 Department.
    - Sum of Profit By Vendor Name.
    - 10 Most Profitable Items.

## Key Findings
- The Pharmacy generates strong revenue with over 29% profit Margin.
- Grams Pharma dominates On-Order Qty and Profit contribution which 
poses an over dependence risk.
- Augmentin 625mg & 1g, Vit-C white 100mg, and Rocephin are among 
the most costly and profitable items.
- Zinc have huge stocks compared to sales.
- The Drug Department dominates profit contribution.

## Recommendations
- Reduce purchase volumes for slow-moving products like Zinc and invest more in fast 
moving drugs like Augmentin and Rocephin.
- Negotiate better terms with Grams Pharma while actively onboard secondary 
vendors to avoid supply chain dependency.
- Reassess high-cost but low-margin products to see if price adjustments can improve 
profitability. Consider promotions or slight markups on fast movers that are less price 
sensitive.
- Prioritize fast-moving ,high-margin drugs while trimming down orders for slow
moving stock.
- Implement a stock level threshold alert system for Augmentin, Rocephin and 
Ampiclox B/C.
- The Drug Department drives most profit but System and Other Departments are 
underperforming. Explore if this is due to low demand or stocking inefficiencies and 
either boost marketing or reduce orders in underperforming Departments.

## Portfolio
[View the full PDF Portfolio](https://github.com/okwyrika/Orchad-Pharmacy-Inventory-Analysis/blob/main/Orchad%20pharmacy%20project%20analysis.pdf)
