---
name: Vega Lite Multiple Ways Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Ways to get vega-lite plots in our webpages.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example Vega-lite Specs Multiple Ways to Includes

<vegachart schema-url="{{ site.baseurl }}/assets/json/visfromvegaeditor.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/interactivefromvegaeditor.json" style="width: 100%"></vegachart>


## Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

