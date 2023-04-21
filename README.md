# PHASE 2 PROJECT
# KING COUNTY HOUSE SALE ANALYSIS
# Project Description
## Introduction
With nearly 2.2 million residents, King County is the largest county in Washington State. Nationally, it is the 13th largest by population and ninth largest by total employment. Two million of its residents live in one of the 39 cities in the county and the remaining 200,000 in the unincorporated area. Seattle, the largest city in the county, is home to 730,000 residents
It is home to Seattle, the state's largest city, and is a hub of innovation, technology, and creative industries. The housing market in King County has been one of the fastest-growing in the country, with strong demand and limited supply leading to a highly competitive market.
Several nationally-known businesses are collectively the major economic drivers for the region: Amazon, Boeing Commercial Airplanes, Microsoft, Starbucks and the University of Washington. These large businesses, and along with smaller enterprises, have led King County out of the Great Recession and into a period of overall economic growth.

# The challenge
At its core, the housing crisis is driven by a supply and demand challenge that is two-fold. First, since 2012, King County’s population has grown faster than new homes have been built, creating a growing gap between supply and demand. Second, King County’s population has not grown evenly across the income spectrum. Sixty percent of the new households in King County between 2006 and 2016 earned USD 125,000 or more per year, while 18 percent earned less than USD 50,000. Middle income earners constituted only 22 percent of new households

New real estate developers are planning to build new housing facilities and there has been a problem in evaluating homes in King County. 
Objectives
Throughout the course of the project, we will answer several questions:
    • To develop a model that will help in identifying the attributes that bring more value to the houses, hence bringing maximum profit. Specifically, to uncover:
    • Which features have the biggest impact on the sale price of a house?
    • How much does location affect the sale price of a house?
    • To create a regression model to advice developers on how to accurately price a property
    
Our Role as data scientists is to advice New real estate developers who are planning to build new housing facilities on what factors come into play   while evaluating new housing facilities in King County
    
    ## Data Understanding
    An image of the dateset
   ![alt text](https://github.com/Cynthiah-Mulwo/dsc-phase-2-project-v2-3/blob/master/Screenshot%20from%202023-04-20%2019-35-47.png)
   
Here we will explore the data to get a better understanding of its state, then decide on the steps we need to take to clean it. We will begin by defining some helper functions for the following tasks:
- getting the shape of the data
- getting data info
- simple check for missing data
- duplicates
- descriptive stats

We will then group together the helper function under a new function that explores the data for the above attributes

# Explolatory Data Analysis
We will explore the following areas to set context for the presentation
- Average Price of property based on number of bedrooms
- Average Price of property based on the condition of the property
- Regions (North, East, Seattle & South)
- Price distribution
- Houses Sold Per Quarter

Some of the visualisations are created:
Avarage price of houses based on the number of bedrooms

 ![alt text](https://github.com/Cynthiah-Mulwo/dsc-phase-2-project-v2-3/blob/master/Screenshot%20from%202023-04-20%2019-53-43.png)

Avarage price of the property based on the condition of the property
![alt text](https://github.com/Cynthiah-Mulwo/dsc-phase-2-project-v2-3/blob/master/Screenshot%20from%202023-04-20%2019-58-34.png)


# Modeling 
This section demonstrates the Linear modeling process, from the baseline model to the multiple regression model

A scatter plot illustrating the linear relationship between the columns used in the baseline model(living space vs price)
![alt text](https://github.com/Cynthiah-Mulwo/dsc-phase-2-project-v2-3/blob/master/Screenshot%20from%202023-04-20%2020-02-55.png)

# Success Metrics 
We will use RSQUARED and MAE to meet 2 objectives:
- Rsquared will help us asses model improvements in prediction variation in house prices
- mean absolute error will help us to measure the distance of the predicted prices from the actual prices. From the code below, we have chosen mae over rmse because it is less infuenced by outliers

# Conclusions:
1. Bedrooms, bathrooms, square footage of living space, number of floors, and the condition of the house are all significant predictors of the price of a house.
2. The quarter of the year in which the house was sold also appears to have a small effect on the price.
3. The third model explains only about 60.8% of the variance in the price of the house.
4. The limitations of the data used to train the model should be considered.
