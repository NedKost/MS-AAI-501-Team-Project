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
**Data Collection and Aggregation**:  The past 3 years of [Airline On-Time Perormance](https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=FGJ) data data was downloaded from the Bureau of Transportation [website](https://www.transtats.bts.gov/databases.asp?Z1qr_VQ=E&Z1qr_Qr5p=N8vn6v10&f7owrp6_VQF=D), and supplemented with Carrier Employee data  also downloaded from the Bureau of Transportation [website](https://www.transtats.bts.gov/Employment/).  Once downloaded, the data was correlated into a single large dataset and randomly sampled for equal distributions of 360,000 Delayed and Non-Delayed flights. An API call was used to supplement this dataset from the [National Oceanic and Atmospheric Administration](https://www.ncei.noaa.gov/products/land-based-station/integrated-surface-database).  Since the original 3 years of flight data was too large, we only supplmeneted this smaller dataset with weather data due to time constraints in pulling data for each individual flight.
Notebooks used:
- data_preprocessing
- data_preprocessing_large
- data_preprocessing_weather

**Data Exploration and Analytics**:  We performed data exploration and statistical analysis on the full 3 years of flight data to identify trends and feature relevance.  We aligned on 3 feature sets that each represented data from separate phases of a flights lifecycle. 
**Feature Set 1 (pre-departure)**:   Features in this set could be used before the flight even departs in order to predict whether or not it would be delayed.  Models using only these features to predict flight delays may help airlines be proactive about handling delayed flights with plenty of time to mitigate issues.
- Year, Quarter, Month, DayOfMonth, DayofWeek, Origin, Dest, CRSDepTime, CRSArrTime, CRSElapsedTime, Distance, Carrier,
- Employee Full-time, Employee Part-time, Employees Grand Total,
- Aircraft_Daily_Flight_Count
- Origin_Windspeed, Prigin_Precip, Dest_Windspeed, Dest_Precip, Origin_ianaTimezone, Dest_ianaTimezone

**Feature Set 2 (departure)**:  Features in this set could be used up till the plane departs in order to predict possible arrival delays.  Models using features from set 1 and 2 should have a much higher accuracy, and could still be used by airlines to mitigate the delay while the plane is in flight.
- DepTime, DepDelay
- TaxiOff, WheelsOff

**Feature Set 3 (pre-arrival)**:  Features in this set include times up till the plane arrives at the gate.  Models using features from all three sets will be very accurate, but may not be helpful for airlines to mitigate delays (it would already be known that the plan is delayed).  Model analysis with this data could be useful for airlines to study airline flights historically or through model analysis.
- AirTime
- WheelsOn
- TaxiIn

Notebooks used: 
- Data Exploration_NK
- data_explore_sigtest

Data Modeling:  Once the dataset was understood, we began formulating various models to test with each of the feature sets.

Notebooks used
- Logistic Regression
- neural_net
- neural_net_large_dataset
- Neural_NetFlight
- random_forest
- random_ForestFlight_Failed
- XGBoost Model

## License
This project is privded under the Apache License 2.0.  Please see the [LICENSE](https://github.com/NedKost/usd_data_hackathon_2023/blob/main/LICENSE) file for more information.

## Acknowledgements
