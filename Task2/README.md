# Choropleth Map Analysis using Power BI

## Project Overview

This task visualizes global app installs using an interactive choropleth map based on app categories.

## Dataset

File used: **Play Store Data.csv**

Main columns used:

* Category
* Installs
* Country (derived using ISO country codes)

## Data Transformations

* Converted Installs to numeric format
* Removed categories starting with **A, C, G, S**
* Selected **top 5 categories** based on total installs
* Filtered categories where **installs exceed 1 million**
* Mapped countries using **ISO-3 country codes**

## Visualization

An **interactive choropleth map** was created to show:

* Global distribution of installs
* Category-wise installs
* Highlighted categories exceeding **1 million installs**

## Time Restriction Logic

The choropleth map is displayed **only between: 6 PM IST and 8 PM IST**.

Outside this time range, the visualization is hidden.

## Tools Used

* Python
* Pandas
* Plotly
* Jupyter Notebook

## Conclusion

* A few top categories dominate global installs.
* High-install categories show strong global presence.
* Time-based visibility adds dynamic dashboard control.

---
