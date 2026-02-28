## Category-Wise and Time-Driven App Analytics using Power BI
## Project Overview

This project focuses on analyzing the Google Play Store dataset using Power BI. The goal is to clean, transform, and visualize the data to gain actionable insights into app performance, installs, ratings, size distribution, sentiment subjectivity, and category trends.

The final deliverable is an interactive Power BI dashboard containing dynamic filters, advanced visualizations, category translation, and time-based visual control.

## Dataset

Source: Google Play Store Dataset
Main Columns Used:

App

Category

Rating

Reviews

Installs

Size

Sentiment Subjectivity

Last Updated

## Data Cleaning & Preprocessing

Performed using Power Query Editor:

Removed null and invalid records

Converted Installs and Reviews to numeric format

Cleaned Size column and converted to MB

Handled missing rating values

Created derived column: Size_MB

Created calculated column: Sentiment_Subjectivity

## Visualizations Implemented
1)Bubble Chart (Scatter Plot)

Shows relationship between:

X-axis: App Size (MB)

Y-axis: Rating

Bubble Size: Installs

Legend: Category

This visual highlights how app size and installs impact user ratings.

2️)Category-Based Filtering

Filtered:

Rating > 3.5

Installs > 500,000

Selected categories for focused analysis

3️)Category Translation (Multi-Language)

Applied dynamic translation using DAX calculated column:

Original	Translated
BEAUTY	सुंदरता (Hindi)
BUSINESS	வணிகம் (Tamil)
DATING	Verabredung (German)

This enhances global usability and localization support.

4️) Time-Based Visualization Control

Bubble chart is visible only between 5 PM and 7 PM IST using a DAX time-based measure.

This demonstrates dynamic visualization control based on real-time conditions.

##  Key DAX Measures & Columns
🔹 Category Translation Column
Translated_Category =
SWITCH(
    TRUE(),
    'Play Store Data'[Category] = "BEAUTY", "सुंदरता (Beauty)",
    'Play Store Data'[Category] = "BUSINESS", "வணிகம் (Business)",
    'Play Store Data'[Category] = "DATING", "Verabredung (Dating)",
    'Play Store Data'[Category]
)

🔹 Time Control Measure
Show Bubble Chart =
VAR CurrentHour = HOUR(UTCNOW()) + 5.5
RETURN
IF(CurrentHour >= 17 && CurrentHour < 19, 1, 0)

## Dashboard Features

Interactive filters

Dynamic bubble chart

Category translation

Time-based visibility

Responsive layout

Business-friendly UI

## Business Insights Generated

Identified top-performing app categories

Analyzed impact of app size on ratings

Studied install trends across categories

Improved international usability using translation

Implemented operational control using time filtering

## Tools & Technologies Used

Power BI Desktop

Power Query Editor

DAX (Data Analysis Expressions)

Data Visualization Techniques

## Project Deliverables

.pbix Power BI dashboard file

Dataset (CSV)

README documentation

## Outcome

Successfully created a professional interactive dashboard with advanced analytics, dynamic control, and multilingual support, suitable for business decision-making and portfolio demonstration.
