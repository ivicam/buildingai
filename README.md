# Create personalized recommendations for Customers in fast food restaurant

Final project for the Building AI course

## Summary

Goal of this project would be to create system which would display recommendations tailored to each Customer preferences based on the historical data for each Customer. Data will be gathered using information about order history crossreferenced with other information which could be used to connect it to the specific Customer (e.g. loyalty card, credit card information, vehicle licenceplate on drive-in etc.). Recommendations will be displayed to Customer on self-service kiosks and at menu display board in drive-in.


## Background

In recent years fast-food sales have slowed as people turn to the alternatives. By using recommendation system, products with highest probability to be sold for specific Customer will be recommended what should have positive impact on sale. 

## How is it used?
First step is to identify specific Customer. For this purpose, it will be used following methods:
- indoor - for example via loyalty card
- drive-in - for example by car licenceplate

After Customer is positively identified, background system will need in short period of time before Customer places an order, create recommendations and display them to the Customer. Recommendations could be displayed, for example:
- indoor - as part of graphical user interface on self-service kiosk
- outdoor - as part of display placed at drive-in

## Data sources and AI methods
System woudl require following data sources:
- information required to identify Customers - e.g. via loyalty card system or by using automatic number plate recognition (ANPR) at drive-in
- information about Customers - e.g. information about age of the Customer, gender
- information about previous order history for the Customer - this information should be available in interal database of the company
- Other relevant information - e.g. actual weather conditions to create weather based recommendations (e.g. cold drink in summer, hot dring in winter) from publicly available public weather services (for example: WeatherStack API), information about actual marketing campaigns (e.g. to prefer articles which are currently in special offer etc.)

After Customer is positively identified, information will be provided to recommendation system. Recommendation system will be based on neural network. As it is expected that it will be required to process large amount of data in short period, task will be roughly divided into two sub-tasks:
1. choose top N-candidates
2. ranking them

Output of the recommendation system will be one or more items which will be then displayed to the Customer during order generation process.

## Challenges

In order to objectively evaluate quality of the model it will be required to define appropriate quality metrics, specially for recommendation systems (e.g. Recall@k, Precision@k).

As system requires some amount of personal data to be collected, this should be done with Customer consent and in compliance with with local law on data protection and privacy. 

## What next?



## Acknowledgments
Recommendation System Algorithms by Daniil Korbut (link: https://blog.statsbot.co/recommendation-system-algorithms-ba67f39ac9a3, retrieved on 30.12.2020)
