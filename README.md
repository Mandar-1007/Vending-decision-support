# Overview

This project presents a profit-focused decision support dashboard built in Tableau for a smart vending machine company.
The dashboard enables executives to explore and compare **net profit performance** across vending machines, product categories, and time periods.
It leverages advanced Tableau features like **parameters**, **sets**, **hierarchies**, and **trend analysis** to deliver actionable insights.
This repository holds the Tableau workbook (.twbx) file containing all interactive visualizations.

# Tools Used

- **Tableau Desktop**
- **Tableau Public**
- **Microsoft Excel**

# Dashboard Visuals & Business Insights

**Final Dashboard**

![image](https://github.com/user-attachments/assets/cd2d6591-b4fb-4f84-b8e0-57b144c0c14b)

*View the Interactive Dashboard on Tableau Public:* https://public.tableau.com/app/profile/mandar.nadkarni/viz/Profit-DrivenDecisionSupportSystemforSmartVendingManagement/ProfitAnalysisDashboard

# Business Questions Answered

1. **Which vending machines are highly profitable?**

![image](https://github.com/user-attachments/assets/e589ec7a-8d85-4ee2-8a38-7715bdd16b4d)

This bar chart compares the net profit of each vending machine, using a dynamic Profitability Cut-off slider. Machines generating profit above the cut-off (e.g., $4,200) are highlighted in green as "High Profit," while others are marked in red. A reference line visually indicates the cut-off value. The chart is interactive—clicking on any machine filters other dashboard elements to show only relevant products and trends for that machine

2. **Which product categories and products are most profitable across locations?**

![image](https://github.com/user-attachments/assets/d2ac2af8-2dc4-4b4c-bb7a-7d3988b50ef1)

This hierarchical bar chart breaks down net profit by Product Category → Product Description across different vending machine locations (Company, Mall, School). Users can drill down to analyze individual product performance within each category, and use filters to isolate specific locations. Products like Lays and Doritos show strong performance, especially in school environments. The chart is interactive—selecting a product category or location updates other dashboard visuals for focused insight.c

3. **How has total profit changed over time?**

![image](https://github.com/user-attachments/assets/bf017451-08c9-4319-86b5-fee091e70a4e)

This scatter plot shows daily net profit over time using a custom Actual Date field. A 4th-degree polynomial trend line with confidence bands helps visualize profit fluctuations and potential seasonal patterns. The chart supports interactivity—users can apply date filters to focus on specific time periods, automatically updating other dashboard views to reflect the selected range.

# Additional Insight: Custom Features & Calculations

- Created a calculated field **Units Sold** to account for stale products before computing net profit.
- Built a **Profitability Set** to dynamically segment machines based on user-defined thresholds.
- Developed a custom **Formatted Date** field using year, month, and day columns to enable accurate trend analysis.
- Integrated interactive filters across the dashboard for machines, products, and dates.

> These features empower business users to make data-driven decisions around inventory planning, machine placement, and product selection.


# Dashboard Interactivity

The dashboard is designed with cross-filtering capabilities and dynamic interactivity, enabling executives to explore net profit insights in a flexible and intuitive way:

**1) Machine-Level Filtering**
- Clicking on a vending machine bar in the "Net Profit vs. Machine ID" chart updates the other two charts (Product Category and Trend Analysis) to show only data relevant to that selected machine
- This helps management understand which products and locations are contributing to a specific machine's profitability.

**2) Category/Product-Level Filtering**
- Clicking on a product category or drilling down to a specific product updates the Machine Profitability and Trend charts
- This allows users to analyze which machines and time periods are driving profits for a specific product line.

**3) Date Range Filtering**
- The trend analysis chart includes a date filter that allows users to select a specific time range.
- Once a range is selected, the Product and Machine charts automatically adjust to reflect only the profits recorded within that period.
- This enables seasonality and time-based comparisons.

**4) Location Filter (Dropdown)**
- A dropdown filter lets users isolate data by location type (e.g., School, Mall, Company).
- This affects the Product Category chart and allows focused comparison across different environments.


# Conclusion

The Profit-Driven Decision Support System for Smart Vending Management dashboard empowers stakeholders with a centralized, interactive view of business performance. By analyzing net profit across machines, locations, and product categories, and by tracking profit trends over time, the company can make informed decisions to:
- Optimize machine placements and inventory strategies
- Identify and scale high-performing products
- Reduce stales and losses through targeted interventions
- Track profitability goals dynamically using parameter-driven cut-offs

This dashboard not only enhances visibility into operational efficiency but also supports data-driven decision-making for sustainable growth in the vending business.
