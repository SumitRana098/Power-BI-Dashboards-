📌 PlanetSpark Sales Funnel Analytics | Power BI Dashboard
📁 Project Overview

This project analyzes PlanetSpark’s end-to-end sales funnel, covering performance from Leads → Calls → Demos → Sales → Revenue.
The dashboard highlights key KPIs, agent performance, revenue distribution, and conversion insights to support strategic decision-making.

This project demonstrates skills in:

Data cleaning

Power BI data modeling

DAX measures

UI/UX dashboard design

Analytical storytelling

📊 Key Business Questions

How many leads were generated, and how many converted into sales?

What is the overall sales funnel performance?

Which agents are performing the best?

How does revenue vary across regions?

What is the daily revenue trend?

How close is the team to achieving revenue targets?

📈 Dashboard Features
1. KPI Summary

Total Leads

Total Calls

Total Demos

Total Sales

Total Revenue

Total Target Achievement %

2. Sales Funnel

Visualizing drop-offs at each stage:

Leads → Calls → Demos → Sales

3. Daily Revenue Trend

Line chart showing day-wise revenue movement.

4. Agent Performance

Comparison of:

Revenue by Agent

Sales by Agent

Efficiency score (custom DAX)

5. Revenue by Region

Bar chart showing revenue contribution from different regions.

6. Dynamic Filter Panel

Includes slicers for:

Date range

Region

Agent

Product

Styled inside a floating filter container with a close/open icon for usability.

🧠 Data Model
calendar
   |
leads
 /   |   \
calls demos sales
         |
     AgentMonth
         |
      targets


The model supports accurate filtering, time intelligence, and clean relationships.

🧮 Important DAX Measures Used
Total Revenue
Total Revenue = SUM(sales[revenue])

Total Sales
Total Sales = COUNTROWS(sales)

Total Calls
Total Calls = COUNTROWS(calls)

Total Leads
Total Leads = COUNTROWS(leads)

Demo Conversion %
Demo Conversion(%) = DIVIDE([Total Demos], [Total Calls])

Target Achievement %
Target Achievement % =
DIVIDE([Total Revenue], [Total Target])

Agent Efficiency
Agent Efficiency =
([Total Sales] * 0.4) + ([Total Revenue] * 0.6)

📁 Tools & Technologies

Power BI

Power Query

DAX

Excel

Figma (for background design)
