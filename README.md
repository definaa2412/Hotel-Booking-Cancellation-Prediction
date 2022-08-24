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
    
### Exploratory Data Analysis
   1. From where the most guests are coming?
      ![The most guest](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/The%20most%20guest.jpg)
      Ans: Portugal
     
   2. How much do guests pay for a room per night?
      ![Reserved room](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/Reserved%20room%20type%20adr.png) ![Meal type](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/Type%20meal%20adr.png)
     
     Ans: Average price per room depending on its type and meal arrangement.
     
   3. How does the price vary per night over the year?
      ![Price vary](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/room%20per%20night.png)
   
      Ans : The number of guests in Resort Hotels reaches the highest value in summer, while the number of guests in City Hotels relatively higher than Resort Hotels.
  
   4. How long do people stay at the hotels?
      ![People long stay](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/Long%20Stay.png)
   
      Ans : For 1-5 total nights, City Hotel is preferable, while Resort Hotel is preferable for more than five nights.
   
   5. How many bookings were cancelled?
      ![Booking cancelled](https://github.com/definaa2412/Hotel-Booking-Cancellation-Prediction/blob/main/images/many%20booking%20cancelled.png)
   
      Ans : There are  37.1 % bookings were cancelled. So, this target variable is categorized into **Imbalance Data**.
     
### Data Preparation for Modelling
   1. Drop some variables to make the model more general.
   2. Get dummies for the categorical variables.
   3. Standardize the numerical variables.
   4. Handling the imbalanced dataset with SMOTE.
   5. Split the data into train and test split.
   
### Machine Learning Model

   
     
     
    








