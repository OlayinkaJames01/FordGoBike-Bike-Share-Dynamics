# FordGoBike Usage Trend Data Analytics Project

## Dataset  
GoBike is a regional public bike-sharing system serving the San Francisco Bay Area, California. This project explores monthly individual trip data from February 2019, provided in CSV format, covering the greater San Francisco Bay area.

---

## Data Wrangling Process  
- Converted `start_time` and `end_time` to datetime format.  
- Changed `start_station_id`, `end_station_id`, and `bike_id` to string data type.  
- Converted `user_type` and `member_gender` to categorical data type.  
- Created new columns:  
  - `duration_minutes`  
  - `trip_start_date` (yyyy-mm-dd format)  
  - `trip_start_hour` (hour of the day)  
  - `day_of_week`  
  - `month`  
- Dropped rows containing null values.  
- Created a new column `age_of_rider` calculated from `member_birth_year`.  
- Converted `member_birth_year` and `age_of_rider` from float to integer for better visualization.

---

## Summary of Findings  

- **Trip Timing & Usage Patterns:**  
  Trips peak during weekday rush hours: 7 AM–9 AM and 4 PM–7 PM. Most rides occur Monday through Friday, indicating the primary use is commuting.  
- **User Demographics:**  
  More male users than female. Most users are subscribers rather than occasional customers.  
- **Age Distribution:**  
  Majority of riders are between 25 and 40 years old.  
- **Trip Duration:**  
  Most trips last between 5 and 15 minutes, although some extend up to 24 hours.

- **Subscribers vs. Customers Usage:**  
  - **Subscribers:** Predominantly weekday commuters with peak trips during rush hours. Usage drops significantly on weekends.  
  - **Customers:** Mainly use the system for recreation on weekends, especially in late afternoons or early evenings.

- **Multivariate Analysis:**  
  Visualizations confirm subscribers’ short, efficient trips during rush hours Monday to Friday. Customers show a relaxed and flexible riding pattern, favoring weekends and leisure rides.

---

## Key Insights for Presentation  

- The two rider types (subscribers and customers) exhibit distinct behavior patterns.  
- Subscribers heavily utilize the system on weekdays for commuting, concentrated between 7 AM–9 AM and 4 PM–7 PM.  
- Customers primarily use the system for recreational purposes on weekends, especially in the late afternoon around 5 PM.  
- The short, efficient trip durations for subscribers align with commuting needs.  
- Customers’ flexible, longer trips reflect leisure and city tours.  

These insights highlight how usage varies by user type and day, informing targeted service improvements and marketing strategies.
