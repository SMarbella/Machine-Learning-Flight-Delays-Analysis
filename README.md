# Machine Learning Flight Delays Analysis
I used the R programming language and machine learning techniques to analyze the data from the 2013 NYC Flights dataset. This project gives us an analysis of flight delays from different airlines and airports in New York City, and the top 10 popular destinations. The project approaches the problem of flight delays through visualizations that calculate the number of early flights and delayed flights from each airline. The last part of the project includes the development of a few machine learning modules to attempt to predict whether or not a flight is going to be delayed. The end result is that it is not easy to predict when a flight is going to be delayed, and one of the hints tell us that the month of flight affects the number of flight delays. The fall months and December have more flight delays than other months of the year.

## Synopsis
Flight delays are a very important subject for the entire aviation industry around the world because of their association with the loss of revenues. According to the Bureau of Transportation Statistics, over 20% of flights within the US were delayed in 2018, which resulted in a revenue loss of approximately 41 billion USD. These delays cause inconvenience to the airlines and passengers because increased travel time leads to increased food, crew payment, aircraft repositioning, fuel consumption, and lodging costs and added stress among passengers. Flight delays could happen due to several factors, such as air congestion, weather conditions, mechanical problems, the time it takes for all passengers to board the plane, and    an airline's inability to handle demands.
The flight dataset contains information about all flights that departed in 2013 from airports in New York City to destinations in the United States, Puerto Rico, and the American Virgin Islands. The airports included are NYC, EWR, JFK, and LGA.

## Table Columns
-	`year`: All flights departed in 2013.
- `month`: The month of departure.
- `day`: The day of departure.
- `dep_time`: Actual departure time (format HHMM or HMM) in an airport's local timezone.
- `sched_dep_time`: Scheduled departure time (format HHMM or HMM) in an airport's local timezone.
- `dep_delay`: Number of minutes delayed from expected departure time. Negative times represent early departures.
- `arr_time`: Actual arrival time (format HHMM or HMM) in an airport's local timezone.
- `sched_arr_time`: Scheduled arrival time (format HHMM or HMM) in an airport's local timezone.
- `arr_delay`: Number of minutes delayed from expected departure time. Negative times represent early arrivals.
- `carrier`: Two-letter abbreviation of the carrier/airline.
- `flight`: Flight number.
- `tailnum`: Plane tail number.
- `origin`: The airport where the plane flew.
- `dest`: The destination airport where the plane flew.
- `air_time`: Amount of time in minutes spent in the air.
- `distance`: Distance between airports in miles.
- `hour, minute`: Time of the scheduled departure broken into hours and minutes.
- `time_hour`: Scheduled date and hour of the flight.

## Retrieved table from
https://cran.r-project.org/web/packages/nycflights13/nycflights13.pdf

## Objectives
The goals of the analysis are to develop a machine learning model that predicts the duration of flight delays in various airports in New York City. The methods I used for data exploration are a linear regression model to calculate the correlation between different variables, an indicator that categorizes delayed and early flights, dodged bar plots that display the on-time flight performance between the airlines, airports, and number of flights. The main results show that no matter how many flights an airport receives and an airline delivers, there will always be a large proportion of flight delays. The main results obtained the existing relationships between the delay predictor variable and the response variables. It also displayed the number of New York City delayed flights from different airlines, the top 10 airport destinations, the month of the year, and the total number of delayed and early flights.

# Charts Generated For This Project
## Summary Table
