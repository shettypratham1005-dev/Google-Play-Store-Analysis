Google Play Store Analysis — Task 3
## Project Overview

This task extends the original Google Play Store Analysis project by implementing an advanced dual-axis visualization using Power BI.
The dashboard compares Average Installs and Average Revenue for Free vs Paid apps across the Top 3 App Categories, using multiple business-driven filters and dynamic time-based visibility logic.

## Dataset Used

File: Play Store Data.csv
Source: Google Play Store dataset

## Key Columns Used:

App

Category

Type (Free / Paid)

Rating

Reviews

Installs

Price

Size

Android Version

Content Rating

## Data Cleaning & Transformations

The following transformations were applied using Power Query & DAX:

Converted Installs and Reviews to numeric values

Cleaned Size column (removed 'M' and converted to numeric)

Converted Price to numeric

Created Revenue column

Created App_Len column to calculate app name length

Handled missing and error values

Converted Last Updated column to Date format

## Calculated Columns & Measures (DAX)
Calculated Columns:

Revenue = Price × Installs

App_Len = Length of App Name

Paid_Free = Free / Paid classification

Measures:

Avg Installs

Avg Revenue

Total Installs

Total Revenue

Average Rating

Time-based visibility measure (Show Chart)

## Visualization Implemented
Dual-Axis Chart:

Column Axis: Average Installs

Line Axis: Average Revenue

Legend: Free vs Paid Apps

Categories: Top 3 App Categories by total installs

## Business Filters Applied

The following filters were implemented as per task instructions:

Installs ≥ 10,000

Revenue > 0

Android Version > 4.0

App Size > 15 MB

Content Rating = Everyone

App Name Length ≤ 30 characters

Top 3 Categories based on total installs

## Time-Based Visibility Logic

The visualization is dynamically displayed only between 1 PM IST and 2 PM IST using a DAX-based time filter.

Outside this time window, the chart automatically disappears from the dashboard, ensuring time-controlled reporting behavior.

- KPIs Added

Total Installs

Total Revenue

Average Rating

These KPIs enhance dashboard readability and business insights.

## Tools & Technologies Used

Power BI Desktop

Power Query Editor

DAX (Data Analysis Expressions)

Microsoft Excel (for dataset review)

- Dashboard Preview

<img width="1915" height="1079" alt="PowerBI (2)" src="https://github.com/user-attachments/assets/c202067a-b824-4c07-a280-57f7f7b685d8" />


## Conclusion

This task demonstrates advanced data transformation, business rule filtering, dual-axis visual comparison, and dynamic time-based control using Power BI.
The dashboard provides actionable insights into Free vs Paid app performance across leading app categories.
