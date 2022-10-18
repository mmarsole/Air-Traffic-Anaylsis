# Air-Traffic-Anaylsis
Contained within this repository are the code, results, and general summaries of two different projects (one trying to predict flight Trajectory and the other an explorartory Analysis of flight data). Both Projects used data from 'Open Sky Network'
## General Summary

During the course of my studies within the MGIS program at the U of MN, I studied and assessed flight data from Open Sky Network. Here you can access archival flight information and current flight data. Each plane is outfitted with a transponder that transmits it current coordinates, velocity, heading, and other relevant flight information for Air Traffic Controlers. Utilizing this data I first performed general exploratory analysis such as the frequency 
of flights within U.S. Class B airspaces, average flight speed at varying altitudes, the length and frequency of flights within the continental U.S., and an assessment  of flights' behavior near or around strong weather. Secondly, I predict a plane’s location in space over time (lat., lon.) relying on Automatic Dependent Surveillance – Broadcast (ADS-B) data and the implementation of a Long-Short-Term-Model (LSTM). 

All results from the exploratory anaylsis was for flight within the conteneal U.S. on May 25th of 2020 from 12:00:10 am to 5:59:50 am GMT (May 24th of 2020 from 07:00:10 pm to 12:59:50 am CDT). While Results and training of the LSTM relied on data over Chicago's airport on  May 25th of 2020 from 12:00:10 AM and 12:59:50 AM (recorded in GMT time). 

## File Index:
### ExploratoryAnalysis:

### PredictingFlightTrajectory:
  #### Data
  ##### a198e5.csv: 
  Data for 1 flight path during <__insert time___>. Used for intial LSTM training (where intial 90% of its flight points were used to train and the last 10% of its flight points to test). 
  ##### adsb_Chicago_flights.csv: 
  All flights that were recorded during <__insert time___> and intersected with Chicago Class B airspace (essentially identifying fights around Chicago O'Hare International Airport). ???Used to train an LSTM???
  ##### flight_89902f.csv: 
  Data for 1 flight path during <__insert time___>. Used for intial LSTM training (where intial 90% of its flight points were used to train and the last 10% of its flight points to test).
  ##### flight_89902f_dif.csv: 
  Data for 1 flight path during <__insert time___>. Additional column attributes were created, that recorded the differnce between varying timestamps. Used for linear regression model. 
  
  #### Models-Results
  ##### allflights.pt
  ##### flight0.pt
  ##### lstm1_1.pt
  ##### lstm1_3inputs_2outputs.pt
  ##### lstm1_3inputs_3outputs_a198e5.pt
  ##### lstm2_3inputs_2outputs_89902f.pt
  * the question is: do i remember which model was train on what and resulted in which images....???
  
  #### Notebooks:
  ##### ETL_flight data.ipynb:
  ##### LSTM_a198e5_flight.ipynb: 
  ##### LSTM_allChicagoFlights_12-20.ipynb:
  ##### Mreg_flighta198e5.ipynb: 
  

## Resources:
[Open Sky Network](https://opensky-network.org/)

[LSTM for time series prediction](https://towardsdatascience.com/lstm-for-time-series-prediction-de8aeb26f2ca)

### Citations: 
