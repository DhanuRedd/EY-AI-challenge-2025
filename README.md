# EY AI 2025 Data science challenge :  XG Boost model building

Some important file links:
1. Buildings foot print cleaned data: https://drive.google.com/file/d/14wUbC5S1K32DoLNh82BjvOWu43dUAgza/view?usp=sharing
2. Landsat saved Geotiff file: https://drive.google.com/file/d/1UKlSCU4W6EzxDrWprpMjnSoRyz2ldHoc/view?usp=sharing
3. Sentinel saved Geotiff file: https://drive.google.com/file/d/1o_P9hPkRYiaKAHfW5vNssWY2WJdgUu22/view?usp=sharing

## About the Challenge:

Aligned with the United Nations Sustainable Development Goals and the EY Ripples program, the EY Open Science AI & Data Challenge is an annual competition that gives university students, 
early-career professionals and EY people the opportunity to develop data models using artificial intelligence (AI) and computing technology to create solutions that address critical climate issues, building a more sustainable future for society and the planet.

The 2025 AI & data challenge is focused on a phenomenon known as the urban heat island effect, a situation that occurs due to the high density of buildings and lack of green space and water bodies in urban areas. 
Temperature variations between rural and urban environments can exceed 10-degrees Celsius in some cases and cause significant health-, social- and energy-related issues. Those particularly vulnerable to heat-related problems include young children, older adults, outdoor workers, and low-income populations.

All output from the challenge can help bring cooling relief to vulnerable communities, but entrants with top scores will take home cash prizes and receive an invitation to an exciting awards celebration.

## Problem Statement:

The goal of the challenge is to develop a machine learning model to predict heat island hotspots in an urban location. Additionally, the model should be designed to discern and highlight the key factors that contribute significantly to the development of these hotspots within city environments.

Participants will be given near-surface air temperature data in an index format, which was collected on 24 July 2021 using a ground traverse in the Bronx and Manhattan region of New York City. This dataset constitutes traverse points (latitude and longitude) and their corresponding UHI (Urban Heat Island) index values. 
Participants will use this dataset to build a regression model to predict UHI Index values for a given set of locations.

It is important to understand that the UHI Index at any given location is indicative of the relative temperature difference at that specific point when compared to the city's average temperature. This index serves as a crucial metric for assessing the intensity of heat within different urban zones.

## Data Description

Target Dataset:

Near-surface air temperature data in an index format was collected on 24 July 2021 across the Bronx and Manhattan regions of New York City in the United States. The data was collected in the afternoon between 3:00 pm and 4:00 pm. This dataset includes time stamps, 
traverse points (latitude and longitude) and the corresponding Urban Heat Island (UHI) Index values for 11229 data points. These UHI Index values are the target parameters for your model.

Note: Participants are strictly prohibited from using Longitude and Latitude values as features in building their machine learning models. Submissions that employ longitude and latitude values as model features will be disqualified. These values should only be utilized for understanding the attributes and characteristics of the locations.

Incorporating latitude and longitude data in their raw forms or through any form of manipulation—including multiplication, embedding, or conversion to polar coordinates—as predictive features in your model is strictly prohibited, as it can compromise the adaptability of your model across diverse scenarios. 
This prohibition extends to calculating the distance from a reference point and using it as a feature, which is essentially a transformation of the original geographical coordinates into a new feature form. Submissions that include these types of features will be considered non-compliant and will be disqualified.

## Datasets used for building the model:

1. European sentinel-2 satellite data
2. NASA Landsat optical satellite data
3. Buildings foot print data of Manhattan and Bronx regions

## Other data sets suggested to improve the model predictions:
1. Weather data which includes Temperature, solar radiation, wind direction etc.

## Validation Dataset:

After building the machine learning model, you need to predict the UHI index values on the locations identified in the validation dataset. The template was given in the repository.
Predictions on the validation dataset need to be saved in a CSV file.
