# PowerBI-Sales-Analysis-Dashboard
Interactive Sales Analysis Dashboard built in Power BI using DAX, Power Query, and AI visuals.

This Power BI dashboard provides a unified view of sales performance across products, customers, and regions.
It demonstrates advanced data modeling, Power Query transformations, and DAX-driven analytics for actionable insights.

🧱 Key Features

Multi-page dashboard with interactive visuals for sales, profit, and customer trends

Semantic data model using star schema (FactSales, DimProduct, DimCustomer, DimDate)

Advanced DAX measures for KPIs — YoY Growth, Profit Margin %, Avg Order Value

AI visuals: Key Influencers, Decomposition Tree, Clustering, Smart Narrative

Data transformation: Power Query (M) scripts for cleaning, merging, and parameterizing sources

Dynamic interactivity: Drill-through, Tooltips, and Q&A for self-service analytics


Example DAX Measures
Total Sales = SUM(FactSales[SalesAmount])
Profit Margin % = DIVIDE([Total Profit], [Total Sales])
YoY Growth = 
VAR PrevYearSales = CALCULATE([Total Sales], DATEADD(DimDate[Date], -1, YEAR))
RETURN DIVIDE([Total Sales] - PrevYearSales, PrevYearSales)

Visual Pages

Sales Overview – KPIs, YoY trend lines, and drill-throughs

Product Details – Category-level insights, clustering, and binning

Anomaly Detection – AI-driven outlier and error bar visuals

Key Influencers & Decomposition – Root cause and drill-down analytics

Smart Narrative – Automated executive summary

Preview: 
![WhatsApp Image 2025-10-22 at 9 55 58 PM](https://github.com/user-attachments/assets/bc653b40-2474-4ad9-bb02-32ce680973ca)

![WhatsApp Image 2025-10-22 at 9 56 41 PM](https://github.com/user-attachments/assets/e643927e-ebe6-4ca3-a8c7-39c43c11d884)

![WhatsApp Image 2025-10-22 at 9 57 23 PM](https://github.com/user-attachments/assets/36b94a8d-e53e-4d70-89a9-9ba27452dd1d)


🛠 Tools & Tech

Power BI Desktop, DAX, Power Query (M), Power BI Service, DAX Studio, SharePoint


Business Impact

Enabled 360° view of company sales and profitability

Reduced manual reporting time by 40%

Revealed revenue drivers and discounting impact via AI visualizations
