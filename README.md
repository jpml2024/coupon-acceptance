## Assignment 5.1: Will the Customer Accept the Coupon?

**Background**

A customer driving through town and a coupon is delivered to their cell phone.There are five different types of coupons:
* Carry out & Take away
* Coffee House
* Bar
* Less expensive resturants (under \$20)
* More expensive resturants (\$20 - $50)

*Will they accept the coupon?*

**Goal**

The goal is to analyze the data to understand the differences between customers who did and did not accept the coupons. 

**Approach**

Data Science lifecycle approach is applied
* Ask a question
* Obtain the data
* Understand the data
* Clean and prepare the data
* Understand the data/world
* Make a recommendation

**Data**

This data was collected via a survey on Amazon Mechanical Turk and are coming from the UCI Machine Learning repository.

The atributes are detailed here : [Data Attributes](https://github.com/jpml2024/coupon-acceptance/blob/main/coupon_acceptance.ipynb)  

Data file at : [data](https://github.com/jpml2024/coupon-acceptance/tree/main/data)


**Data preperation**

(1) Total data size in 12684  

(2) There are 74 duplicate rows that has been removed  

(3) Car column has 99% missing data. Dropped this column from analysis  

(4) Rest of the missing data are less than 1% and has been dropped  

(5) Converted 'age' column to integer and replaced "below21" to 20  and "50plus" to 51  


| Column | Missing data count |
|---|---|
| car| 12576|
| Bar | 107 |
| CoffeeHouse |	217 |
|CarryAway| 151 |
|RestaurantLessThan20 |130 |
|Restaurant20To50 |189|


**Data Analysis and conclusion**  

_**High acceptance rate**_  

(1) Total Coupon acceptance rate is 56.8%. 

(2) Out of all 5 different kind of Coupons, follwing two has the higest  acceptace rate:  
  * "Carry out & Take away" has top acceptance rate of 73.57% 
  * "Restaurant(<20)" is the 2nd top with 70.97%

(3) Drivers of age group 21 to 35 are having higher acceptance rate in these two categories of coupons

(4) Roughly 60% of the drivers who accpetd cheaper resturants coupons eats at a restaurant with average expense less than \$20 atlest once a month.

(5) Roughly 60% of drives who accepted carryAway coupons buys takeaway food at least once a month.

(6) The acceptance rate for carry away coupons are higher when driving in the morning (7 AM to 10 AM) or in the late night 10 PM or so.

(7) They accept cheaper resturant coupons mostly when driving during lunch or dinner time of 2 PM or 6 PM

(8) Coupons having expiration of 1 day has higher acceptance rate

(9) Cheaper resturant coupons has higher acceptance rate if lesser distance to drive but it has no bearing on carry away coupons.

(10) Drivers who accepts most are either unemployed or student or earning less than $50K and has no urgent destination to go. Gender has no bearing on acceptance rate.

_**Low acceptance rate**_

(1) 43.2 % of the distributed coupons are not accpted

(2) The coupon with expiration of 2hr has low acceptance

(3) 'Bar' coupons are least aceepted

(4) Drivers with income more than $100K has least acceptance

(5) Driver  going to work are less likely to accecpt coupon

(6) Females accecpts less than males

