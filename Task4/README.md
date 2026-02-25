## Time Series Trend Analysis & Dynamic Dashboard Control

##Project Overview
This task focuses on performing time series analysis on Google Play Store app installs, identifying monthly growth trends, applying advanced filtering logic, and creating a dynamic Power BI dashboard that displays data only during a specific time window (6 PM – 9 PM IST).

## Dataset
File used:
Play Store Data.csv

## Main columns used:
App

Category

Installs

Reviews

Last Updated

Data Cleaning Process

Removed missing and invalid values

Converted Installs column into numeric format

Converted Last Updated column into datetime format

Extracted Month-Year for time series grouping

## Applied advanced filtering conditions:

Reviews > 500

App name does not start with X, Y, Z

App name does not contain letter S

Category starts only with E, C, or B

## Data Transformations

Created Month-Year column for trend analysis

Aggregated monthly installs

Calculated Month-over-Month growth percentage

Applied category-based translation logic for visualization

## Analysis Performed

Time series trend analysis of installs

Category-wise monthly growth analysis

Identification of high-growth periods (>20%)

Comparison of install trends across categories

## Category Translation (Visualization Level)
Original Category	Display Language	Translated Name
Beauty	Hindi	सौंदर्य
Business	Tamil	வணிகம்
Dating	German	Partnersuche

## Visualization

The following visualizations were created:

Monthly Time Series Line Chart

Category-wise trend comparison

Growth highlighting (>20%)

Multilingual category representation

Dynamic dashboard visibility control

## Time Restriction Logic

The dashboard visuals are displayed only between 6 PM IST and 9 PM IST using the following DAX logic:

Show Chart =
VAR CurrentHour = HOUR(NOW()) + 5.5
RETURN
IF(CurrentHour >= 18 && CurrentHour < 21, 1, 0)

Outside this time range, visuals remain hidden, adding dynamic control to the dashboard.

## Tools Used

Python

Pandas

Matplotlib

Jupyter Notebook

Power BI

DAX

## Conclusion

Clear monthly install growth trends were observed.

Certain categories showed high growth spikes (>20%).

Advanced filtering & transformation logic improved data quality.

Time-based dashboard visibility added automation and business logic control.
