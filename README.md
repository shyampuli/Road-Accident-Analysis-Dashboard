🚗 Road Accident Analysis Dashboard

A dynamic and interactive Power BI dashboard designed to provide deep insights into road accident patterns across the years 2021 and 2022, focusing on accident severity, vehicle involvement, environmental factors, and geographical distribution.

📝 Short Description / Purpose

The Road Accident Analysis Dashboard enables users to analyze and compare road safety data between 2021 and 2022. It highlights key performance indicators (KPIs) such as total casualties, accident severity, vehicle type breakdowns, and environmental conditions.
This tool is intended for traffic authorities, urban planners, policymakers, and data analysts aiming to identify high-risk areas, monitor year-over-year changes, and develop strategies for improving road safety.

⚙️ Tech Stack

The dashboard was built using the following tools and technologies:

📊 Power BI Desktop – Main data visualization platform used to design and publish the dashboard.

📂 Power Query Editor – Used for data cleaning, transformation, and column-level editing.

🧠 DAX (Data Analysis Expressions) – Applied for calculated measures, YOY analysis, and time intelligence.

🧩 Data Modeling – Established relationships between accident and calendar tables for dynamic time-based reporting.

🖼️ PowerPoint – Used to design a customized dashboard background layout.

📁 File Formats – .pbix (dashboard), .xlsx (dataset), .pptx (background), .jpg (preview image).

📂 Data Source

Source: Provided client dataset titled Road Accident Data.xlsx

The dataset contains detailed information on traffic accidents across the United Kingdom for the years 2021 and 2022, including:

Date and time of accident

Number of casualties and severity levels

Vehicle type and road type

Area classification (Urban/Rural)

Light and weather conditions

Geographic location coordinates

Each record represents an individual road accident event with associated attributes used for aggregation and visualization.

🌟 Features / Highlights
• Business Problem

Road traffic accidents contribute significantly to annual fatalities and injuries. Authorities lacked a unified system to visualize accident trends, assess the impact of road conditions, and identify areas requiring intervention.

Key questions addressed:

What is the trend in total casualties and accidents compared to the previous year?

Which vehicle types and road categories are most involved in accidents?

How do environmental conditions (day/night, rural/urban) influence casualty rates?

Which regions report the highest number of casualties?

• Goal of the Dashboard

To deliver an interactive and data-driven analytical tool that:

Provides clear visibility into yearly accident trends and casualty severity.

Helps traffic management departments identify risk-prone vehicle and road types.

Enables geospatial accident mapping for targeted safety improvements.

Supports policy-level decision making using comparative analytics between years.

• Walkthrough of Key Visuals

1. KPI Summary Cards (Top Row)
Displays primary and secondary KPIs including:

Total Casualties: 195.7K (↓11.9%)

Total Accidents: 144.4K (↓11.7%)

Fatal Casualties: 2.9K (↓33.3%)

Serious Casualties: 27K (↓16.2%)

Slight Casualties: 165.8K (↓10.6%)

2. Casualties by Vehicle Type (Left Panel)
A vertical bar chart highlighting casualties by type:

Cars: 155,804

Bikes: 15,610

Vans: 15,905

Buses: 6,573

Agricultural & Others: 1,845 combined

This visual identifies vehicle categories most prone to accidents.

3. Monthly Trend Comparison (Center Panel)
Line graph comparing Current Year (2022) and Previous Year (2021) casualties month-by-month.
Provides seasonal trend analysis to identify high-incident periods (e.g., summer peaks).

4. Casualties by Road Type (Bottom Left)
Horizontal bar chart displaying total casualties per road category:

Single Carriageway: 145K

Dual Carriageway: 32K

Roundabout: 13K

Slip/One-way Roads: ~3K each

Helps pinpoint which infrastructure types pose greater risk.

5. Area & Light Condition Analysis (Bottom Center)
Two donut charts showing:

Urban vs Rural Distribution: Urban (61.95%), Rural (38.05%)

Light Condition: Day (73.84%), Night (26.16%)

These visuals show the influence of environment and visibility on accidents.

6. Casualties by Location (Right Panel)
An interactive map visualization of accident density across the United Kingdom.
Hotspots like London, Birmingham, and Manchester indicate regions with higher incident counts.

• Business Impact & Insights

📉 Reduction in Overall Casualties: A notable decline of 11.9% YoY demonstrates improving safety initiatives.

🚗 Car-related accidents dominate total casualties, emphasizing the need for stricter speed and seatbelt regulations.

🌇 Urban areas account for nearly 62% of total casualties, highlighting city congestion and high traffic density.

🌞 Daytime accidents are almost triple those at night, indicating exposure duration as a key factor.

🛣️ Single carriageways remain the most accident-prone road type, warranting infrastructure redesign and lane management strategies.

🧮 Key DAX Calculations (Sample)
-- Current Year Casualties
Current Year Casualties =
TOTALYTD(SUM(Data[Number_of_Casualties]), 'Calendar'[Date])

-- Previous Year Casualties
Previous Year Casualties =
CALCULATE(SUM(Data[Number_of_Casualties]), SAMEPERIODLASTYEAR('Calendar'[Date]))


Additional calculations were built for:

YOY Growth %

Severity-level breakdowns (Fatal, Serious, Slight)

Vehicle and Road Type aggregations

Date hierarchy using Calendar Table

🧰 Tools & Technologies
Category	Tool
Data Visualization	Power BI Desktop
Data Cleaning	Power Query Editor
Calculations	DAX (Data Analysis Expressions)
Design	PowerPoint
Data Source	Excel (.xlsx)
🗂️ Project Files
File Name	Description
Road Accident Dashboard.pbix	Power BI report file
Road Accident Data.xlsx	Original dataset used for analysis
Dashboard Background.pptx	Custom dashboard background design
Screenshot_2025-10-24.jpg	Preview image of the final dashboard

(Upload all files in the GitHub repository and link them here.)

🧭 Conclusion

The Road Accident Analysis Dashboard successfully provides a holistic view of traffic accident trends, patterns, and contributing factors.
By integrating data visualization, geospatial analysis, and year-over-year metrics, it empowers decision-makers to enhance safety strategies, optimize traffic policies, and focus resources on high-risk zones.

📧 Author Information

Author: Shyamprasad Puli
![Dashboard Preview](
