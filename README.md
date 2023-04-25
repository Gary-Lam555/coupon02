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
 
 For Q4, I find that the total observations chose to accept the coupon is around 56.8% that is by simply count of 1 at column Y
 
 For Q5, i use a pandas horizontal bar to show the distribution of coupon type. From the bar chart, we understand the highest coupon type s
 
