---
name: Vega Lite Interactive Plot Homework 10 Group 17
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/cars.png
description: Homework 10 Group 17 Interactive Vega-lite Visuals
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 10 Group 17 Interactive Vega-lite Visualization

<vegachart schema-url="{{ site.baseurl }}/assets/json/vis1_dashboard_select_interact.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/vis2_dashboard_bar_interact.json" style="width: 100%"></vegachart>


## Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

