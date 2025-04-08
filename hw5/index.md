---
layout: default
title: Homework 5 - Visualizations
---

## Bar Chart: Total Licenses by License Type

<iframe src="bar_chart.html" width="600" height="600"></iframe>

This bar chart visualizes the total number of licenses issued by license type in the Illinois dataset. I used a vertical bar chart to support easy comparison between categories. I encoded the "License Type" column on the x-axis as a nominal (categorical) variable, and the aggregated count on the y-axis as a quantitative value. I did not use color encoding, as the goal was to focus solely on quantity rather than additional dimensions. The data was transformed using Pandas’ `value_counts()` method on the "License Type" column to calculate totals.

---

## Line Chart: Licenses Over Time (Filtered by License Type)

<iframe src="line_chart.html" width="900" height="500"></iframe>

This interactive line chart visualizes the number of licenses issued per year, filtered by license type. I used a line chart to show trends over time. The "Year" was encoded on the x-axis as an ordinal value, and the count of licenses was encoded on the y-axis as a quantitative variable. I also applied color encoding to the "License Type" to distinguish values, but since the dropdown filter limits it to one type at a time, only one line appears based on selection. To prepare the data, I first converted the "Original Issue Date" column to datetime format, extracted the year, and then used Pandas `groupby()` to aggregate counts by year and license type.

---

### Interactivity

For interactivity, I used Altair’s `selection_point()` along with a `binding_select()` dropdown. This allows the viewer to choose a license type from the dropdown menu, dynamically filtering the chart. This interaction simplifies the visualization and makes it easier to analyze trends for individual license types without the clutter of overlapping lines.

---

### Overlap

The dataset used for this homework is new to me and has not been used in any previous homework or lab assignments.

---

<p><a href="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv">The Data</a></p>
<p><a href="https://github.com/Aanchal123/Aanchal123.github.io/blob/main/hw5/Workbook.ipynb">The Analysis</a></p>
