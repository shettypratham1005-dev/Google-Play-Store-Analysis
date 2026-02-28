## Time Controlled Multilingual Stacked Area Visualization using Power BI
## Project Overview

This task focuses on creating an advanced stacked area visualization to analyze the cumulative growth of app installs over time for selected app categories.
The dashboard applies strict business filters, multilingual category translations, dynamic highlighting of high-growth periods, and time-based visualization control to ensure intelligent and interactive reporting.

## Dataset Used

File: Play Store Data.csv
Source: Google Play Store Dataset

Key Columns Used

App

Category

Rating

Reviews

Installs

Size

Last Updated

## Data Cleaning & Transformations

The following transformations were applied using Power Query & DAX:

Converted Installs, Reviews, Rating, and Size into numeric format

Cleaned Installs column by removing + and ,

Converted Size column into MB numeric values

Converted Last Updated column to Date format

Handled missing and invalid values

Created Month-Year column for time-series analysis

## Business Rules & Filters Applied

The following filters were applied before visualization:

Rating ≥ 4.2

Reviews > 1,000

App name must not contain any numeric characters

Category must start with letter “T” or “P”

App Size between 20 MB and 80 MB

## Category Translation Logic

To improve global readability, category names were translated as:

Original Category	Translated Language
Travel & Local	French → Voyage et Local,
Productivity	Spanish → Productividad,
Photography	Japanese → 写真.

These translated values are displayed directly in the chart legend.

## Calculated Measures & DAX Logic
1.Measures Created:

Total Installs

Month-over-Month Growth %

Highlight Flag (Growth > 25%)

Time-Based Visibility Logic

**Time Control Logic:

The visualization appears only between 4 PM IST and 6 PM IST.
Outside this time window, the chart is automatically hidden from the dashboard.

## Visualization Implemented
1.Stacked Area Chart

X-Axis: Month-Year

Y-Axis: Total Installs

Legend: Translated Category Names

2.Special Enhancements

Dynamic color intensity increase for months where installs grow more than 25% MoM

Multilingual legend for better interpretability

Time-controlled dashboard visibility

## Tools & Technologies Used

Power BI Desktop

Power Query Editor

DAX (Data Analysis Expressions)

Microsoft Excel (Dataset Review)

## Conclusion

This task demonstrates advanced Power BI skills, including:

Complex data transformation

Business-driven filtering

Time-series trend analysis

Multilingual dashboard design

Dynamic time-based visualization control

The final dashboard delivers highly actionable insights into cumulative app growth patterns across premium categories while ensuring professional-level interactivity and governance.
