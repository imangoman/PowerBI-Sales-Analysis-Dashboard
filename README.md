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

🛠 Tools & Tech

Power BI Desktop, DAX, Power Query (M), Power BI Service, DAX Studio, SharePoint


Business Impact

Enabled 360° view of company sales and profitability

Reduced manual reporting time by 40%

Revealed revenue drivers and discounting impact via AI visualizations
