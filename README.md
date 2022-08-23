# Project - Hotel Booking Cancellation Prediction
Defina Ambarwati : [Github](https://github.com/definaa2412)
***

## Problem Statement
  The hospitality industry is one of the most profitable businesses and a major sector in the tourism industry. However, often potential visitors cancel hotel reservations which can result in various losses.
1. The hotel cannot estimate the occupancy rate for their revenue management.
2. The hotel will suffer losses (vacant hotel rooms due to cancellations).

## Goals
1. Find out the characteristic of customers who cancelled booking by doing an exploratory data analysis.
2. Building the best classification model to predict cancellation.
3. Find out which factors have a high influence on booking cancellation.

## Dataset
  The dataset used is from Kaggle dataset [Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) with the data details as follows.
| Feature Name                    | Description                                                           |   
| -----------------------------   |:---------------------------------------------------------------------:|
| Hotel                           | Hotel (H1 = Resort Hotel or H2 = City Hotel)                          |
| is_canceled                     | Value indicating if the booking was canceled (1) or not (0)           |
| lead_time                       | Number of days that elapsed between the entering date of the booking into the PMS and the arrival date |
| arrival_date_year               | Year of arrival date |


## Summary
### Data Preprocessing
1. Data Cleaning
    * Handling Missing Values
      * Drop **company** column because it's containing 94,3% missing data.
      * Imputing **agent** column with 0 (without an agent).
      * Imputing **country** column with its mode because it has categorical data type.
      * Imputing **children** column with 0 (customer doesn't have any children).
    * Handling Double Meaning Category and Unimportant Data
      * Change Undefined to SC (They have the same meaning, *No Meal*)
      * Drop rows with 0 adults, 0 children and 0 babies.
    * Feature Engineering
    
2. Exploratory Data Analysis
   * From where the most guests are coming?
     ![The most guest](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/The%20most%20guest.jpg)
     Ans: Portugal
     
   * How much do guests pay for a room per night?
     
     Ans: Average price per room depending on its type and meal arrangement.
     
     
    








