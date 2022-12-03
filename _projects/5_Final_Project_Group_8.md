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

##### Dataset Source and Additional Resources

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

For the contextual dataset we selected the New York City schools Progress Reports for the year 2010-2011. This dataset classifies each school from A to F and collected data on the school's learning environment, student performance, and progress. The data have indicators of students and how well the schools are doing for parents' and teachers' understanding. It can be compared to other similar schools. We decided to ignore the year of columns and compare schools around New York city with schools around Chicago because this dataset was collected around a similar timefram as the Chicago dataset, it represents achievements from 2010 to 2011. Although not all columns match the Chicago dataset, we designated this dataset as a "contextual dataset" because it classified schools by grade and expressed annual achievement as scores which is in the similar context as our Chicago Public schools dataset.

We created the below dashboard for our contextual dataset and we observe that there is a correlation between performance and overall score.

<vegachart schema-url="{{ site.baseurl }}/assets/json/final_proj_contex_dash_v1.json" style="width: 100%"></vegachart>

The overall score for a school is the weighted average of school environment, student performance and student progress plus additional credit earned.

Environment score reflect measuring pre-conditions for learning, student attendance and other aspects, such as high expectations, engagement, safety, respect and communication in school.

Performance score is the measure of student performance, which varies based on school type. The letter grades are based on a set grade distribution based on their percentile ranking and denote the average student's performance.

Hence the correlation visible in the graphs makes sense, as school environment and performance score are indeed some of the factors that affect the overall score of the school.

The dashboard is interactive. In the rect map, the darker color indicates higher count of records. Selecting a part from the rect map automatically displays the corresponding histogram for the overall score, thus from the charts one can get a sense of the overall score that occurs most frequently for a selected data subset.

##### NYC Schools Dataset Pie Chart

<img src="/assets/pngs/NY_school_level_pie_v1.png" alt="">

The above visualization is a pie chart that depicts the number of schools for each school level for our NYC dataset. Each school level is represented by a different color, whose legend is given on the right side of the pie chart. From the chart, it seems that most of the schools in our dataset were elementary schools, followed by high schools.
This pie chart was created from the tools provided on the cit of new york data website referenced below. 

#### Reference links for contextual dataset

2010 - 2011 School Progress Report from NYC 
https://data.cityofnewyork.us/Education/2010-2011-School-Progress-Report/upwt-zvh3



#### Starboard Notebook Final Project Part 3.1
We have our complete visualization work in Starboard which can be accessed using link [Final Project Part 3.1 Starboard Notebook](https://starboard.gg/nb/nWxM3xB)


### Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://starboard.gg/nb/nWxM3xB" text="The Analysis" %}
</div>

