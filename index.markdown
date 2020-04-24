---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Car Crashes in New York School Districts"
---
In 2019 227 people were killed in traffic accidents in New York City, and more than 50.000 people were injured. On this webpage we will visualize the geographical patterns of accidents in New York City. More specifically we will investigate which school districts, that are the most dangerous. The data used for the visualizations on this page, is found on <https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95>

The figure below shows a map of New York City, where each school district has been colored according to the number of traffic accidents. The different tabs allow you to base the coloring on incidents, injuries, fatalities and the injury rate (injuries divided by incidents).
{% include CloroplethIncidentTabs.html %}
Both in terms of incidents, injuries and fatalities, school district 2 is by far the most dangerous district. The safest districts are located in the west of Brooklyn (district 16 and 32). When switching to injury percentage the pciture changes a lot. School district 2 is now the safest district, while districts in West Brooklyn and Queens are more dangerous. The most dangerous district in terms of injury rate is district 18 in Brooklyn, where 40 % of crashes results in an injury.

Below the temporal patterns are investigated. The plot below shows the distribution of the accidents across the 24 hours of the day. The legend allows you to add one or more districts
{% include DistrictBars.html %}
