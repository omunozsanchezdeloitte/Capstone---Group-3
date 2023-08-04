# Empower Automotive - Used Car Price Analysis

![cars](https://th.bing.com/th/id/R.9afaff6944accabe5dc55f713134f5fa?rik=ha%2fls5fh6wMN2Q&riu=http%3a%2f%2fmcity.umich.edu%2fwp-content%2fuploads%2f2017%2f02%2fcar-sunrise.jpg&ehk=3ZQbYDUCnoP09vNWkQ1uj7XLQWarfDz6hUJY1pmOLy8%3d&risl=&pid=ImgRaw&r=0)

## Overview
Imagine this: you're looking to sell your used car, and you have no idea where to begin in coming up with a price. We've all been there. That is where Empower Automotive comes in. This brand-new app is working to become a major player in the automtotive industry. You download the app, snap a photo of your car, potentially fill in some unidenfitifed details, and the app recommends a reasonable price to sell your car for.

Extensive data, such as those incorporating price, production year, leather interior, and mileage, in conjuction with powerful AI models, such as linear regression, random forest, and XGBoost with LASSO, have gone into the creation of this app. Our final recommended model, XGBoost with LASSO, did an effective job at solving the problem.

In our report we will cover:
1. Business Understanding: The goal, key business questions, and stakeholders.
2. Data Understanding & Analysis: Data sources, descriptions, and visualizations.
3. Conclusion: Relevant findings and recommendations. 

Related Presentation, Jupyer Notebook, and Data Sources are linked below:
1. PowerPoint Presentation
2. Jupyter Notebook
3. Data Sources

This GitHub repository is a one-stop shop for this project. We have a main branch, as well as a branch for each project member: Hannah, Sasha, Cristian, Oscar, and Jordan. In the files section you can find the dataset, PowerPoint Presentation, and Jupyter Notebooks. The README provides a summary of everything regarding the project, as well as the links to those files.

## Business Understanding
Empower Automotive is an app that users can use to help set a price on their used car.

### Goal
Empower Automotive's goal is to help users analyze what price would be the most accurate, competitive, and successful for selling their cars. Our goal is to provide Empower Automotive a recommendation based on data analysis of linear regression, random forest, and XGBoost with LASSO. We formed key business questions and will consider stakeholder input to provide the recommendation.

### Key Business Questions
1. What features are the most important when accurately pricing a car?
2. How can Empower Automotive become a trusted source for used car prices?

### Stakeholders
1. Empower Automotive Executives
2. Car sellers & buyers

## Data Understanding & Analysis
### Descriptions of Data

We examined data from Kaggle Dataset "Car Price Prediction Challenge". We focused on the Price, Prod. year, Leather interior, and Mileage features for our models.

![image](https://github.com/omunozsanchezdeloitte/Capstone---Group-3/assets/125094602/1ef59da8-3979-461c-9d31-7db5ebd3b4eb)

(https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge)

Our first step was to implement some data cleaning in this data set. We replaced null values to 0 or removed them. This allows us to be able to convert data types to float.

Then we began modeling with our selected, cleaned data in order to provide the best recommendation.

### Model Selection Evaluation
1. Linear Regression
   - Base will always be linear
   - There was no significant difference between the base and linear
   * Continued to follow up with more complex models that are more common and suitable for regression problems: 
2. Random Forest
   - One of the most common models for regression
   - Simplicity and high accuracy
3. XGBoost with LASSO
   - Execution speed and model performance
   - Simplicity and high accuracy

### Modeling & Evaluation
We used models to analyze our main business questions. We created visualizations to help support our questions and analysis.

#### Price & Production Year - Linear Regression

![image](https://github.com/omunozsanchezdeloitte/Capstone---Group-3/assets/125094602/f9311b79-0935-49e8-b299-e20270a398da)

- The graph demonstrates the newer the car, the higher the price

#### Price & Production Year + Engine Volume - Random Forest

![image](https://github.com/omunozsanchezdeloitte/Capstone---Group-3/assets/125094602/8690f936-b4ee-4516-9bdf-603d8cfdc768)

- This graph shows newer models of cars have a higher selling price than older models of cars
- Engine volume and mileage are also important influencers on the price for this model

#### Price & Type of Aspiration - XGBoost with LASSO

![image](https://github.com/omunozsanchezdeloitte/Capstone---Group-3/assets/125094602/72d69825-49ad-4fd1-bfe0-06fd0c4c3e92)

- Better performance than previous models
- Different features account the most for this model

## Conclusion
1. What features are the most important when accurately pricing a car?
    - The most important features for determining car prices are Year of Production, Engine Volume and Aspiration Type
2. How can Empower Automotive become a trusted source for used car prices?
    - Empower can become a trusted source by using the most up-to-date car data and continuing to add features that are useful for sellers and buyers, especially features related with the condition of the car

In comparing linear regression, random forest, and XGBoost with LASSO, our recommendation is for Empower Automotive to use XGBoost with LASSO. This model proved to be the most accurate, with the smallest RMSE and a strong R2.

### Next Steps
1. Implement more complex models:
   - Neural Network
2. Tune current model to include more correlated features to price and condition of the car
