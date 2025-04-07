---
layout: default
title: Homework 5 - Visualizations
---

## Bar Chart: Total Licenses by License Type

<iframe src="bar_chart.html" width="700" height="500"></iframe>

This bar chart visualizes the total number of licenses issued by license type in the Illinois dataset. The x-axis shows the different license types, and the y-axis shows the number of licenses. I used a vertical bar chart so that comparisons between license types would be clear and intuitive. No color was applied, as the chart focuses on raw counts rather than categorical dimensions. The data was transformed using Pandas’ `value_counts()` method on the "License Type" column to aggregate the number of entries for each type.

---

## Line Chart: Licenses Over Time (Filtered by License Type)

<iframe src="line_chart.html" width="700" height="500"></iframe>

This interactive line chart visualizes the number of licenses issued per year, filtered by license type. A dropdown allows the user to select a license type, and the chart updates accordingly. The x-axis represents the year (derived from the “Original Issue Date”), and the y-axis shows the count of licenses issued. I used Altair’s `selection_point()` and `binding_select()` to implement the dropdown filter. The interactivity improves the clarity by allowing users to isolate trends for one license type at a time. The data was grouped using Pandas `groupby()` on both year and license type.

### Interactivity

The dropdown interactivity enables viewers to focus on one license type at a time, which helps reduce clutter and reveal year-by-year trends more clearly. This makes the visualization more informative and user-friendly.

---

<p><a href="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv">The Data</a></p>
<p><a href="https://github.com/Aanchal123/Aanchal123.github.io/blob/main/hw5/YOUR_NOTEBOOK.ipynb">The Analysis</a></p>

