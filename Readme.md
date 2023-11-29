# Airline Flight Delay Analysis and Modeling  
## MS-AAI-501 Introduction to Artificial Intelligence
This README docuemts the Final Team project of Course #2 in the University of San Diego's Master's program for Applied Artificial Intelligence.

## Installation
Python 3.8 or later is needed along with installed libraries including:
* pandas
* numpy
* datetime
* statsmodels
* sklearn
* matplotlib
* category_encoders
* XGBoost
* tensorflow
* seaborn

## Project Intro / Objective
Flight delays, an inherent challenge in contemporary travel, pose significant repercussions for both airlines and passengers.  They are a pervasive issue incurring substantial costs for airlines, tarnishing their reputation, and causing frustration among passengers.  This project seeks to investigate this industry-wide concern by delving into the intricacies of Domestic US airline flight delays. Our project is motivated by the need to alleviate these challenges by unraveling the complexities behind flight delays and proposing intelligent predictive solutions.  Our team aims to comprehensively understand the factors contributing to delays and, subsequently, employ artificial intelligence models to predict these disruptions.  By focusing on this binary classification problem, we intend to deploy a range of models, including Logistic Regression, Neural Nets, Random Forest Trees, and Gradient Boosting, to optimize predictive accuracy.

We supplement base airline traffic data (e.g. flight date, carrier, origin and destination, and distance) with weather data and carrier employee data to enrich our feature set.  The algorithms will be used to predict delays and our analysis into these models will explain feature relevance, patterns, and correlations.  
In this project we will focus on dataset identification, preprocessing and programmatically enriching these datasets for additional features, statistical analysis, and data visualizations.  Once we are ready to involve models we will analyze the model behavior, perform parameter tuning, and compare model performance to identify the best type of model for this classification problem.

## Partners / Contributions
<b>Ned Kost</b>:  Data Collection (Carrier Employee Data), Data Analysis, Data Preprocessing, Logistic Regression, XGBoos Classifier  
<b>Brian Morris</b>:  Data Collection (weather), Data Analysis, Data Preprocessing, Neural Net, Random Forest  
<b>Anova Youngers</b>:  Data Analysis, Data Preprocessing, Data Visualizations, Neural Net, Random Forest  

## Project Description & Methodology
Data Collection and Aggregation:  The past 3 years of <a href=https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=FGJ>Airline On-Time Perormance</a> data data was downlated from the Bureau of Transportation <a href=https://www.transtats.bts.gov/databases.asp?Z1qr_VQ=E&Z1qr_Qr5p=N8vn6v10&f7owrp6_VQF=D>website<a>.  Once downloaded, the data was correlated into a single large dataset and randomply sampled for equal distributions of Delayed and Non-Delayed flights.  

Data Exploration and Analytics:

Data Preprocessing:

Data Modeling:

## License
This project is privded under the Apache License 2.0.  Please see the [LICENSE](https://github.com/NedKost/usd_data_hackathon_2023/blob/main/LICENSE) file for more information.

## Acknowledgements
