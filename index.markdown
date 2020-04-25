---
layout: home
title:  
---
<h1> Car Crashes in New York School Districts </h1>

In 2019 227 people were killed in traffic accidents in New York City, and more than 50.000 people were injured. On this webpage we will visualize the geographical patterns of accidents in New York City. More specifically we will investigate which school districts, that are the most dangerous. The data used for the visualizations on this page, can be found [here](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95).

The figure below shows a map of New York City, where each school district has been colored according to the number of traffic accidents. The different tabs allow you to base the coloring on incidents, injuries and fatalities per square kilometer. The plot includes accidents from January 2012 to March 2020.
{% include CloroplethIncidents.html %}
Most accidents happens in Manhattan and East Brooklyn, and the further away from Manhattan the fewer accidents. The same pattern is seen when considering only accidents where someone was injured (Injuries tab) or died (Fatalities tab). There are however some districts in Brooklyn and the Bronx with a high number of injuries compared too the number of accidents. Especially district 23 in Brooklyn is worth to notice. District 21 in Brooklyn has a high number of fatalities. Investigating the plot seems to indicate, that the seriousness of accidents increases the further from Manhattan it happens.

Below a new map of New York City is shown. Here the school districts are colored according to the injury rate and the fatality rate - that is the number of injuries (fatalities) divided by the number of accidents.
{% include CloroplethRates.html %}
The map indeed shows that the injury rates are lowest in Manhattan, and are higher in the less urban school zones.


Below the temporal patterns are investigated. The plot below shows the distribution of the accidents across the 24 hours of the day. The legend allows you to add the distribution for one or more district to the plot. Notice that all the distributions have been normalized, such that the total height of the bars is 1.
{% include DistrictbarsTabs.html %}

The distribution of the accidents is very similar for the different districts. There are most accidents at day-time with peaks at 8-9 o'clock and 16-17 o'clock - typical rush hour.

## Explore the temporal patterns of the districts
{% include ClickTabMap.html %}
