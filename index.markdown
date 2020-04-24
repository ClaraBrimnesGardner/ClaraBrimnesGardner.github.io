---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Car Crashes in New York School Districts"
---
In 2019 227 people were killed in traffic accidents in New York City, and more than 50.000 people were injured. On this webpage we will visualize the geographical patterns of accidents in New York City. More specifically we will investigate which school districts, that are the most dangerous. The data used for the visualizations on this page, is found on <https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95>

The figure below shows a map of New York City, where each school district has been colored according to the number of traffic accidents. The different tabs allow you to base the coloring on incidents, injuries and fatalities per square kilometer.
{% include CloroplethIncidents.html %}
Both in terms of incidents, injuries and fatalities, school district 2 is by far the most dangerous district. The safest districts are located in the west of Brooklyn (district 16 and 32). When switching to injury percentage the pciture changes a lot. School district 2 is now the safest district, while districts in West Brooklyn and Queens are more dangerous. The most dangerous district in terms of injury rate is district 18 in Brooklyn, where 40 % of crashes results in an injury. The plot indicates that most accidents happens in the most urban areas (Manhattan), but the seriousness of the accidents rise as we enter the residential areas of New York.

Below the temporal patterns are investigated. The plot below shows the distribution of the accidents across the 24 hours of the day. The legend allows you to add the distribution for one or more district to the plot. Notice that all the distributions have been normalized, such that the total height of the bars is 1.
{% include DistrictBarsTabs.html %}
The distribution of the accidents is very similar for the different districts. There are most accidents at day-time with peaks at 8-9 o'clock and 16-17 o'clock - typical rush hour.
