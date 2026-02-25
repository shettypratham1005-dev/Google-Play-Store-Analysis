📊 Task 4 – Time Series Trend Analysis & Dynamic Dashboard Control
📌 Objective

To analyze monthly install trends over time using Python and Power BI, apply advanced filtering conditions, and build a dynamic dashboard that shows data only during a specific time window (6 PM – 9 PM IST).

🛠 Tools & Technologies

Python (Jupyter Notebook)

Pandas

Matplotlib

Power BI

DAX

📂 Dataset

Google Play Store Dataset

Source: Kaggle

File: Play Store Data.csv

🧹 Data Cleaning Steps

Removed missing and invalid values

Converted Installs into numeric format

Converted Last Updated to DateTime

Extracted Month-Year for time series analysis

Filtered apps based on:

Reviews > 500

App Name does not start with X, Y, Z

App Name does not contain letter "S"

Category starts with E, C, or B

📊 Analysis Performed
1. Time Series Trend Analysis

Aggregated total installs monthly

Segmented trend by app category

Created line chart to visualize growth

2. Growth Highlighting

Calculated Month-over-Month growth (%)

Highlighted areas where growth > 20%

3. Category Translation (Visualization Level)
Original Category	Display Language	Translated Name
Beauty	Hindi	सौंदर्य
Business	Tamil	வணிகம்
Dating	German	Partnersuche
4. Dynamic Dashboard Visibility (Power BI)

Dashboard is visible only between 6 PM to 9 PM IST using DAX measure logic.

Show Chart =
VAR CurrentHour = HOUR(NOW()) + 5.5
RETURN
IF(CurrentHour >= 18 && CurrentHour < 21, 1, 0)
📈 Dashboard Output

Time series line chart

Dynamic filtering

Growth highlighting

Multilingual category display

Time-based visibility control

📁 Project Files
File Name	Description
task4_analysis.ipynb	Python data cleaning & time series analysis
task4_dashboard.pbix	Power BI dynamic dashboard
Play Store Data.csv	Dataset
🎯 Key Learning Outcomes

Advanced time series analysis

Complex filtering logic implementation

Dynamic dashboards using DAX

Data translation & localization techniques

Business-level dashboard design

🚀 Conclusion

This task demonstrates advanced Power BI dashboard engineering, Python time series analytics, and dynamic report automation, making it highly relevant for Data Analyst and BI Developer roles.
