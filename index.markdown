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


## Exploring the Temporal Patterns of the Districts
It is of interest to explore the temporal patterns of traffic accidents in New York in order to identify any trends, both in a broad timeframe and regarding time of day etc. Firstly the entire dataset is considered, for all districts and all times. In the graph below, the number of accidents is plotted against time. The data is furthermore smoothed with a rolling mean in order to give an indication of the overall trend of the data. The purple box below the plot allows you to choose a specific time interval to zoom in on.
{% include TimeSeries.html %}
The number of accidents seems to be fairly stable with around 500 accidents each day. Some days have an exceptionally high number of accidents. For instance there was 1512 accidents of the 5'th of March in 2015 and 1687 accidents of the 3'rd of February in 2014. Considering only longer lasting trends, there is a dive in accidents in April 2016 and in March 2020. The dive in March 2020 can probably be explained by less traffic due to covid-19, but there is no obvious explanation for the pattern in April 2016.


We now zoom in on the different districts and the temporal patterns they exhibit and how they deviate from the overall distribution. For each district the distribution of the accidents across time is displayed (the figure allows you to toggle between an _hourly_, _weekly_, _monthly_ and _yearly_ timeframe).
By clicking on a district the accident distribution for that district will be added to the plot. This allows for comparison with the overall distribution, making exploration of how each district behaves easy.
Notice that all the distributions have been normalized, such that the total height of the bars is 1.

{% include ClickTabMap.html %}

The _daily_ distributions of the accidents are quite similar for the different districts. There are most accidents at day-time with peaks at 8-9 o'clock and 16-17 o'clock - typical rush hour. Some districts deviate a little. In the districts in Manhattan there are more accidents at night time than expected (especially in the small district 2). This is probably due to the urbanity of the area. Also in Staten Island there are more accidents at night, than expected. There are not obvious deviations from the total pattern in the other districts. Moving to the _weekly_ patterns, fewest accidents are happening in the weekend, and most are happening on Fridays. The distribution over the the rest of the week-days is almost even, with a slight dive on Mondays. Again the small district in Manhattan (district 2) deviates from the general pattern, as much more accidents happen in the weekend. This is probably due to people from the outer districts going into the city. Most of the other districts follows the general pattern. In district 14 and 15 in Brooklyn (just across from district 2), fewer accidents are happening in the weekend, but the deviation is not as big as for district 2. The _monthly_ pattern shows that few accidents are happening in April. A possible explanation for this can be the Spring Break, which takes place in April. Surprisingly it does not seem like more accidents are happening in the winter - something one could have expected due to bad weather conditions. At last the _yearly_ distribution shows that there in general was a slight rise in the accidents from 2013 to 2018. In 2019 the number of accidents dropped. Notice that 2020 has been left out of this plot. Some districts shows very different patterns. In district 1 and 2 in Manhattan the number of accidents was highest in 2013 and has decreased since. On the other hand Staten Island (district 31) saw no decrease in 2019. Many of the districts in the Bronx (e.g 7, 8, 9, 11) have more accidents in 2017-2019 than the general pattern.


## Exploring Schools in Focus Districts
One thing is how many accidents that happens in a school district, another thing is where they happen. In the following we will investigate which schools in each district that are the most dangerous. We have selected 5 focus districts with different characteristica - namely district 1, 5, 18, 21 and 26. The figure below highlights the locations.

{%include FocusDistricts.html %}

Below individual maps of the five focus-districts are shown. The black dots shows the locations of the schools, and the opaque circles are colored according to the number of accidents happening within a 250 meter radius of the school. Notice that only accidents happening in the same school district as the schools has been counted. 5000 accidents have been randomly sampled from each district. The red dots shows these.
{% include DistTabsSample.html %}
District 1 is a small school district located in Manhattan. The schools are close to each other, and in general many accidents happen close to the schools. There is a tendency that the westernmost schools have most accidents nearby.

District 5 is located in the north of Manhattan. Here it seems that the westernmost schools are the safest, while the schools in the south east of the district have many accidents nearby. The number of accidents close to the schools are again high - the safest school have more than 1500 accidents within the radius of 250 meters.

District 18 is the district with highest injury-rate. It is located in the south west of Brooklyn. The district is larger than district 1 and 5, and therefore the circles appear smaller. The most dangerous schools are found in the north-east of the district. It is worth noting the difference between the two northernmost schools, PS 219 Kennedy King and PS 268 Emma Lazarus. PS 219 Kennedy King have a much higher number of accidents that PS 268 Emma even though they are located very close to each other. This is maybe due to a dangerous road near PS 219 Kennedy - looking at the plot there seems to be a street with many accidents south east of PS 219 Kennedy.

District 21 is located in the south of Brooklyn. Looking at the scale on the color-bar it is seen that in general fewer accidents happens nearby the schools in this district. The most accidents happens in the east of the district, while the safest schools are found in the south west.

At last district 26 is found in East Queens. The school district is large an fairly few accidents happen close to the schools. The most dangerous schools are found in the middle of the district. Looking at the plot is seems like there are some dangerous, vertical roads.

Comparing the locations of the district and the distributions it seems like the most dangerous parts of all districts, are the one faced towards the city, while closer to the water is more safe. This is especially seen in district 1, 18 and 21.

## Predicting the Probability of Accidents
At last we seek to predict the number of accidents happening close to schools. We restrict ourselves to the between 8-10 AM and between 2-4 PM, which are classical drop-off and pick-up times. Furthermore we base our predictions on the weather, as we investigate the probability of an accident happening with and without rain.


The predictions are based on a generalized linear model with the Poisson-distribution as probabilistic model.
