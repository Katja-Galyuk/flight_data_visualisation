# Carrier on-time performance for the state of New York, 2018
## by Yasir Gani


## Dataset

> My dataset was on the on-time carrier performance for domestic flights in the state of New York (NY), USA, in 2018. It was a recommended dataset as part of the Udacity project, but I obtained the data from the following source: https://www.transtats.bts.gov/Fields.asp.

> The data I downloaded contained the following columns: 'month', 'day_of_month', 'day_of_week', 'fl_date', 'op_unique_carrier', 'origin', 'dest', 'dep_time', 'dep_delay', 'dep_del15', 'taxi_out', 'taxi_in', 'arr_time', 'arr_delay', 'arr_del15', 'cancelled', 'diverted', 'actual_elapsed_time', 'air_time', 'distance', 'carrier_delay', 'weather_delay', 'nas_delay', 'security_delay', 'late_aircraft_delay', 'dep_period', 'arr_period'.



## Summary of Findings

> Data was explored by finding the fundamental insights, such as the most active airlines, most active airports and busiest time of day. I then went on to explore how factors such as the time of year influence the departure delays and taxi times to the runway of flights. I found there was little correlation in my numerical data, therefore I looked for patterns in the categorical data to give insights on the departure delays and taxi times. I found a pattern between weather delays and departure delays throughout the year, as well as how each airline is affected by specific types of other delays. I then combined the categorical variables to give more detailed insights on how airport and airline can play a part in departure delays and taxi times. Add to that the effect of the time of day on the taxi times and departure times and it was important to note the categorical variables in the dataset provided the most potential for insights into the outcomes of my investigation.

> However it should still be noted that, given the data my investigation can only shed light to a certain extent. Other factors in a complex operation of air travel may also play a significant part in departure delays and taxi times, so more data would be needed to give more confident insights.


> My key findings were as follows:
- 724,850 flights analysed, filtered for domestic flights that were not cancelled
- Most taxi out times to the runway were around 25 minutes long, although the range of times was high
- LGA was the airport with the most domestic air traffic in 2018 in NY
- The numerical data (such as departure delays and taxi out time) did not show any strong correlation in the dataset, only airtime and distance, departure delay and arrival delay showed strong correlation
- The larger airports of LGA and JFK saw the highest numbers of delays of specific delay type (weather, late aircraft, security, NAS, carrier). The months of July and August also showed highest number of delays
- This translated to longer departure delays for during July an August, which correlated with the pattern of the number of weather delays encountered, with Delta and JetBlue most affected
- Taxi times had a slightly higher mean during these months too, with Endeavour the top airline for longest taxi time
- Mean taxi times were highest across the two main airports of LGA and JFK, with the highest mean of each airport from the six most active airlines as 29.9 mins (JFK) and 30.8 mins (LGA)
- The pattern of departure delays gradually increased through the day, with morning seeing shorter delays, afternoon seeing slightly longer delays, but evenings showing greater delays. Night flights, of which there were few, saw longest mean departure delays at JFK
- Taxi times were more consistent through the day, but JFK saw a spike in the evening

> I chose to follow up with the categorical variables of airport, airline, time of day and time of year to present in my explanatory data analysis as these fields gave most insight into the pattern of departure delays and taxi times.

## Key Insights for Presentation

> The key insights were:
- Flight delays increasing with weather
- JetBlue seeing longest mean departure delays
- JFK and LGA displaying longest taxi times to the runway on departure, with JFK's times increasing during the evening period

## Resources used

> https://matplotlib.org/tutorials/colors/colormaps.html for color palettes
> https://www.bts.gov/topics/airlines-and-airports/understanding-reporting-causes-flight-delays-and-cancellations for definitions of delay type
> https://stackoverflow.com/questions/54495376/rename-ticks-from-y-axis-in-seaborn-barplot to rename ticks on x and y axis
https://stackoverflow.com/questions/33179122/seaborn-countplot-with-frequencies for help positioning frequency values in frequency plots