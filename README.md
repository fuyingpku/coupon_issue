First of all, Github desktop is working well (for me for the first time, hopefully the update is in real time).....please see the link for the coding: https://github.com/fuyingpku/coupon_issue/blob/8172c660424a4a3193f6a7903751b369160994a7/Untitled.ipynb

Goal: “Will a customer accept the coupon?” 

Study goal: The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not. 

Data Description:

Data input: This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, passenger, etc., and then asks people whether they will accept the coupon if they are the driver. Answers given that the users will drive there “right away” or “later before the coupon expires” are labeled as “Y = 1”, and answers “no, I do not want the coupon” are labeled as “Y = 0”. There are five different types of coupons—less expensive restaurants (under $20), coffee houses, carry out and take away, bars, and more expensive restaurants ($20–$50).

Data analysis:  'destination', 'passanger', 'weather', 'temperature', 'time', 'coupon',
       'expiration', 'gender', 'age', 'maritalStatus', 'has_children',
       'education', 'occupation', 'income', 'car', 'Bar', 'CoffeeHouse',
       'CarryAway', 'RestaurantLessThan20', 'Restaurant20To50',
       'toCoupon_GEQ5min', 'toCoupon_GEQ15min', 'toCoupon_GEQ25min',
       'direction_same', 'direction_opp', 'Y'],

Further analysis focusing on 25 features below: 
[(0, 'destination'),
 (1, 'passanger'),
 (2, 'weather'),
 (3, 'temperature'),
 (4, 'time'),
 (5, 'coupon'),
 (6, 'expiration'),
 (7, 'gender'),
 (8, 'age'),
 (9, 'maritalStatus'),
 (10, 'has_children'),
 (11, 'education'),
 (12, 'occupation'),
 (13, 'income'),
 (14, 'car'),
 (15, 'Bar'),
 (16, 'CoffeeHouse'),
 (17, 'CarryAway'),
 (18, 'RestaurantLessThan20'),
 (19, 'Restaurant20To50'),
 (20, 'toCoupon_GEQ5min'),
 (21, 'toCoupon_GEQ15min'),
 (22, 'toCoupon_GEQ25min'),
 (23, 'direction_same'),
 (24, 'direction_opp')]
 
Overall analysis for sub-population who is more willing to take the coupon: 
 
1. Destination is playing a role, but only for people who has not immediate place to go. Highlight the req of taking the coupon: time
2. Driving passenger sure with friend(s) is more prone to take the coupon. Highlight the importance of why takin the coupon: social
3. Weather is also important, sunny day make people tend to take the coupon. 
4. Temperatue (as high as 80) also make people tend to take the coupon, probably due to the need (importance/usage of the coupon). 
5. Time (timing) surely make us to think about late afternoon (could be off work early) make it more feasible for people to take the coupon. 
6. The coupon type: restaurants, carry out/take away makes people think an easy gain so tend to accept the coupon more. 
7. Expriation date: everyone like to accpet longer expiration date. 
8. Male has higher chance to take the coupon 
9. Age seems not a major factor to make the decision in favor of taking the coupon. 
10. Single (mariage status) seems align with the major function to take the coupon more than others.
11. Align with single, no kid probably indicate more time to spend using the coupon, so more likely to take the coupon. 
12. Education seems give us some hints on differences, however, there is no clear trend about higher education or lower education group has obvious trend. 
13. Occupation also does not make a clear call 
14. Income seems not playing a role in this case
15. Not sure why driving old car seems make people prefer to take the coupon
16. Bar seems a good better choice than others, but restaurants has to be close (less than 20miles). 
17. Direction is quite interesting and playing a major role in this case.
 
 Conclusions and Furture recommendations: 
 We have seen everything make sense that pepole has time (single, no rush to anyhwere, good timing after work or lunch) tend to prefer to accept the coupon. However, in this design, we did not see clear data plan wiht hypothesis and it is quite long questionire that I personally not sure who will address such long question list and their mode in the very end could escaping this ASAP! I would recommend a hypothesis driven design of questions with 10-12 max questions. The goal would targeting devliery/motivation to take the coupon and go with it. Final reading of coupon usage is missing here which is more important. 
 
 
 
 
 


