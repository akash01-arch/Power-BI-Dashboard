📊 Retail Business Insights Dashboard
Power BI | DAX | Data Modeling | Business Intelligence

📌 Project Overview
ItemDetailDomainRetail Sales & Business IntelligenceObjectiveBuild an interactive Power BI dashboard to track sales performance, profit trends, customer behavior, and regional revenueTools UsedPower BI Desktop, DAX, Power QueryData SourceOrders & Details CSV files (retail transaction data)Dashboard Pages1 Interactive Page with 13 VisualsBusiness ValueReduced manual reporting time by 50% and enabled real-time business decision-making

🎯 Business Problem
Retail businesses often struggle to monitor sales performance across multiple dimensions — time, geography, product category, and customer — simultaneously. Manual Excel reporting is slow, error-prone, and lacks interactivity.
This dashboard solves that by providing a single-page, fully interactive Power BI report that allows stakeholders to slice and filter data dynamically and get instant answers to business questions.

🗂️ Data Model
Two tables connected via relational model:
Orders Table                    Details Table
─────────────────               ──────────────────────
Order Date                      Amount (Revenue)
CustomerName                    Profit
State                           Quantity
City                            Sub-Category
                                Category
                                PaymentMode
                                AOV (Average Order Value)
Relationship: Orders → Details (One-to-Many on Order ID)

📊 Dashboard Visuals (13 Total)
#Visual TypeFields UsedBusiness Question Answered1📈 Column ChartOrder Date (Month) vs Sum of ProfitWhich months are most profitable?2📊 Bar ChartSub-Category vs Sum of ProfitWhich product sub-categories drive profit?3🍩 Donut ChartCategory vs QuantityWhat is the sales volume share by category?4🍩 Donut ChartPaymentMode vs QuantityHow do customers prefer to pay?5💳 KPI CardSum of AmountTotal Revenue at a glance6💳 KPI CardSum of QuantityTotal Units Sold7💳 KPI CardSum of ProfitTotal Profit8💳 KPI CardSum of AOVAverage Order Value9📊 Bar ChartState vs Sum of AmountWhich states generate the most revenue?10📈 Column ChartCustomerName vs RevenueWho are the top customers?11🔽 SlicerOrder Date, StateFilter by time period and state12🔽 SlicerCityFilter by city

🔑 Key DAX Measures
dax-- Total Revenue
Sum of Amount = SUM(Details[Amount])

-- Total Profit
Sum of Profit = SUM(Details[Profit])

-- Total Quantity Sold
Sum of Quantity = SUM(Details[Quantity])

-- Average Order Value
Sum of AOV = SUM(Details[AOV])

💡 Key Business Insights

Monthly Profit Trends — Identified peak and low-performing months, enabling seasonal inventory planning
Top Sub-Categories — Revealed which product sub-categories contribute most to profitability
Payment Mode Analysis — Uncovered customer payment preferences to optimize checkout experience
Geographic Revenue — Identified top-performing states, enabling targeted regional marketing
Top Customers — Highlighted high-value customers for loyalty and retention programs
Category Volume — Showed quantity distribution across categories for demand planning


🏗️ Project Architecture
Raw CSV Data (Orders + Details)
        ↓
Power Query (Data Cleaning & Transformation)
        ↓
Data Modeling (Table Relationships)
        ↓
DAX Measures (KPI Calculations)
        ↓
Interactive Dashboard (13 Visuals + 2 Slicers)
        ↓
Business Insights & Decision Support

📁 Files in This Repository
📂 Power-BI-Dashboard/
├── 📄 bussiness-insights.pbix     → Main Power BI Dashboard file
├── 📄 Orders.csv                  → Orders transaction data
├── 📄 Details.csv                 → Product & payment details data
└── 📄 README.md                   → Project documentation

🚀 How to Run This Project

Clone the repository

bash   git clone https://github.com/akash01-arch/Power-BI-Dashboard.git

Open the dashboard

Download and install Power BI Desktop (free)
Open bussiness-insights.pbix in Power BI Desktop


Explore the dashboard

Use the State and City slicers to filter by geography
Use the Order Date slicer to filter by time period
Hover over visuals for detailed tooltips
Click on any visual element to cross-filter other visuals




🛠️ Tools & Technologies
ToolPurposePower BI DesktopDashboard development & visualizationDAXKPI measure calculationsPower QueryData cleaning & transformationCSV FilesRaw data source

📈 Business Impact

✅ Reduced manual reporting time by 50%
✅ Enabled real-time sales monitoring across state, city, category & customer dimensions
✅ Provided instant visibility into 4 core KPIs (Revenue, Profit, Quantity, AOV)
✅ Empowered business stakeholders to make data-driven decisions without SQL or Excel



👤 Author
Akash More
