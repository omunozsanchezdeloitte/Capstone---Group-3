# Empower Automotive - Used Car Price Analysis

![cars](https://th.bing.com/th/id/R.9afaff6944accabe5dc55f713134f5fa?rik=ha%2fls5fh6wMN2Q&riu=http%3a%2f%2fmcity.umich.edu%2fwp-content%2fuploads%2f2017%2f02%2fcar-sunrise.jpg&ehk=3ZQbYDUCnoP09vNWkQ1uj7XLQWarfDz6hUJY1pmOLy8%3d&risl=&pid=ImgRaw&r=0)

## Overview
Imagine this: you're looking to sell your used car, and you have no idea where to begin in coming up with a price. We've all been there. That is where Empower Automotive comes in. This brand-new app is working to become a major player in the automtotive industry. You download the app, snap a photo of your car, potentially fill in some unidenfitifed details, and the app recommends a reasonable price to sell your car for.

Extensive data, such as those incorporating price, production year, leather interior, and milage, in conjuction with powerful AI models, such as linear regression, random forest, and XGBoost with LASSO, have gone into the creation of this app. Our final recommended model, ___, did an effective job at solving the problem.

In our report we will cover:
1. Business Understanding: The goal, key business questions, and stakeholders.
2. Data Understanding & Analysis: Data sources, descriptions, and visualizations.
3. Conclusion: Relevant findings and recommendations. 

Related Presentation, Jupyer Notebook, and Data Sources are linked below:
1. PowerPoint Presentation
2. Jupyter Notebook
3. Data Sources

## Business Understanding
Empower Automotive is an app that users can use to help set a price on their used car.

### Goal
Empower Automotive's goal is to help users analyze what price would be the most accurate, competitive, and successful for selling their cars. We formed key questions to answer in order to provide the stakeholders our best recommendations.

### Key Business Questions
1. What features are the most important when accurately pricing a car?
2. What is the relationship between car price and year?
3. What is the relationship between leather interior and price?
4. How can Empower Automotive become a trusted source for used car prices?

### Stakeholders
1. Empower Automotive Executives
2. Car buyers
3. Car sellers

## Data Understanding and Analysis
We examined data from Kaggle Dataset "Car Price Prediction Challenge". We focused on the Price, Prod. year, Leather interior and Mileage features for our models.

### Descriptions of Data
Our first step was to implement some data cleaning in this data set which includes

Replacing null values to 0 or remove them. This allows us to be able to convert data types to float.

### Visualizations and Modeling
We created visualizations to help support our questions and analysis.

Price and Mileage 
This graph shows cars with the lowest mileage have a higher selling price than those with high mileage.




Price and Production Year
This graph shows newer models of cars have a higher selling price than older models. There are some instances where the car is older but has a higher price tag because it is vintage or a one of a kind.




Price and Leather Interior 
This box and whisker plot shows cars with leather interior tend to have higher price tags but the averages of leather vs cloth are similar showing that leather interior does not have that much of a value add when selling used cars.

## Conclusion
We recommend Empower Automotive to use the xxx modeling technique as it proves to be the most accurate. 
