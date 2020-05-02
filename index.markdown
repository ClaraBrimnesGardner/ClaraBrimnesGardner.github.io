---
layout: home
title:  
---
<h1> Car Crashes in New York School Districts </h1>
 ___Created by Clara Brimnes Gardner (s153542), Sara Nielsen (s153173)___  
 ___and Jon Roslyng Larsen (s154358)___


In 2019 233 people were killed in traffic accidents in New York City, and 56,469 people were injured. Similar numbers apply for the last few years. On this webpage we will visualize the geographical patterns of accidents in New York City. More specifically we will investigate which school districts and schools, that are the most dangerous. The data used for the visualizations on this page, can be found [here](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95).

The figure below shows a map of New York City, where each school district has been colored according to the number of traffic accidents. The different tabs allow you to base the coloring on incidents, injuries and fatalities divided by area. The plot includes accidents from January 2012 to March 2020.
{% include CloroplethIncidents.html %}

Most accidents occur in Manhattan and West Brooklyn and the further away from Manhattan the fewer accidents.
Injuries also occurs most frequently in Manhattan, but there is a larger area with many occurrences - the rate is for instance high in most of Brooklyn. The fatalities follows a pattern similar to the injuries. Comparing the accidents with the injuries and fatalities suggest that the accidents happening outside Manhattan is more serious. This is investigated below, where a new map of New York City is shown. Here the school districts are colored according to the injury rate and the fatality rate - that is the number of injuries and fatalities divided by the number of accidents.

{% include CloroplethRates.html %}

There are some districts in Brooklyn and the Bronx with a high number of injuries compared too the number of accidents. Especially district 18 in Brooklyn is worth noticing. Here we find both the highest injury and fatality rate among the districts. By further inspection, the plot seems to indicate that the seriousness of accidents increases the further from Manhattan we go. This trend most likely stems from the speed of which the cars moving; in Manhattan the density of traffic will not as frequently allow for unsafe speeds.
The map indeed shows that the injury rates are lowest in Manhattan, and are higher in the less urban school zones.


## Exploring the temporal patterns of the districts
It is of interest to explore the temporal patterns of traffic accidents in New York in order to identify any trends, both in a broad timeframe and regarding time of day etc.
Firstly the entire dataset is considered, for all districts and all times. In the graph below, the number of accidents is plotted against time. The data is furthermore smoothed with a rolling mean in order to give an indication of the overall trend of the data.
{% include TimeSeries.html %}

We now zoom in on the different districts and the temporal patterns they exhibit and how they deviate from the overall distribution. For each district the distribution of the accidents across time is displayed (the figure allows you to toggle between an _hourly_, _weekly_, _monthly_ and _yearly_ timeframe).
By clicking on a district the accident distribution for that district will be added to the plot. This allows for comparison with the overall distribution, making exploration of how each district behaves easy.
Notice that all the distributions have been normalized, such that the total height of the bars is 1.

{% include ClickTabMap.html %}

The daily distributions of the accidents are quite similar for the different districts. There are most accidents at day-time with peaks at 8-9 o'clock and 16-17 o'clock - typical rush hour. Some districts deviate a little. For instance district 2 in Manhattan has more accidents at night time than expected - probably because it is one of the most urban areas. In district a lot accidents happen at 8 AM. The weekly patterns, shows that the week-day in general does not influent the number of accidents. When considering all districts a few more accidents happens on Fridays, but otherwise it is evenly distributed. Again District 2 in Manhattan deviates from the overall distribution, as many accidents happen on Sunday and Saturday - perhaps due to non-residents visiting in the weekends. In district 20 on the other hand, the number of accidents on Saturdays is much lower than the overall distribution.

April is the month with fewest accidents. Especially April 2016 seems to be an all time low for all districts. Further research has not unveiled any extraordinary things happening at that time, so perhaps the deep valley is caused by human error in the data. The systems that registers accidents were perhaps acting up this April.

## Exploring the Schools
One thing is how many accidents that happens in a school district, another thing is where they happen. In the following we will investigate which schools in each district that are the most dangerous. Below a map of selected school districts are shown. The black dots shows the locations of the schools, and the opaque circles are colored according to the number of accidents happening within a 100 meter radius of the school.
{% include DistTabsSample.html %}
