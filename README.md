# CRIME DATA ANALYSIS

![Crime-Data-Analysis](https://github.com/ddhaval04/Smart-City/raw/master/images/smart-city-header.png)


## INTRODUCTION:

A smart city is an urban development vision to integrate multiple information and communication technology (ICT) and Internet of Things (IoT) solutions in a secure fashion to manage a city's assets – the city's assets include, but are not limited to, local departments' information systems, schools, libraries, transportation systems, hospitals, power plants, water supply networks, waste management, law enforcement, and other community services. 
The goal of building a smart city is to improve quality of life by using urban informatics and technology to improve the efficiency of services and meet residents' needs.

## BUSINESS PROBLEM TO SOLVE:

Providing safety is crucial to improve the quality of life in the cities, and has a significant impact on the promotion of economic growth. Public security is a growing problem for cities worldwide. The world’s cities are bursting at the seams, civic resources are under pressure and crime is harder than ever to police.  Safe neighborhood is the one of the fundamental factor for developing city to become a smart city.  This is the business problem, to reduce the crime rate in cities.

## WHY THE PROBLEM IS IMPORTANT TO SOLVE?  

To promote health, safety and security, it’s important to solve this problem. Reducing the crime rate will have a positive socio-economic impact on the society. It would lead to improve the businesses of some real-estate areas and also help small businesses like grocery stores, restaurants etc.  It would have the authorities more aware about certain locations and timings which would help them operate more efficiently.

## IDEA:

Our vision behind this problem statement is to reduce the crime rate in the city to make it safe and smart. In order to reduce the crime rate we need to not only respond to the crime but prevent the crime from occurring in first place and our idea is to predict if the accused is arrested for the given crime type and work effectively to avoid such crimes from occurring where the accused is not likely to be arrested and hence achieve low crime rate in the city.
The goal here is to develop a model based on the crime data that help the authorities to make effective decision and implement effective strategy to keep the city safe and evolve as a smart city.
Crime data analysis is fundamental to effective crime prevention. Knowing as much as you can about crime will help significantly in its prevention.
Determining if particular crimes are increasing; identifying the hot spot locations where crime is concentrated; understanding the temporal trends of offending and analyzing potential reasons for crime trends will be critical features of crime data analysis.


## WHAT DIFFERENCES YOU COULD MAKE WITH YOUR DATA SCIENCE APPROACH?

With the access to large amounts of data and with increasingly smarter statistical analysis, we will be able to use the collected data to foresee and percept various types of criminal acts at a particular time and location, before they even occur.
Such insight will enable city authorities to detect areas of increased crime, which will give them the opportunity to act more deliberately and deploy officers more intelligently, e.g. sending them to the areas that are more exposed to crime. With such systems, police officers will not only respond to criminal acts, but will also be able to act proactively and stop them before they occur.
In order to reduce the crime rate of the city, our solution is not limited to responding to the crime but also to prevent crime from occurring in first place by identifying the crime type that needs more attention by authorities.
We originally categorized the dataset by type, time and location, based on our findings by our problem statements discussed above.
- Crime types: Our model predicts the crime type that requires more attention in order to reduce the crime rate. 
- By Locations: Our model predicts the Location that requires more attention for a specific location at specific time, which will help prevent the occurrence of crime and reduce the crime rate.
- By Time: Interesting finding of our model was, the general notion of more crimes taking place during night hours is actually not true. Analysis indicates that most of the crimes occur during day time and during weekdays. 

## DATA COLLECTION:

Our major source of crime data for city of Chicago was from   https://data.cityofchicago.org/.
The website hosts official public record on every crime that is reported to Chicago police department. The dataset does have a limitation with personal records to maintain the privacy. Apart from crime dataset, we also explored in collecting few other datasets required to address and analyses the crime and other related factors that’s could help control the crime to build smart city.

Few other datasets were:
- Police data of city of Chicago
- Real Estate data for city of Chicago
- School dataset

Dataset Size:  The dataset includes the crime data from 2001 through 2016, with total observations of 6,193,548.

Training Set: Dataset from year 2001-2015
Test Set: Dataset from year 2016

## DATA ISSUES:

There were few limitations with the dataset. 
- Data Skewness: the skewed data and was not good for our analysis over years which would lead to bias results. 
- Null values: lots of observations had no values or invalid information’s.
- Drop NA

## DATA PREPROCESSING:

 As explained earlier we collected data from city of Chicago website. This data consists of few columns to play on. So, we decided to add additional columns by transforming Timestamp column into Date, Day, Month, Year, Time of the day (Morning, Afternoon, Night).

 Also, we extracted Zip Codes using `geolocator` library in python using latitude and longitude given in data set.

  We have attached the screenshot on the interactive visualization which helps user to get insight about crime data set and using which he can make decisions to reduce the crime. The visualization are performed on the columns which are highly correlated to our targets.


## SOLUTION:

- Implemented Logistic Regression and LDA (Linear Discriminant Analysis).

## INTERACTIVE JUPYTER NOTEBOOK VISUALIZATIONS (DASHBOARD):

We also developed interactive UI, where the user can narrow down the by entering more details to narrow down the analysis.
For instance, 
•	Get top 10 zip codes with highest crime rate.
•	Enter desired zip code – to get top crime types
•	Enter desired crime type – to get the occurrence by time


![Dashboard-1](https://github.com/ddhaval04/Smart-City/raw/master/images/dashboard-1.png)


![Dashboard-2](https://github.com/ddhaval04/Smart-City/raw/master/images/dashboard-2.png)


![Dashboard-3](https://github.com/ddhaval04/Smart-City/raw/master/images/dashboard-1.png)