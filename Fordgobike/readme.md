#  Ford Gobike Data Exploration
## by Mohammad Hanafy

## Dataset

> This document explores a dataset containing the trip data of the ford gobike approximately 183,412 with 16 features (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude ,end_station_longitude, bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip). Most variables are 9 numerical, and others are 2 datetime, 4 object type and 1 is boolean type.

> To clean the datasee the following is done: 1- change the data type for start and end time to be datetime64. 2- change the data type for bike_share_for_all_trip to be bool. 3- All the null values were dropped.

> Further steps were made: 1- "start_hour", "end_hour" columns were added by extracting the hour from the datetime format. 2- "distance_meter" column was added by calculating the distance using the lat,long coordinates of the start and end stations. 3- "member_age_ column was added by subtracting the member birth year from the year of the dataset collection (2019).


## Summary of Findings

> Trip Duration is highly dependent on the age of the member, when the age between 20 to 50, the trip duration is higher than the older ages, also the duration has a high relation with distance, finally, we can observe that the Customer category go in longer trips than the subscribers..
> For the age, duration, and user type, both Customer and Subscriber are showing similar trends for age and trip duration, but for subscribers the trip duration is higher for older age.
> The gender didn't seem to affect the duration of the trips that much.


## Key Insights for Presentation

> Trip Durations in the dataset take on a very large range of values. Number of Trips values first increases starting from around 1400 values to 12500 values at peak around 350 seconds but then starts to fall below at 2000 values.
