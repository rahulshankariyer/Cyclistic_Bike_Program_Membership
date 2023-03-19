# Bike Sharing Data Analysis for Cyclistic, Chicago

-<i>Google Data Analytics Professional Certificate Case Study</i>

## Scenario

I am a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. They have Member riders, who have an annual membership with Cyclistic and Casual riders, who buy single-day or single-ride passes to utilize the service. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, the team wants to understand how Casual riders and Members use Cyclistic bikes differently. From these insights, the team will design a new marketing strategy to convert Casual riders into Members. But first, Cyclistic executives must approve my recommendations, so they must be backed up with compelling data insights and professional data visualizations.

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

1. On average, Member riders ride 14 minutes and Casual riders ride 26 minutes, which is nearly twice as long as Member riders.
2. The number of Casual rides went up by 74.45% during the weekend while the number of Member rides dropped by 10.58% during the weekend.
3. The top 6 stations for the Member riders are clearly in downtown Chicago while the top 6 stations for the Casual riders are closer to the tourist/leisure spots.
4. The first three findings together indicate that Members are generally commuters, while Casual riders generally ride for leisure.
5. Number of rides peaked during the summer, June to September, and was the least during the winter, December to March, for both Members and Casual riders. Member rides went up 3.5 times while Casual rides went up 9.1 times in the summer months.
6. There is no data regarding the age of Members for 2021. From the data of the previous year (2019), there is a negligible number of members below the age of 16 (0.02% among the total riders that year).
7. In 13% of the rides, the riders neglected to return the bike to any station. Among the riders who did not return the bikes, there was an almost even split between Member and Casual riders, with slightly more Member riders - 50.6% for Member riders & 49.4% Casual riders.

## Recommendations (Data Based)

1. Introduce 3 new types of membership:

    (i) Weekend membership (Saturdays & Sundays)
    
    (ii) Summer membership (May-October)
    
    (iii) Weekend-Summer hybrid membership (Saturdays & Sundays and all of July & August)
2. Approach the Corporations and local businesses to enroll their employees and offer group discounts, thus increasing membership.
3. Initiate a program to attract riders 16 years and below.
4. Based on frequency, make sure all stations are stocked with appropriate numbers and types of bikes.

## Recommendations (General, not necessarily Data Based)

1. Have a business tie-up with a bank to finance annual memberships.
2. Develop an App for only members with:
    - bike availability information at each station
    - bike reservations valid for 30 mins. 
    - other membership information such as expiry date, number of rides, ride duration, etc. 
   
   This will enhance membership privileges and may induce some Casual riders to become Members.
