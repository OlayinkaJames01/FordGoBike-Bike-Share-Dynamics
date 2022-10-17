# FordGoBike-Usage-Trend-Data-Analytics-Project

## Dataset

GoBike is a regional public bike sharing system in the San Francisco Bay Area, California. The dataset used for this exploratory analysis consists of monthly individual trip data from February, 2019 in CSV format covering the greater San Francisco Bay area.

##### Data wrangling process:
-  Convert `start_time` and `end_time` to datetime format
-  Convert `start_station_id`, `end_station_id` and `bike_id` to "string" dtype 
-  Covert `user_type` and `member_gender` to "category" dtype 
-  Creation of new columns for `duration_minutes`, `trip start date` in yyyy-mm-dd format, `trip start hour` of the day, `day of week` and `month`

- Dropping rows with null values
-  Creation of new column calculating `age_of_rider` from `member_birth_year`
-  Convert `member_birth_year` and `age_of_rider` to integer instead of float type for visualization purposes

## Summary of Findings

The distribution of daytime trips peaks between 7am and 9am and 4pm and 7pm during normal rush hours. The bulk of rides occurred on work days (Monday through Friday) and the primary usage is likely for commuting. This is evident from the trip distribution over day of the week plot.
There were more male than female users, and the majority of members were subscribers as opposed to occasional users. The majority of members did not utilise bike sharing for all of their journeys, and the majority were between the ages of 25 and 40.
The majority of trips were rapid and brief, lasting between 5 and 15 minutes, while there were exceptions as long as 24 hours.

There are much more subscribers than customers. The riding patterns of subscribers and customers vary significantly. Subscribers use the bike sharing system to commute to work, so the majority of trips occurred on weekdays (Mon-Fri) and especially during rush hours (when going to work in the morning and leaving in the afternoon), whereas customers typically ride for recreation on weekends in the late afternoon or early evening. The drop in usage on weekends for subscribers suggests that they primarily use their bikes for commuting to and from work during the week, whereas the little increase in usage on weekends for consumers suggests that they primarily use their bikes for leisure/touring and relaxing purposes.

The multivariate investigation reinforced some of the patterns observed in the previous bivariate and univariate explorations; the relationship between the various variables plotted are visualized collectively, and the information is presented in a unified manner. The efficient/short time of usage for subscribers corresponds to their high concentration during rush hours Monday through Friday, showing that the consumption is mostly for commuting to and from work. The more relaxed and flexible usage pattern of customers indicates that they are using the bike-sharing system considerably differently than subscribers, primarily on weekends and in the afternoons, likely for city tours or recreational purposes.


## Key Insights for Presentation

Exploration reveals that the two types of riders have distinct usage patterns/habits. The system is highly utilized by subscribers on weekdays, i.e., Monday through Friday, while customers ride frequently on weekends, particularly in the afternoon. Many subscribers' travels are concentrated between 7:00 am and 7:00 pm and 4:00 p.m. and 7:00 p.m. on weekdays, however customers tend to utilize the service more in the late afternoon around 5:00 p.m. The efficient/short time of usage for subscribers corresponds to their high concentration during rush hours Monday through Friday, showing that the consumption is mostly for commuting to and from work. The more relaxed and flexible usage pattern of customers indicates that they are using the bike-sharing system considerably differently than subscribers, primarily on weekends and in the afternoons, likely for city tours or recreational purposes.
