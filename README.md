# Machine Learning Flight Delays Analysis
I used the R programming language and machine learning techniques to analyze the data from the 2013 NYC Flights dataset. This project gives us an analysis of flight delays from different airlines and airports in New York City as well as the top 10 popular destinations. The project approaches the problem of flight delays through visualizations that calculate the number of early flights and delayed flights from each airline. The last part of the project includes the development of a few machine learning modules to attempt to predict whether or not a flight is going to be delayed. The end result is that it is not easy to predict when a flight is going to be delayed, and one of the hints tell us that the month of flight affects the number of flight delays. The fall months and December have more flight delays than other months of the year.

## Synopsis
Flight delays are a very important subject for the entire aviation industry around the world because of their association with the loss of revenues. According to the Bureau of Transportation Statistics, over 20% of flights within the US were delayed in 2018, which resulted in a revenue loss of approximately 41 billion USD. These delays cause inconvenience to the airlines and passengers because increased travel time leads to increased food, crew payment, aircraft repositioning, fuel consumption, and lodging costs and added stress among passengers. Flight delays could happen due to several factors, such as air congestion, weather conditions, mechanical problems, the time it takes for all passengers to board the plane, and an airline's inability to handle demands.
The flight dataset contains information about all flights that departed in 2013 from airports in New York City to destinations in the United States, Puerto Rico, and the American Virgin Islands. This analysis focuses on the following airports in New York City: Newark Liberty International Airport (EWR), John F. Kennedy International Airport (JFK), and LaGuardia Airport (LGA).

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
![Image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/blob/main/Graphs/Summary%20Table.png)
- **Figure 1.** A numerical summary of the variables in the data set.

In Figure 1, the numerical summary analyzes each variable's minimum numbers, first quartiles, medians, means, third quartiles, and maximum values. These values give a brief analysis of the differences between the variables. The Hartsfield-Jackson Atlanta International Airport received the most flights (16,837 in total) from New York City while the Charlotte Douglas International Airport received the fewest flights (13,674 in total) from New York City.

## Linear Regression Model
![Image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/blob/main/Graphs/Linear%20Regression%20Model.png)
- **Figure 2.** A numerical summary of the variables in the data set.

In Figure 2, the linear regression model gets a general idea of the relationships between each variable from the dataset. There are 16 carriers that flew to one of the three airports in New York City. Some carriers are more prone to flight delays than others. It did not matter what month of the year a flight took place to cause a delay, but there is a weak relationship between the month and delay. Planes coming from the JFK and LGA airports often face flight delays. The LGA airport has more delays than JFK because its p-value is more significant. The travel distance, scheduled departure and arrival times, actual departure and arrival times, and delays have strong relationships with delays.

## Number of Flights Per Airline
![Image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/blob/main/Graphs/Flights%20Per%20Airline.png)
- **Figure 3.** The on-time flight performance key indicator shows the number of early flights and delayed flights in each airline.

In Figure 3, most carriers have more early flights than delayed flights. They still have a large proportion of delayed flights. It shows that it is difficult for airline carriers to depart and arrive at airports on time. Alaska Airlines Inc, Hawaiian Airlines Inc, and Mesa Airlines Inc have an approximately even number of delayed flights and early flights. Only the Frontier Airlines Inc and AirTran Airways Corporation carriers had more delayed flights than early flights in 2013. SkyWest Airlines did not have any flights in 2013, meaning that it ceased operations before 2013.

## Number of Delayed Flights and Early Flights in New York City
![Image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/blob/main/Graphs/Number%20of%20Delayed%20Flights%20and%20Early%20Flights%20in%20New%20York%20City.png)
- **Figure 4.** This bar plot shows that there are more early flights in total than delayed flights in New York City.

In Figure 4, out of the total number of flights to New York City in 2013, there were more early flights than delayed flights. Due to a large proportion of delayed flights, the graph indicates that it is quite difficult to maintain a positive on-time flight performance.

## Number of Delayed Flights and Early Flights Per Month 2013
![Image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/blob/main/Graphs/Number%20of%20Delayed%20Flights%20and%20Early%20Flights%20Per%20Month%202013.png)
- **Figure 5.** This bar plot shows that the winter months have more flight delays than the summer months.

In Figure 5, the proportion of delayed and early flights varied throughout the year. The summer months of June and July have almost equal numbers of early and delayed flights. The fall months of September, October, and November mostly had early flights. September had the fewest number of delayed flights while December had the most delayed flights. The month of December is the only month that had more delayed flights than early flights due to the Christmas holiday season and heavier air traffic levels. The average month in 2013 had approximately 27,300 flights in New York City. February 2013 had the fewest flights approximately 23,600. August 2013 had the most flights approximately 28,800.

## Number of Delayed Flights and Early Flights to Top 10 Destinations from New York City
![Image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/blob/main/Graphs/Number%20of%20Delayed%20Flights%20and%20Early%20Flights%20to%20Top%2010%20Destinations%20from%20New%20York%20City.png)
- **Figure 6.** This bar plot shows the proportion of delayed flights and early flights in the top 10 destinations from New York City.

In Figure 6, this figure shows the flights traveling from New York City to the top 10 popular destinations in 2013. The Hartsfield Jackson Atlanta International Airport had the most flights from New York City, but it had a large proportion of delayed flights. Some airports, such as the Hartsfield Jackson Atlanta International Airport and Miami International Airport have a large proportion of delayed flights that takes up almost half of their total flights. The Ronald Reagan Washington National Airport had a low proportion of delayed flights compared to the other airports.

## Machine Learning Model Results
Based on the data used to create the graphs above, I split the data into two sets: training and testing data. 70% of the original data went to the training data while the rest went to the testing data. I developed a logistic machine-learning model that trained on the training data to make predictions that were supposed to be similar to the testing data. The calculations for the correct predictions are based on whether or not the column value and row value match diagonally.

![image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/assets/92709384/9fc39404-a0c0-491d-8d26-996566f78b27)

The logistic machine learning model is ineffective in predicting uncertainties that cause flight delays. There was a total of 98,062 flights in New York City in 2013. When a flight is early, the model predicts the flight correctly 971/(972 + 1,241) = 43.88% of the time. When a flight is delayed, the model predicts the flight correctly 39,344/(56,505 + 39,344) = 41.05% of the time. The error rate is (56,505 + 1,241)/98,062 = 58.89%.

95% confidence intervals between the delay and the distance, origin, and carrier.

![image](https://github.com/SMarbella/Machine-Learning-Flight-Delays-Analysis/assets/92709384/ec7fbe1c-3283-471f-b00d-6db693383a30)

The fit variable indicates that the predicted variable is about 36.45. The range between the lower and upper bound is approximately the same as my colleague's lower and upper bound. It is the range where the model thinks most of the observations would fit in 95% of the time. The difference is that my predicted variable is higher by about 14 units.

## Conclusions
In conclusion, my logistic machine learning model is ineffective in predicting uncertainties that cause flight delays due to high error rates from uncertainties. My model is 58.89% wrong due to the variety between the variables. Each month in 2013 had uncertainties between the flights from New York to their destinations. The proportion of delayed and early flights varied throughout the year. The summer months of June and July have almost equal numbers of early and delayed flights. The fall months of September, October, and November mostly had early flights. September had the fewest number of delayed flights while December had the most delayed flights. December is the only month with more delayed flights than early flights due to the Christmas holiday season and heavier air traffic levels. The range between the lower and upper bound is approximately the same as my collaborator's lower and upper bound. The difference is that my predicted variable is higher by about 14 units.

I approached the issue of flight delays using a logistic machine learning model. I created a delay indicator in a separate variable that indicates whether or not a flight is delayed by adding the arrival and departure delay times together. I explored the data visually to understand the possible underlying causes of flight delays. The flight indicator color-coded the flights in the graphs, where red represents delayed flights while green represents early flights. Different airlines and airports have different flight delays. Seasons are a possible factor for causing flight delays due to higher air traffic in the fall months and December. I also created summary calculations to find the variables that had significant p-values with the delay indicator.

The performance of my approach is extensively detailed and gives me plenty of insight into flight delays. When I divided the data into training and testing samples, I used the entire data set to create a logistic machine learning model and a linear machine learning model. I used the logistic model to create a confusion matrix to consider the trade-offs associated with the overall model error and prediction error for the delay predictor and the distance, origin, and carrier response variables. Since the error rate is high, it is ineffective in avoiding or predicting uncertainties.

The error rate could have been improved if the flight dataset had more table columns and variables that had strong correlations with each other. In this dataset, the correlations are either very weak or non-existent, which is why my logistic machine learning model has high error rates in predicting the causes of flight delays. The logistic machine learning model will only work if the dataset has information about the other factors that cause flight delays, such as weather conditions, airline glitches, airplane maintenance issues, and air traffic levels.
