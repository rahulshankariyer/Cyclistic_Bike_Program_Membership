# Google Data Analytics Professional Certificate Case Study - Bike Sharing Data from Cyclistic, Chicago

## Scenario

I am a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. They have Member riders, who have an annual membership with Cyclistic and Casual riders, who buy single day or single ride passes to utilize the service. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, the team wants to understand how Casual riders and Members use Cyclistic bikes differently. From these insights, the team will design a new marketing strategy to convert casual riders into members. But first, Cyclistic executives must approve my recommendations, so they must be backed up with compelling data insights and professional data visualizations.

## Data Used

<a href = "https://divvy-tripdata.s3.amazonaws.com/index.html"> The data used is the original Bike Trip Data since its founding in 2013. </a>The data chosen for this analysis was for the calendar year 2021.

## Tools Used

1. SQL BigQuery
2. Tableau 
3. R Programming
4. Pivot Tables

## Data Transformations

1. Added a column named "ride_length" to calculate the time taken for each bike journey. 
2. Calculation of ride_length = ended_at – started_at
3. Added a column named "day_of_week" to mention which day of the week on which each trip happened
4. Calculation of day_of_week = WEEKDAY(started_at,1), ranging from 1-7
5. Generated Pivot tables to show the weekly data of average ride lengths and number of rides, for both the casual and member riders, every month and every quarter of 2021

## Analysis

The below visualizations were generated:

### 1. Casual Rider vs Member Rider - Number of Riders Each Day of the Week (Y-axis scale: 100,000 per unit)

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Portfolio/main/Cyclistic%20Bike%20Program%20Membership/Data%20Visualization%20through%20R%20and%20Tableau/Number%20of%20Rides%20by%20Member%20and%20Casual%20Riders%20each%20Day%20of%20the%20Week.png)

### 2. Casual Rider vs Member Rider - Number of Riders Each Month of the Year

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Casual%20Rider%20vs%20Member%20Rider%20-%20Number%20of%20Riders%20for%20Each%20Month%20of%20the%20Year.png)

### 3. Casual Rider vs Member Rider - Ride Duration Each Day of the Week

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Average%20Ride%20Duration%20of%20Casual%20%26%20Member%20Riders%20by%20Day%20of%20the%20Week.png)

### 4. Casual Rider vs Member Rider - Ride Duration Each Month of the Year

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Casual%20Rider%20vs%20Member%20Rider%20-%20Ride%20Duration%20for%20Each%20Month%20of%20the%20Year.png)

### 5. Casual Rider vs Member Rider - Top 6 Start & End Stations

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Portfolio/main/Cyclistic%20Bike%20Program%20Membership/Data%20Visualization%20through%20R%20and%20Tableau/Top%206%20Start%20%26%20End%20Stations%20of%20Casual%20%26%20Member%20Riders.png)

### 6. Casual & Member Riders By Bike Type

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Casual%20%26%20Member%20Riders%20by%20Bike%20Type.png)

### 7. Top 6 Most Popular Stations by Bike Type

![alt text](https://raw.githubusercontent.com/rahulshankariyer/Cyclistic_Bike_Program_Membership/main/Data%20Visualization%20through%20R%20and%20Tableau/Top%206%20Most%20Popular%20Stations%20by%20Bike%20Type.png)

## Insights

1. Casual riders on an average, ride longer than member riders.
2. The number of casual riders increased during the weekend while the number of member riders decreased during the weekend.
3. The top 6 stations for the member riders are clearly in downtown Chicago while the top 6 stations for the casual riders are closer to the tourist/leisure spots.
4. The first three findings together indicate that members are generally commuters, while casual riders generally ride for leisure.
5. Number of riders reached its peak during the summer, especially July and August, and tapered off during winter for both member and casual riders. 
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
