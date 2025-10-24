🚗 Road Accident Analysis Dashboard (Power BI)

📊 Project Overview

This Power BI project analyzes road accident data for the years 2021 and 2022, providing actionable insights into accident patterns, severity, vehicle involvement, and environmental conditions.
The dashboard enables stakeholders to identify key metrics, trends, and high-risk areas to support road safety decisions and policy making.

🧩 Project Objectives

The client required an interactive Road Accident Dashboard to visualize:

Primary KPIs

Total Casualties and Total Accidents (Current Year)

Year-over-Year (YOY) growth for both

Accident Severity Breakdown

Fatal, Serious, and Slight Casualties (with YOY comparison)

Vehicle Type Analysis

Total Casualties by type (Car, Bike, Bus, Van, etc.)

Monthly Trends

Comparison of Current Year (CY) vs Previous Year (PY) casualties

Road Type Analysis

Casualties across Single Carriageway, Dual Carriageway, Roundabout, etc.

Geographical Insights

Casualties and Accidents by Location (Map visualization)

Environmental Factors

Distribution by Urban/Rural areas and Day/Night light conditions

📂 Dataset Information

File Name: Road Accident Data.xlsx

Data Source: Provided by client (2021–2022 accident records)

Key Columns:

Accident Date

Number of Casualties

Accident Severity

Vehicle Type

Road Type

Urban/Rural

Light Conditions

Location Details

🧹 Data Preparation
1. Data Cleaning

Performed using Power Query Editor:

Removed duplicates

Standardized column names

Fixed data type mismatches

Handled missing values

2. Data Processing

Created a Calendar Table for time-based calculations:

Calendar = CALENDAR(MIN(Data[Accident Date]), MAX(Data[Accident Date]))
Year = YEAR('Calendar'[Date])
Month = FORMAT('Calendar'[Date], "mmm")

🔗 Data Modelling

Established relationships between tables:

Accident Table → Calendar Table (Many-to-One relationship)

This enabled the use of time intelligence functions for YTD and YOY calculations.

📈 DAX Measures (Sample)
Current Year Casualties =
TOTALYTD(SUM(Data[Number_of_Casualties]), 'Calendar'[Date])

Previous Year Casualties =
CALCULATE(SUM(Data[Number_of_Casualties]), SAMEPERIODLASTYEAR('Calendar'[Date]))


Additional DAX formulas were created for:

YOY Growth %

Fatal/Serious/Slight Casualties

Road Type & Vehicle Type Summaries

🎨 Data Visualization
Tools Used:

Power BI Desktop

PowerPoint (for background design)

Dashboard Sections:

KPI Cards: Total Casualties, Total Accidents, Fatal/Serious/Slight breakdown

Line Chart: CY vs PY Casualties monthly trend

Bar Charts: Road Type & Vehicle Type breakdowns

Donut Charts: Urban/Rural and Light Conditions

Map Visualization: Casualties by Location (UK region-based)

📉 Insights Highlight

195.7K Total Casualties recorded, down 11.9% YoY

2.9K Fatal Casualties (–33.3% YoY)

Car accidents caused majority (155K+) casualties

Urban areas contributed 61.95% of total casualties

Daytime accidents were 73.8%, significantly higher than at night

Single Carriageways were the most accident-prone road type

⚙️ Tools & Technologies

🧠 Power BI – Data Visualization & Analysis

🧮 DAX (Data Analysis Expressions) – Calculations

🧼 Power Query – Data Cleaning & Transformation

🖼️ PowerPoint – Dashboard Background Design

🏁 Conclusion

This dashboard empowers stakeholders to:

Monitor yearly trends and accident severity

Identify high-risk road types and conditions

Improve road safety through data-driven insights

📧 Contact

Author: Shyamprasad Puli
