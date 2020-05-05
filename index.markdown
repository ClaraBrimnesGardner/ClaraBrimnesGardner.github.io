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
It is of interest to explore the temporal patterns of traffic accidents in New York in order to identify any trends, both in a broad timeframe and regarding time of day etc. Firstly the entire dataset is considered, for all districts and all times. In the graph below, the number of accidents is plotted against time. The data is furthermore smoothed with a rolling mean in order to give an indication of the overall trend of the data. The purple box below the plot allows you to choose a specific time interval to zoom in on.
{% include TimeSeries.html %}
The number of accidents seems to be fairly stable with around 500 accidents each day. Some days have an exceptionally high number of accidents. For instance there was 1512 accidents of the 5'th of March in 2015 and 1687 accidents of the 3'rd of February in 2014. Considering only longer lasting trends, there is a dive in accidents in April 2016 and in March 2020. The dive in March 2020 can probably be explained by less traffic due to covid-19, but there is no obvious explanation for the pattern in April 2016.


We now zoom in on the different districts and the temporal patterns they exhibit and how they deviate from the overall distribution. For each district the distribution of the accidents across time is displayed (the figure allows you to toggle between an _hourly_, _weekly_, _monthly_ and _yearly_ timeframe).
By clicking on a district the accident distribution for that district will be added to the plot. This allows for comparison with the overall distribution, making exploration of how each district behaves easy.
Notice that all the distributions have been normalized, such that the total height of the bars is 1.

{% include ClickTabMap.html %}

The _daily_ distributions of the accidents are quite similar for the different districts. There are most accidents at day-time with peaks at 8-9 o'clock and 16-17 o'clock - typical rush hour. Some districts deviate a little. In the districts in Manhattan there are more accidents at night time than expected (especially in the small district 2). This is probably due to the urbanity of the area. Also in Staten Island there are more accidents at night, than expected. There are not obvious deviations from the total pattern in the other districts. Moving to the _weekly_ patterns, fewest accidents are happening in the weekend, and most are happening on Fridays. The distribution over the the rest of the week-days is almost even, with a slight dive on Mondays. Again the small district in Manhattan (district 2) deviates from the general pattern, as much more accidents happen in the weekend. This is probably due to people from the outer districts going into the city. Most of the other districts follows the general pattern. In district 14 and 15 in Brooklyn (just across from district 2), fewer accidents are happening in the weekend, but the deviation is not as big as for district 2. The _monthly_ pattern shows that few accidents are happening in April. A possible explanation for this can be the Spring Break, which takes place in April. Surprisingly it does not seem like more accidents are happening in the winter - something one could have expected due to bad weather conditions. At last the _yearly_ distribution shows that there in general was a slight rise in the accidents from 2013 to 2018. In 2019 the number of accidents dropped. Notice that 2020 has been left out of this plot. Some districts shows very different patterns. In district 1 and 2 in Manhattan the number of accidents was highest in 2013 and has decreased since. On the other hand Staten Island (district 31) saw no decrease in 2019. Many of the districts in the Bronx (e.g 7, 8, 9, 11) have more accidents in 2017-2019 than the general pattern.


## Exploring the Schools
One thing is how many accidents that happens in a school district, another thing is where they happen. In the following we will investigate which schools in each district that are the most dangerous. Below a map of selected school districts are shown. The black dots shows the locations of the schools, and the opaque circles are colored according to the number of accidents happening within a 250 meter radius of the school. Notice that only accidents happening in the same school district as the schools has been counted. 5000 accidents have been randomly sampled from each district. The red dots shows these. 
{% include DistTabsSample.html %}
In district 1 it is seen that
