# Car Pricing Research

Given a dataset which contained the characteristics of used vehicles and their prices, we wanted to explore key driving factors for used car prices. With this knowledge, our stakeholders can learn the intricacies of what customers prefer in a vehicle and shift their market more towards this thought bubble. With that in mind, our goal with this dataset is to then figure out what specific features and characteristics of a vehicle are the most important towards influencing its price and thus using this available knowledge to better our resoruces to satisfying customer needs and in turn making profit.

### Build Set up

First we'll filter the dataset into a usable format for machine learning. What we're aiming for is a computer model that predicts prices of these used cars based on their characteristiics. The characteristics that are the most prominent in the model (ie have the largest numerical values) will then be the key driving factors for car prices! The set up begins with cleaning the dataset for the variables that would be of most interest before transforming them to be usable for the computer model. In this case we've chosen the following features for their likelihood of major relationship to car prices:

- region of vehicle
- manufacturer of vehicle
- condition	of vehicle
- Number of cylinders vehicle contains
- fuel type of vehicle
- max distance traveled on vehicle
- type of vehicle
- title-status of vehicle
- vehicle age

From there, we begin setting up a computer model which learns which features (and more directly which groupings of specific features) to utilize best upon to predict pricing and slowly train multiple computer models utilizing hyper parameter tuning and cross validation. Once both are done, we train one last time with certain specifics that we deemed best fit for our model creation here to create the best computer model utilizing the information we have that comes the closest to predicting the given used car prices.

### Results
