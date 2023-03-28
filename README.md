# Latam Postulation

This repository is the solution of the **Data Scientist Challenge**. The problem is presented below.

## Problem

The problem consists in predicting the probability of delay of the flights that land or take off from the airport of Santiago de Chile (SCL).
For that you will have a dataset using public and real data where each row corresponds to a flight that landed or took off from SCL during 2017.
The following information is available for each flight:

- Fecha-I: Scheduled date and time of the flight.
- Vlo-I : Scheduled flight number.
- Ori-I : Programmed origin city code.
- Des-I : Programmed destination city code.
- Emp-I : Scheduled flight airline code.
- Fecha-O : Date and time of flight operation.
- Vlo-O : Flight operation number of the flight.
- Ori-O : Operation origin city code
- Des-O : Operation destination city code.
- Emp-O : Airline code of the operated flight.
- DIA: Day of the month of flight operation.
- MES : Number of the month of operation of the flight.
- AÑO : Year of flight operation.
- DIANOM : Day of the week of flight operation.
- TIPOVUELO : Type of flight, I =International, N =National.
- OPERA : Name of the airline that operates.
- SIGLAORI: Name city of origin.
- SIGLADES: Destination city name

## Challenge

- How is the data distributed? Did you find any noteworthy insight to share? What can you conclude about this?
- Generate the following additional columns. Please export them to a CSV file named synthetic_features.csv:
  - high_season : 1 if Date-I is between Dec-15 and Mar-3, or Jul-15 and Jul-31, or Sep-11 and Sep-30, 0 otherwise.
  - min_diff : difference in minutes between Date-O and Date-I .
  - delay_15 : 1 if min_diff > 15, 0 if not.
  - period_day : morning (between 5:00 and 11:59), afternoon (between 12:00 and 18:59) and night (between 19:00 and 4:59), based onDate-I .
  
- What is the behavior of the delay rate across destination, airline, month of the year, day of the week, season, type of flight?What variables would you expect to have the most influence in predicting delays?
- Train one or several models (using the algorithm(s) of your choice) to estimate the likelihood of a flight delay. Feel free to generate additional variables and/or supplement with external variables.
-  Evaluate model performance in the predictive task across each model that you trained. Define and justify what metrics you used to assess model performance. Pick the best trained model and evaluate the following: What variables were the most influential in the prediction task? How could you improve the Performance?
