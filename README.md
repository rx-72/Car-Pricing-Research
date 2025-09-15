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

Once our best model was chosen, we looked into the features that it utilize most prominently for prediction based on numerical strength. The first features of major notice were the car age and the distance traveled of the vehicle. In particular, higher car age was correlated with  higher prices while higher distances traveled was correlated with lower prices. It seems here that age is interestingly more valued despite depreciation in a vehicle while total distances traveled implies less reliability, at least according to customers.

In terms of manufacturer brand, multiple groups of these were chosen to be impactful towards the pricing, though at various strengths. The most strongest one was vehicles of the tesla brand were more likely to be higher priced, indicating a preference for this more unique brand. Other similar high priced brands include Porsche, Jaguar, and Rover. On the flip end, brands such as Hyundai, Dodge, and Kia were more like to be lower pricing for customers, perhaps due to the more commonality of these brands

The feature region played a large part in pricing as multiple regions proved to particularly strong in influencing pricing both for higher rates ('olympic peninsula', 'great falls', 'anchorage') and lower as well ('southern maryland', 'joplin', 'fort smith'). That said, it seems that the region of the vehicle is more likely to affect the price negatively (as seen where the strongest numerical value positively was 1.6 whereas negative it was -3.367). This seems to suggest that region areas is more of a factor that costs vehicle to be paid for less in pricings, being especially more dependent on origin.

The vehicle type had multiple factors for pricing played on it, where types such as pickup and convertibles influenced higher rates and others like sedan and truck suggested lower rates. That said, the strength of these values were rather low (In numerical terms, 0.55 vs -0.67 on -1 to 1 scale) so while type is useful, it's not as helpful for pricing influences as other factors.

The condition of the vehicle proved particularly useful when the condition was labelled "good", which contained a numerical value of 1.016. In this case, it seems customer highly value better conditions for the vehicles (which makes sense considering customer interest) and because of that, positive status such as "good" for condition would there influence the pricing higher due to be more favored.

Vehicle fuel was considered in the model however proved to be rather weak in terms of numerical strength (ranging between 0.11 to -0.45 and thus not a strong relation to pricing). The main exception is the fuel listed "unknown" being at 0.89 numerical strength, but this isn't relatively useful or make sense that due to the vehicle fuel status being unknown, it would cost more. Some research of the unlisted fuel types on these vehicles would prove useful here.

Cylinder counts of the vehicle varied extremely in numerical strength with no pattern to determine (For instance, 8 cylinders has 0.15 as its coefficient, 10 cylinders has -0.78, but 4 cylinders had -0.07). Overall while there's strengths in feature (10 cylinders at -0.78 and unknown count at -0.92) since the data isn't very well spread here, some more research is needed in this area to better determine the relationship in this case.

Finally title status of the vehicle was particularly useful for pricing when the vehicle was labeled "missing" at a numerical value of -1.08. This implies missing vehicles would in turn gain a reduction in price (which does follow). All other statuses with either of lower importance or not deemed useful by the model

### Conclusions and Next Steps

From our listed features inputted into our model, we were able to find stronger relational factors that helped people influence to higher and lower pricings on used vehicles. In particularly car age and odometer each played a relatively strong factor, though both on opposite spectrums where car age influenced price increase and the latter for odometer. Condition and status also played important factors, where "good" conditions were satisfactory and led to high pricings whereas being labeled "missing" dropped pricing and customer interest. Region also proved to be extremely effective against pricings where specific regions were more likely to be priced higher and lower depending on said region location of the vehicle. Brand manufacturer also made a similar case where certain brands were priced higher and others were priced lower. That said both of these features were certainly weaker than the first few we mentioned. Finally we had features that the model found useful but a relationship cannot be pulled as to why. Specifically cylinder counts and the vehicle fuel fell under this description. The next few steps suggestions would include investigating the usefulness of these features and why the model found them to be so strong along with working with the already strong features we have and trying to gain further explanations and vehicle focus on these characteristics to target more of our customer base.
