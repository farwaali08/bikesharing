# bikesharing :bike:

## OVERVIEW

This analysis of bike-sharing data was prepared for investors looking to begin a similar program in Des Moines, Iowa. It features CitiBike data from New York City in August 2019, and aims to address the following:

* **When the service is utilized**
  * What are the peak times?
  * How does ridership vary throughout the week?
* **How regionality impacts ridership**
  * How does ridership vary amongst different city types? 
* **User demographics**
  * Who is using this service? 

Data was obtained from CitiBike (see under Tools and Resources) and transformed using Python/Pandas. Tableau Public was used to create the graphics.

## TOOLS & RESOURCES

### DATA

* File: `201908-citibike-tripdata.csv.zip` ([Link](https://s3.amazonaws.com/tripdata/index.html))
* [Code](https://github.com/farwaali08/bikesharing/blob/d7dbf88019605ec60ef3d388e9fb81b2c7fda98f/NYC_CitiBike_Challenge_starter_code.ipynb)

### SOFTWARE

* Python/Pandas
* Jupyter Notebook
* Tableau Public

## RESULTS & ANALYSIS

A Tableau story can be accessed by clicking [here](https://public.tableau.com/shared/C6G9H6C48?:display_count=n&:origin=viz_share_link), and can be utilized for an interactive experience.


### DATA HIGHLIGHTS

![alt_text](https://github.com/farwaali08/bikesharing/blob/7854d5e434f317b0b48bcd5f82acbe96852be588/Images/HIGHLIGHTS.png)

The highlights from this analysis include an impressive ridership number and dedicated subscriber base. Over `2.3 million` rides were recorded in August 2019, which is typically the most profitable month. Over `81%` of all users are subscribers, which indicates that CitiBike services are utilized often enough to warrant a subscription, and are in-demand.

Also included in the highlights is the peak hour data for the month. Ridership remains fairly steady from 7 AM to 9 PM, with peaks during the morning and evening rush hours (8AM-10AM and 4PM-8PM, respectively). Regarding the off-peak hours between 2AM and 5AM, this provides a window to conduct bike repairs and other maintenance activities.


### TRIPS BY WEEKDAY PER HOUR

![alt_text](https://github.com/farwaali08/bikesharing/blob/ece047f91dc26cd2846b2d1c2404a34d99a4c783/Images/2.png)

The heatmap for Trips by Weekday Per Hour further demonstrates that the on-peak times established in the previous map correspond with commuter rush hours, as most activity is observed on weekdays during these times. There is consistent usage of this service on weekends as well, with the peak times between 10 AM and 12 PM. Interestingly, the usage during Wednesday's evening rush-hour is lower than the other weekdays, and it may be worthwhile to explore to increase ridership on this day.

### USER CHECKOUT TIMES

![alt_text](https://github.com/farwaali08/bikesharing/blob/ece047f91dc26cd2846b2d1c2404a34d99a4c783/Images/7.png)

The User Checkout Times graphic displays the number of trips by duration, and indicates that the vast majority of rides are under 20 minutes in length, with a peak at around 10 minutes. The number of rides drops dramatically around the 30-minute mark, which is likely due to the [surcharge](https://help.citibikenyc.com/hc/en-us/articles/360032024912-How-long-can-I-keep-a-bike-out-) that is applied after 30 minutes of usage (and of course, the mechanics of riding a bike for that duration).

### STARTING & ENDING LOCATIONS

![alt_text](https://github.com/farwaali08/bikesharing/blob/ece047f91dc26cd2846b2d1c2404a34d99a4c783/Images/3.png)

The above map displays the starting and ending locations. The size and intensity of the markers correspond to the relative number of trips that started or ended at those locations. The data indicates that usage is higher in dense, Metropolitan areas, especially popular tourist areas, such as Manhattan. Bike usage is comparatively lower in the surrounding boroughs, which are generally suburban areas.

### GENDER ANALYSIS

![alt_text](https://github.com/farwaali08/bikesharing/blob/ece047f91dc26cd2846b2d1c2404a34d99a4c783/Images/4.png)

Both graphics above indicate that the overall customer base is largely male-identifying, with over `65%`, of roughly two-thirds of all users identifying as males. The subscriber base is predominantly male as well.

Subscribers tend to utilize the service more on weekdays, with Thursday being the busiest day, whereas non-subscribing users tend to use the service more on the weekends. As mentioned in the "Trips by Weekday Per Hour" map, the busiest times correspond with commuter rush hours, so perhaps the subscriber base utilizes the service as a means to commute to work. The non-subscribing users are more likely to be tourists, especially on weekends.

![alt_text](https://github.com/farwaali08/bikesharing/blob/ece047f91dc26cd2846b2d1c2404a34d99a4c783/Images/5.png)

The figure above is essentially an intersection between gender and the "Trips by Weekday Per Hour" map. Male-identifying users dominate this graph, which makes sense, as they are the largest group of customers.

![alt_text](https://github.com/farwaali08/bikesharing/blob/ece047f91dc26cd2846b2d1c2404a34d99a4c783/Images/6.png)

This figure is an intersection between gender the User Checkout Times. Interestingly, while the male category is larger in magnitude, both male and female groups follow a similar trend, and have the same peak at around 10 minutes. The Unknown category also has a slight peak at around 10 minutes, but overall follows a different usage pattern.

## SUMMARY & NEXT STEPS

It is apparent from the data that this bike-sharing program is successful, given the high volume of users, and loyal subscribers. However, the data is taken from one of the world's largest metropolitan cities during the busiest month--for this reason, further analysis will be required to determine how this will translate over to Des Moines. The following are questions and considerations that should be addressed:

 * A similar analysis of bike-sharing data during an off-peak month to determine the "highs" and "lows"
 * An analysis of yearly data to identify seasonal trends, if any
 * How the weather impacts these programs
 * How infrastructure impacts these programs
   * Example: the presence or absence of dedicate bike routes/bike lanes 
 * The tourism industry in New York is far more [robust](https://www.osc.state.ny.us/reports/osdc/tourism-industry-new-york-city) than it is in Iowa. It would be worthwhile to determine the percentage of users that are tourists, to see how tourism affects these programs.

Additionally, the data analyzed was taken from a pre-COVID period, and it would be interesting to examine how COVID has impacted bike sharing, especially in smaller cities and suburban areas. Some [studies](https://www.sciencedirect.com/science/article/pii/S2590198221000609) indicate that generally, ridership has increased throughout the pandemic, which they suggest is due to an increasing weariness of public transportation systems. [Others](https://www.samschwartz.com/staff-reflections/2020/10/7/shifting-gears-citi-bike-demographics-change-with-ridership-increases) mention that the pandemic has caused a sharp increase in female ridership as well. Regardless of the type of change, COVID has altered the way these programs work, so an analysis of more recent data is warranted.
