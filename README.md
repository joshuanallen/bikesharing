# Bikesharing Analysis for CitiBike

## Project Overview
We analyzed CitiBike bike-sharing data from August 2018 in New York City, New York to assess the possibility of launching a similar bike-sharing program in Des Moines, Iowa. 

## Resources
Data: 201908-citibike-tripdata-modified.csv
Software: Tableau Public, Jupyter Notebook, Python 3.7.6, VS Code

## Dashboard of Results
[Link to dashboard](https://public.tableau.com/app/profile/josh.allen/viz/CitiBike_Challenge_16240482526770/CitiBikeAugust2018Analysis)

## Results

### Summary
We identified the following trends about the bikes and users in the NYC CityBike bikesharing program in August 2018:
1. 2m+ rides taken for ~693k hours in NYC August 2018 
2. 81% of rides are conducted by subscribers to the program
3. Younger users (<20 years old) have the longest bike trips on average
4. Most rides are 4-7 minutes long implying use for "last-mile" travel
5. There is minimal variance in bike trip duration between genders
6. Peak usage hours are during commuting hours on weekdays (7-9 AM, M-F) and middle of the day on weekends (10 AM - 5 PM, Sat-Sun). 
7. Peak usage hours have minimal variance from overall usage between female and male, but undefined genders skew towards weekend usage.
8. Thursday has the heaviest usage amongst males and females. Male and female subscribers are more likely to use during the weekdays.
9. Subscribers use the bikesharing service during commute hours on weekdays whereas non-subscribing customers use the service more on weekends during the day.
10. Subscribers start their rides downtown as part of their commute whereas non-subscribers ("customers") start their rides at various points of interest throughout the tourist part of the city especially Central Park.

### Analysis

**1.** Program usage summary for August 2018
    - Total rides taken: **2,344,224 rides**
    - Total bikes used: **13,893 bikes**
    - Total ride time: **2,461,480,527 seconds** (693,745+ hours)

**Picture 1.1: CitiBike NYC overview for August 2018**

![Picture 1.1: CitiBike NYC overview for August 2018](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_overview.png)


**2.** There are two user types for the bikesharing program; subscribers and non-subscriber customers. **Subscribers accounted for 81% of all rides** taken in August 2018

**Picture 2.1: Bike rides by user type**

![Bike rides by user type](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_user_breakdown.png)


**3.** Picture 3.1 showsthe average trip duration for all users based on their reported birthdates. Users born between 1995-2003 have the highest average trip duration. There is a significant spike in users born after 1998 implying that **younger populations with less access to personal capital and car ownershipare more likely to use the bikesharing service**. There is a large anonmalous spike in 1969, implying users are submitting incorrect birthdates as they are not validated through any official means.

**Picture 3.1: Trip duration by user birth year**

![Trip duration by user birth year](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_trip_duration_birth_year.png)


**4.** Picture 4.1 shows the frequency of trip lengths in minute for all rides in August 2018. Most CitiBike rides are under 20 minutes in length. **A significant portion of trips last 4-7 minutes in length.** This implies the service is used for short trips meant to bridge the "last mile" of travel. 

**Picture 4.1: Frequency of per-trip ride duration (hours and minutes)**

![Frequency of per-trip ride duration (hours and minutes)](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_per_trip_duration_frequency.png)


**5.** Picture 5.1 shows per-trip travel duration data browken out by gender. The curves show **minimal variance between the gender of a user**. Males used the service at a much higher rate than the other gender options. Those without a defined gender had a significantly smaller number of rides, but were longer on average.

**Picture 5.1: Frequency of per-trip ride duration by gender (hours and minutes)**

![Frequency of per-trip ride duration by gender (hours and minutes)](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_per_trip_duration_frequency_by_gender.png)


**6.** Picture 6.1 shows a heat map of when users are starting their rides broken out by hour of the day and day of the week. **Peak usage hours of the bikesharing program occur at commute hours (7-9 AM, M-F) during the weekdays and the middle of the day on the weekends (10 AM - 5 PM, Sat-Sun)**. This implies the heaviest use of the service is largely driven by commuters on the weekdays.

**Picture 6.1: Trip start times for each hour of days of week**

![Trip start times for each hour of days of week](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_trips_by_weekday_per_hour.png)


**7.** Picture 7.1 shows a heatmap that further breaks down the information in Picture 6.1 by gender. The chart shows a **similar time of usage pattern between genders** with the highest usage times being commute hours (7-9 AM, M-F) during the weekdays and the middle of the day on the weekends (10 AM - 5 PM, Sat-Sun). Undefined users' usage pattern shows more usage on the weekends than weekdays in the 10 AM -5 PM hours.

**Picture 7.1: Trip start times for each hour of days of week by gender**

![Trip start times for each hour of days of week by gender](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_trip_by_weekday_per_hour_by_gender.png)


**8.** Picture 8.1 shows a heat map of rides broken out by gender and user type. The service is most used by male subscribers and and female subscribers. The chart shows the **heaviest usage taking place on Thursday followed by Friday, Monday and Tuesday**. The chart also matches our previous results where **usage patterns between genders is similar and the unknown users are mostly weekend users**.

**Picture 8.1: Trip start times for each hour of days of week by gender by user type**

![Trip start times for each hour of days of week by gender by user type](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_trips_by_weekday_by_gender_by_usertype.png)


### Additional Charts

**9.** Picture 9.1 shows a heat map of rides by hour and day of week split by user type. The **highest usage for subscribers is during commute hours (7-9 AM, M-F) during the weekdays**. The highest usage for non-subscribing customers is the middle of the day on the weekends (10 AM - 5 PM, Sat-Sun). This implies that subscribers are possibly using the service as part of their daily commute and non-subscriber customers use the service to get around on the weekends either tourists or causal users.

**Picture 9.1: Trip start times by day of week and time of day by user type**

![Trip start times by day of week and time of day by user type](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_trip_start_times_by_day_of_week_time_of_day_usertype.png)


**10.** Picture 10.1 shows the most popular ride start locations for subscribers to the bike sharing service. Picture 10.2 shows the most popular ride start locations for non-subscribers ("customers").

Picture 10.1 shows the most popular start locations for subscribers is in the downtown area, where commuters leave from. This implies that subscribers are more likely to use the service as part of their commute to an from work.

**Picture 10.1: Most popular trip start locations (subscribers)**

![Most popular trip start locations (subscribers)](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_most_popular_start_loc_subscribers.png)


Picture 10.2 shows the most popular start location for non-subscribers is around points of interest in the city and Central Park. This implies non-subscribing customers are more likely to be using the service for more casual travel between tourist hotspots.

**Picture 10.2: Most popular trip start locations (customers)**

![Most popular trip start locations (customers)](https://github.com/joshuanallen/bikesharing/blob/406c38ef10bd952594b27b5ef1d222873e1fe2b5/images/citibike_most_popular_start_loc_customers.png)

## Conclusion
The bike sharing program in NYC showed success with it's subscriber base as a "last mile" option for commuters. Casual users use the service to move between tourist spots on the weekend. This program would be successful in Des Moines if the working demographic is centralized in a downtown area with an need to provide "last mile" support to their commutes. Additionally, success would rely heavily on the younger male population as they were the largest userbase of the CitiBike NYC program. Also, the program should focus on marketing the program to younger tourists as an alternative means of travel from hotspot to hotspot.

### Limitations of current analysis
1. No pricing or revenue data was provided in the dataset so financial analysis cannot be conducted. Addtionally would require maintenance costs to provide analysis on profitability.

2. Age based data is skewed due to non-verified user input for birthdate of user. To better this analysis we would require more accurate and verified birthdate data.

3. Need more data about native and tourist population of Des Moines versus New York City in order to perform accurate comparison data for feasibility of program launch. 

4. Public transportation availability and locations for Des Moines can determine need


