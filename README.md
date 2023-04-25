# coupon02
 This project is included a jupyter notebook named prompt2.jpynp. The jupyter notebook imported the data from data\coupon.csv. The data set is coming from the UCI machine learning respository and was collected via a survey on Amazon Mechanical Turk.
 
 The data set contained 26 columns, the details explaination per each column can be found from jupyter notebook. Among these columns, the following columns contains empty  cells or Nan. The numbers of null values on a particular column can be found on the second column as listed.
 
 car                     12576
 Bar                       107
 CoffeeHouse               217
 CarryAway                 151
 RestaurantLessThan20      130
 Restaurant20To50          189
 
 To clean the data, I simply assign the values to these null values except for column car, I assigned other to these cells. The other stands for different model of the cars.
 car -> other
 Bar -> never
 CoffeeHouse -> never
 CarryAway -> never
 RestaurantLessThan20 -> never
 Resturant20To50 -> never
 
 For Q4, I found out that the total observations chose to accept the coupon is around 56.8% that is by simply count of 1 at column Y
 
 For Q5, i used a pandas horizontal bar to show the distribution of coupon types. From the bar chart, among all 5 different types of coupons, coffee house is the highest.
 
For Q6, seaborn histogram was used to show the temperature distribution.

Investigating the Bar Coupons
For Q1 The question was told to restrict the dataframe to coupon column equal to value Bar only.

For Q2, I used value_counts(normalize=True) to retreive the percentage breakdown of the proportion of bar coupons were accepted. The percentage is around 41% which is less than half. seaborn histogram is also used to show the distribution of percentage of acceptance and rejection.

For Q3, the trend was located for drivers who were visiting Bar for more than 3 times per month. The percentage was around 76.88%, that was pretty hight. Seaborn catplot was used to illustrate the distribution of Bar visit vs counts.

For Q4, we tried to figure out the percentage of drives who were older than 25 years old and visited Bar more than 1 time per month. The percentage was around 69.52%.

For Q5, the acceptance rate between drivers who go to bars more than once a month and had passengers that were not a kid and had occupations other than farming, fishing, or forestry was found, the percentage was around 41%. 

For Q6, the requirements were  
    go to bars more than once a month, had passengers that were not a kid, and were not widowed OR
    go to bars more than once a month and are under the age of 30 OR
    go to cheap restaurants more than 4 times a month and income is less than 50K.
the acceptance rate was calculated as 41%

#the finding is that 
#1 ) for drivers visiting the bar 3 times regardless the age, they are more likely to use the bar coupons
#2) for drivers visiting the bar 1 or more per months with age over 25, they are more likely to use the bar coupons
# the percentage of the above 2 groups have almost double chances to use the coupon.

Independent Investigation
We looked at coupon for Coffee House. df3 = data[data['coupon']=='Coffee House'] 

The proportion of bar coupons were accepted was around 49.92%. Seaborn histogram was used to show the distribution.
Next, we were trying to look for the relationship amoung gender, age and coupon. We noticed that for young generation such as 21 ages old group espically for female, the couple was more accepted. For histogram, we confirmed that age 21 and age 26 were having higher acceptance rate in comparison with other age groups for coupe Coffee House. 

Next, we looked for the relationship among education, age and coupon acceptance, no special trend being identified.

Then, we use seaborn histogram to show the distribution of destination against coupon Coffee House. We noticed that for drivers who were not going to any place urgently were likely to use the coupons.

We found that if drivers were going to Coffee House 1~8 times or more, they were more happy to use the coupon. 

if the passenger on the cars were friends and partners, the drivers were likely to use the coupon
#the final finding for coupon Coffee House is that 
#1 ) for drivers visiting the CoffeeHouse more frequently, they are using the coupons. THe highest rate actually 
#is for those who are visiting 1 to 3 times. 
#2 ) for drivers who have friend passengers, they are more likely to use the coupon. Next is if partner is sitting on the car
#3) if the drivers are not urgent, they are more likely to use the coffee house coupons





