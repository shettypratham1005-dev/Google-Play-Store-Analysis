# Grouped Bar Chart Analysis

## Project Overview
This project analyzes the Google Play Store dataset to compare average rating and total review count for the top 10 app categories by installs.

---

## Dataset
File used: Play Store Data.csv  
Main columns used:
- Category  
- Rating  
- Reviews  
- Installs  
- Size  
- Last Updated  

---

## Data Transformations
- Converted Reviews to numeric
- Cleaned Size column (removed 'M')
- Converted Last Updated to datetime
- Filtered:
  - Rating ≥ 4.0
  - Size ≥ 10M
  - Last Updated in January

---

## Visualization
A grouped bar chart was created to compare:
- Average Rating
- Total Review Count

for the top 10 filtered categories.

---

## Time Restriction Logic
The grouped bar chart is displayed only between:
3 PM IST and 5 PM IST.

Outside this time range, the graph is not shown.

---

## Tools Used
- Python
- Pandas
- Matplotlib
- Jupyter Notebook

---

 Conclusion

- Free apps dominate the Play Store.
- Certain categories like Games and Tools have the highest installs.
- Paid apps tend to have slightly higher average ratings.
- Recent updates correlate with better ratings and installs.
