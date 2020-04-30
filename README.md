# Traffic Accident Analysis - USA 2016-2019
### Author - Akanksha Shetty
I'm from India which has the second-largest population in the world. Mumbai specifically is known to be the city that never sleeps. Coming to the States was a huge difference for me especially because of how less crowded this place was. Back in Mumbai, I used to live in a locality called Andheri, which has one of the busiest streets. Traffic accidents were a normal thing, in fact, sometimes it gets so bad that the cops have to step in and make the public follow them overriding the traffic signals. I don't think I have experienced anything like this here especially because of this place being not-so-crowded or at least the city I live in here. However, this made me curious about the number of traffic accidents occurring across all states in the United States of America. 


For this project, I plan on analyzing the traffic accidents occurring in the USA and the factors influencing it.

The primary dataset I chose for my project can be found here 
[here](https://www.kaggle.com/sobhanmoosavi/us-accidents)
    
and this is the data for traffic accidents in the USA for the years 2016-2019. 
   

The secondary data set I chose to take can be found here https://www.census.gov/newsroom/press-releases/2019/popest-nation.html, this consists of charts of top 10 populated states in the year 2019 and percentage growth. From this dataset I wanted to obtain the actual population of the states in 2019. The dataset values can also be verified with Wikipedia as they are accurate.

![](/Plots/Plot1.png)

California has the darkest shade indicating that the number of <b>traffic accidents in California is the most</b>. But let's dig deeper.
Since most of the medium to light shades are similar due to their values, a bar chart can give us more insights.

![Plot 2](/Plots/Plot 2.png)

Looking at the bar chart and the geo-map above, it is clear that California has the most number of cases. However, Let's compare it with the population to understand if overall it's normal for California to have high cases or it's just due to its population.
<br>
<b>I decided to compare the top 5 states having the most number of cases.</b><br>

Note:- Different factors can be taken into account like the total number of driver licences issued per state to the number of cases in that state however I decided to take population into account. While the population is not the best factor it can give us an overall insight on the same. I plan on analyzing drivers license in my future analysis.
<br>

![Plot 3](/Plots/Plot 3.png)


Surprisingly comparing the population we get to know that <b>South Carolina has many cases compared to its population</b>. Meaning that of the population is taken as a factor then the percentage of South Carolina being affected is way more than the other states. This makes us realize that <b>only taking the number of cases into account will not give the best interpretation. </b>The Map on the right tells us that the highest cases are occurring on the east coast, which is extremely interesting.


Not all accidents are severe right? <br>There is a level of Severity associated with each accident, let's explore this. Below there is an interactive plot which has a drop-down menu to select the latitude and longitude of the accidents. <br>
Heres an activity for you all:<b><br>
Step 1: adjust x to starting latitude and y to Starting longitude.<br>
Step 2: adjust x to Ending latitude and y to Ending longitude. 
</b><br>
What do you see?

![Plot 4a](/Plots/Plot 4a.png)

![Plot 4b](/Plots/Plot 4b.png)
It can be clearly seen that when we adjust the drop-down menu to the starting locations, most of the points on the map turn blue, orange and grey. These are between mid to high level of severity.

But when we adjust the drop-down to the ending locations, most points on the map turn green.

This implies that the <b>starting locations of the accidents so far have a higher level of severity.</b>
Exploring more on the severity, lets see which states are top 5 states for each level of severities.


![](/Plots/Plot 5.png)

It's not surprising that most of the states are the same throughout, but it was fascinating to see that Severity 4 has Florida with the most number of cases. This indicates that even though California has the most number of traffic accident cases, not all of them are from severity 4.
 
Another interesting thing is that Texas is not in the top 5 states with severity level 4. 

Quiet the opposite is Georgia since it's in the top states with severity level 3 and 4 but not 1 and 2. This indicates that most of Georgias cases are dangerous. Even Ohio for that case is one of the top states with severity level 4.

<h4>Does temperature have any effect on traffic accidents? </h4>

The below graph can be arranged into a 6-month span, 1 year and throughout the years span to get a better understanding. Hovering on the data points gives more details.
Just by looking at the graph and adjusting the parameters, are there any observations? Let's find out!

![](/Plots/Plot 6.png)

Most of the data point seen lie between <b>60 to 85</b>. Most of the low temperatures are from the month of January each year which makes sense since a lot of states experience heavy snowfall during the month of January. And the months June and July have high temperatures because of summer. But extreme high and low temperatures have scare points and most of the data points are between 60 to 85.

Another interesting observation is that the point gets denser over the years. In 2016 there are less scare points compared to 2019. Does this mean that the number of cases increases over time? Let's find out
![](/Plots/Plot 7.png)

We can see that the <b>cases with level 2 severity are way higher than the other levels. </b><br>
Followed by severity 3.<br>
Severity 1 has the least number of cases. <br>
In the left plot, we can see an <b>increase in the number of cases with the increase in the number of weeks</b>, this is an interesting observation, this can be confirmed with the plot on the right. This shows that in the <b>start of the year there are fewer cases</b>, The number of cases in the months October, November and December are higher, this could possibly be because towards the end of the year, its the time for holidays and people tend to travel a lot in those months. However, it is surprising to see that the <b>month of October has the most number of cases </b>compared to November and December.

Let's assess the other factors like<b> Traffic signal, stop sign, turning loop and amenity. </b>
The dataset provides the values for each of the independent accidents.

The below graph describes all these factors.

![](/Plots/Plot 8.png)

<b>Traffic Signal :</b>

Most of the values are false and there are very few True values for each of the accidents.
The leading severity level is severity level 2 however it is biased due to most cases being at severity level 2.

<b>Stop sign:</b>

Almost all accidents did not have a stop sign. This means that the stop sign is not a huge factor affecting accidents.

<b>Turning Loop: </b>

This value too is indicative of the fact that turning loops do not affect the traffic accidents since all of them did not have a turning loop.

<b>Amenity:</b>

This isn't a very good sign since the heavy false value indicates that there were no amenities near the traffic accidents. Having amenities could really help the people affected by the accidents especially if they fall into the higher level severity bracket.

It is clear from the graph below that <b>Visibility is not one of the factors influencing traffic accidents</b>, As we can see that most accidents had the highest visibility(10). Whereas lower visibility values have lesser accidents. 

![](/Plots/Plot 9.png)


<h4>References:</h4>
<br>
The data from this dataset were fetched from the below sources, while there was no need to plot a bar chart for it, I decided to do it anyway since we are working with visualizations.

![](/Plots/Plot 10.png)



Other than this,
The data sets are available to us because of the following sources 
<br>
License of the dataset - Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)
<br>
We can only use this data for non-commercial, research, or academic applications by citing the papers as follows:
<ul>
<li><h5>Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. “A Countrywide Traffic Accident Dataset.”, 2019.</h5></li>

<li><h5>Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, Radu Teodorescu, and Rajiv Ramnath. "Accident Risk Prediction based on Heterogeneous Sparse Data: New Dataset and Insights." In proceedings of the 27th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, ACM, 2019.</h5></li>

</ul>
The following datasets were also explored :

https://www.census.gov/data/tables/time-series/demo/popest/2010s-state-total.html <br>

https://worldpopulationreview.com/states/<br>

https://www.census.gov/newsroom/press-releases/2019/popest-nation.html<br>

https://en.wikipedia.org/wiki/List_of_states_and_territories_of_the_United_States_by_population<br>


