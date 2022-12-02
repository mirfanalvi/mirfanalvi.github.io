---
name: Final Project Group 8
tools: [Python, HTML, vega-lite, Starboard]
image: assets/pngs/cars.png
description: Final Project Part 3.1 Group 8 Chicago Schools Analysis
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


##### Final Project Part 3.1: Chicago Public School data analysis using Interactive Vega-lite Visualization
###### Group 8 Members: Vaibhavi Mehta (vm19), Youngbeen Oh (yo8), Suhas Chitiki (schiti3), Muhammad Irfan Alvi (mialvi2)

## Environment and Teacher impact on College Enrollments for Chicago Public Schools


##### Dataset Description

The name of our chosen dataset is Chicago Public Schools - Progress Report Cards (2011-2012).

We obtained this dataset from the Chicago Data Portal site and this data has been compiled by the Chicago Public Schools which are under https://www.cps.edu site.
This dataset is a compilation of all Chicago Public schools report cards data for the school year 2011-2012.
This dataset has some very interesting facts about Chicago Public schools and their ratings which provide some good insight. This dataset can provide different classification options which has the potential for good visualization.

We analyzed Teacher and Environment ICON (ratings) in this dataset and see how much the ratings have an impact on students College Enrollments.


##### Dataset Characteristics

Dataset is 356KB in size. Dataset has 79 columns and 566 rows. This dataset is below the limits for Github upload.

If there is a missing or null value in the columns for specific rows it is represented by 'NDA' which shows No Data Available for the field.

##### Dataset URLs

URL: https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t

Additional Resources: https://data.cityofchicago.org/, https://www.cps.edu

CSV URL: https://data.cityofchicago.org/resource/9xs2-f89t.csv


#### Dashboard
The below dashboard visualization is a heatmap that shows how the college enrollement rate of a school depends on how supportive the school environment is for the student (environment icon) and the teachers ratings (teachers icon)

Environment Icon defines the Supportive Environment category, taken from from 5 Essentials survey, whose scores range from 1-99) Teachers Icon is based on how collaborative the teachers in that school are, taken from from 5 Essentials survey, whose scores range from 1-99.

Excluding NDA values, which indicate the values were not disclosed for those universities, the heatmap portrays that for most schools, there has been a weak correlation between the graduation rate % (% of students who have graduated within five years) and the quality of school environment and teachers.

<vegachart schema-url="{{ site.baseurl }}/assets/json/final_proj_dash_v1.json" style="width: 100%"></vegachart>


#### College Enrollment by Zip Code
The below bar plot is a histogram displaying the total number of students enrolled in colleges distrbuted by specific zip codes.

<vegachart schema-url="{{ site.baseurl }}/assets/json/final_proj_college_enroll_zip_v1.json" style="width: 100%"></vegachart>


### Contextual Dataset - 2010 - 2011 School Progress Reports from NYC

In the contextual dataset we selected the Progress Report classified each school from A to F and collected data on the school's learning environment, student performance, and progress. These data are indicators of students and how well the schools are doing for parents' and teachers' understanding. It can be compared to other similar schools. We decided to ignore the year of columns and compare schools around New York with schools around Chicago because this dataset was collected around a similar time as the Chicago dataset, even though it represents achievements from 2010 to 2011. Although not all columns match the Chicago dataset, we designated this dataset as a "contextual dataset" because it classified schools by grade and expressed annual achievement as scores.

We created the below dashboard for our contextual dataset and we observe that there is a correlation between performance and overall score.

<vegachart schema-url="{{ site.baseurl }}/assets/json/final_proj_contex_dash_v1.json" style="width: 100%"></vegachart>


##### NYC Schools Dataset Pie Chart

<img src="/assets/pngs/NY_school_level_pie_v1.png" alt="">

#### Reference links for contextual dataset

2010 - 2011 School Progress Report from NYC 
https://data.cityofnewyork.us/Education/2010-2011-School-Progress-Report/upwt-zvh3



#### Starboard Notebook Final Project Part 3.1
We have our complete visualization work in Starboard which can be accessed using link [Final Project Part 3.1 Starboard Notebook](https://starboard.gg/nb/ndZeScg)


### Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://starboard.gg/nb/nWxM3xB" text="The Analysis" %}
</div>

