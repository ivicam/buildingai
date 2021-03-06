
# Create personalized recommendations in fast food restaurant

Final project for the Building AI course

## Summary

Create system which would display recommendations tailored to each Customer preferences based on the historical data for each Customer. Recommendations will be displayed to Customer on self-service kiosks and at menu display board in drive-in. 


## Background

In recent years fast-food sales have slowed as people turn to the alternatives. By using recommendation system, products with highest probability to be sold for specific Customer will be recommended what should have positive impact on sale.

## How is it used?

irst step is to identify specific Customer. For this purpose, it will be used following methods:
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
fter Customer is positively identified, information will be provided to recommendation system. Recommendation system will be based on neural network. As it is expected that it will be required to process large amount of data in short period, task will be roughly divided into two sub-tasks:
1. choose top N-candidates
2. ranking them

Output of the recommendation system will be one or more items which will be then displayed to the Customer during order generation process.

## Challenges

In order to objectively evaluate quality of the model it will be required to define appropriate quality metrics, specially for recommendation systems (e.g. Recall@k, Precision@k).

As system requires some amount of personal data to be collected, this should be done with Customer consent and in compliance with with local law on data protection and privacy.

## What next?

Next step would be to create data model for data sources for Customer, orders and items and then to start building the model of the recommendation system. Anyone interested to help are welcome to contribute. 


## Acknowledgments

Recommendation System Algorithms by Daniil Korbut (link: https://blog.statsbot.co/recommendation-system-algorithms-ba67f39ac9a3, retrieved on 30.12.2020)
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc
