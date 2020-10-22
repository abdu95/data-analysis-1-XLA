# data-analysis-1-XLA
Data Analysis 1, Task 2: Team project. 
Pizza dataset report

Data in this set were collected online from different pizza places in inner Budapest and outer Budapest, which contain prices of 32cm margherita pizza and of 0.5L beverage. 

As the size difference between 30 cm, 31cm and 32cm pizza is not too much (1-2 cm) and their price are almost identical (with 100-400 Hungarian forint difference), we decided to consider these pizzas as of the same type (category), and recorded them in one column **marpizza_price 30-32cm (in HUF)**.
As Pepsi, Cola, Sprite, Canada Dry is offered in the Soft Drinks category in many pizzerias and their prices are almost same, we included them in one variable called **beverage_price 0.5L (In HUF)**. In some other pizzerias, some other type of soft drinks and 0.5l beers were available. Therefore, we decided to include them also as a beverage to this variable

There are 44 places found, 22 from inner Budapest and the other 22 from outer Budapest.

Rating scores, as well as the number of ratings, are from Google Reviews of each restaurant. <br />
Example link: https://goo.gl/maps/AGiJ8kHaBxTphBmj7

All restaurants were searched via Google Map, with food prices displayed on each restaurant's website menu or their Netpincer webpages.
Example link: https://www.netpincer.hu/en/restaurant/o5vp/la-trattoria 

Distances (from CEU campus to the pizza restaurant) are from Google map. We took the shortest distance between the two places. 

We also added addresses of each restaurant as explanatory notes (not as a variable for analysis).


# Data collection, difficulties, problems.
### Entity Resolution 
To avoid duplicates and maintain consistency, all three members of the team recorded their findings (observations) in one Google Sheet. However, at some point of the process, we figured out that they are some duplicates. We decided to leave one such observation and drop the other duplicate observations as they had the same value for all variables.

### Validity 
### Reliability 
### Missing Values(pizza found, Google review not found)
### Extreme Values

### Problem 1
Deciding which size of pizza to choose was problematic. Pizza restaurants were offering the pizzas of size 28cm, 30cm, 32 cm, 48cm and even more. Thus, we initially decided to start analyzing all the restaurants and record the price for pizza  of size 28cm, 30cm, and 32 cm as we met these sizes most frequently. We had a column for price of pizza with the size 28 cm and 32 cm. As the pizza of size 30cm and 32cm were observed most frequently, we decided to drop the column for price of pizza with the size 28 cm and leave the column for the price of pizza with the size 32 cm.

### Problem 2
Deciding which method to use for measuring the distance was also problematic. At the beginning, two team members used "Measure distance" functionality of the Google Map. However, 3rd member of the group used "Show directions" functionality. Even though both methods are valid (shows the distance between two points), "Show directions" functionality shows the fastest and shortest path. Therefore, it shows different distances when checked different times. It may vary based on the traffic jam, maintenance work in roads or due to other reasons. However, "Measure distance" functionality works as a "ruler on the map" manner and shows the same distance between two points no matter when the distance was checked. To maintain the comparability, 3rd member of the group also decided to change the values for variable "distance" by using
