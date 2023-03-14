# Bike Sharing Data Analysis for Cyclistic, Chicago

-<i>Google Data Analytics Professional Certificate Case Study</i>

## Scenario

I am a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. They have Member riders, who have an annual membership with Cyclistic and Casual riders, who buy single day or single ride passes to utilize the service. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, the team wants to understand how Casual riders and Members use Cyclistic bikes differently. From these insights, the team will design a new marketing strategy to convert Casual riders into Members. But first, Cyclistic executives must approve my recommendations, so they must be backed up with compelling data insights and professional data visualizations.

## Data Used

<a href = "https://divvy-tripdata.s3.amazonaws.com/index.html"> The data used is the original Bike Trip Data since its founding in 2013. </a>The data chosen for this analysis was for the calendar year 2021.

## Tools Used

1. SQL using BigQuery
2. Tableau 

## Data Transformations

1. Added a column named "ride_length" to calculate the time taken for each bike journey. 
2. Calculation of ride_length = ended_at – started_at
3. Added a column named "day_of_week" to mention which day of the week on which each trip happened
4. Calculation of day_of_week = WEEKDAY(started_at,1), ranging from 1-7
5. Generated Pivot tables to show the weekly data of average ride lengths and number of rides, for both the casual and member riders, every month and every quarter of 2021

## Analysis

The below visualizations were generated:

### 1. Rides and Average Ride Duration <i>(by Day of the Week & Month)</i>

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Rides%20and%20Average%20Ride%20Duration.png)

### 2. Most Popular Bike Stations

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Most%20Popular%20Bike%20Stations.png)

## Insights

1. Casual riders on an average, ride twice as long as member riders.
2. The number of casual riders nearly doubled during the weekend while the number of member riders dropped by roughly 10-20% during the weekend.
3. The top 6 stations for the member riders are clearly in downtown Chicago while the top 6 stations for the casual riders are closer to the tourist/leisure spots.
4. The first three findings together indicate that members are generally commuters, while casual riders generally ride for leisure.
5. The ratio of the monthly average number of member riders during the summer (June-August) and winter (December-February) was 4:1 while the same ratio for casual riders was 15:1
6. There is no data regarding the age of Members for 2021. From the data of a previous year (2019), there is a negligible number of members below the age of 16.
7. There is no significant difference between the preferences of member and casual riders in the bike type category.
8. In 13% of the rides, the riders neglected to return the bike to any station.

## Recommendations (Data Based)

1. Introduce 3 new types of membership:

    (i) Weekend membership (Saturdays & Sundays)
    
    (ii) Summer membership (May-October)
    
    (iii) Weekend-Summer hybrid membership (Saturdays & Sundays and all of July & August)
2. Approach the Corporations and local businesses to enroll their employees and offer group discounts, thus increasing membership.
3. Initiate a program to attract riders 16 years and below
4. Based on frequency, make sure all stations are stocked with appropriate numbers and type of bikes.

## Recommendations (General, not necessarily Data Based)

1. Have a business tie-up with a bank to finance annual memberships
2. Develop an App for only members with 
    - bike availability information at each station
    - bike reservation valid for 30 mins. 
    - other membership information such as expiry date, number of rides, ride duration, etc. 
   
   This will enhance membership privileges, attracting the casual rider to become a member
