# Flight price prediction

* The dataset contains the date of the flight, the operating airline, ticket class, flight duration, fare, etc for domestic flights in india.
* The airline Indigo operates 28519 flights in the time period of the dataset and is the one with the most flights.
* StarAir on the other hand only operates 62 flights.
<img src="https://github.com/janS95/flight_price_prediction/blob/main/images/amount_of_flights_per_airline.png">

* The most frequent route is from Delhi to Mumbai with 8649 flights.
<img src="https://github.com/janS95/flight_price_prediction/blob/main/images/amount_of_flights_per_route.png">

* Every flight is operated with an economy class while only 4 flights have a first class. Even the business class or permium economy is not very common for the domestic flights.
<img src="https://github.com/janS95/flight_price_prediction/blob/main/images/amount_of_flights_per_class.png">

* The price of the ticket is rising with fewer days left till the journey but nevertheless, there are still some days were you can make a bargain.
<img src="https://github.com/janS95/flight_price_prediction/blob/main/images/fare_dependent_from_days_left.png">

* The fare for the business class tickets is highest (when ignoring the 4 first class flights) but there are still some business class tickets for the price of economy class.
<img src="https://github.com/janS95/flight_price_prediction/blob/main/images/fare_distribution_per_class.png">

* Processed the data (scaled, encoded categorical data, drop columns/rows) and trained 4 models. The RandomForestRegressor has the lowest Mean Absolute Error and highest R2-Score

## Results:
| Model | MAE | MSE | R2-Score |
| --- | --- | --- | --- |
| KNeighborsRegressor | 3257 | 3.32e+07 | 0.92 |
| LinearRegression | 12387 | 2.26e+08 | 0.45 |
| **RandomForestRegressor** | 1768 | 1.38e+07 | 0.97 |
| GradientBoostingRegressor | 3951 | 4.12e+07 | 0.90 |
