# Final Project: Ideation and High-Level Description

## Overall Motivation
For my final project, I chose two topics related to energy consumption. After graduation, I will be working for a company in the energy sector, so I see this as an excellent opportunity to familiarize myself with industry data while applying practical machine learning techniques. The energy sector offers many powerful applications for machine learning, making it an ideal area to explore.

## Idea 1: Energy Theft Detection

### 1. Summary

The first idea focuses on building a model to detect energy theft, a significant challenge in the energy sector. There is an existing dataset well-suited for developing a model to address this problem.

My approach will involve using supervised classification algorithms such as logistic regression and decision trees. Additionally, I may explore combining these with unsupervised clustering methods to improve accuracy. The primary goal is to develop a model with robust predictive performance while maintaining interpretability and ease of understanding for human stakeholders.

The project will be structured in the following stages:
1. **Data Exploration**
2. **Data Cleansing**
3. **Algorithm Selection and Feature Engineering**
4. **Model Development**
5. **Model Evaluation and Validation**

### 2. About Dataset

#### Dataset Name
[Electricity Theft Detection Dataset](https://data.mendeley.com/datasets/c3c7329tjj/3)

#### Dataset Overview
The dataset contains hourly energy consumption for 16 different types of consumers. The data includes several energy consumption measurements for several customers for one year (12 months).

#### The Number of Records
560,655 (35,040 per customer type)

#### Qualitative Variables
-   **Consumer Type:** Category of consumer (e.g., FullServiceRestaurant, MidriseApartment, SuperMarket).
-   **Theft Label:** Indicator of normal usage or type of theft (theft1 through theft6).

#### Quantitative Variables

1.  `Electricity:Facility [kW] (Hourly)`: Total facility electricity consumption per hour.
2.  `Fans:Electricity [kW] (Hourly)`: Electricity used by fans per hour.
3.  `Cooling:Electricity [kW] (Hourly)`: Energy consumed by cooling systems hourly.
4.  `Heating:Electricity [kW] (Hourly)`: Electricity used for heating systems per hour.
5.  `InteriorLights:Electricity [kW] (Hourly)`: Power used by interior lighting hourly.
6.  `InteriorEquipment:Electricity [kW] (Hourly)`: Electricity consumed by interior equipment hourly.
7.  `Gas:Facility [kW] (Hourly)`: Total gas consumption at the facility per hour.
8.  `Heating:Gas [kW] (Hourly)`: Gas used for heating systems per hour.
9.  `InteriorEquipment:Gas [kW] (Hourly)`: Gas consumed by interior equipment hourly.
10. `WaterHeater:WaterSystems:Gas [kW] (Hourly)`: Gas used by water heating systems hourly.


## Idea 2: Electricity Consumption Forecasting using Regression

### 1. Summary
The second idea centers on building a forecast model using hourly electricity consumption data for London households. The main goal is to create a predictive model capable of forecasting hourly household electricity demand based on historical consumption patterns and hourly weather conditions. The final output would be a description of the algorithm along with an app visualizing the forecasted energy consumption and corresponding energy rates for today and the upcoming week in London.

My approach will involve regression algorithms such as Random Forest Regression and Linear Regression. Depending on evaluation results, I may adjust algorithms or combine multiple approaches.

The project will follow these steps:
1.  **Data Exploration**
2.  **Data Preprocessing and Cleansing**
3.  **Feature Engineering and Algorithm Selection**
4.  **Model Training and Development**
5.  **Evaluation, Validation, and Interpretation of Results**

### 2. About Dataset

#### Dataset Name

[Smart Meter Energy Consumption Data in London](https://www.kaggle.com/datasets/jeanmidev/smart-meters-in-london)

I'm thinking about only using the following two datasets.
- halfhourly_dataset: For energy consumption data
- weather_hourly_darksky.csv: For weather data in London during the period


#### Grain of Data
This dataset has half-hourly energy usage data for individual London households, aligned with corresponding hourly weather observations.

#### The Number of Records
Half-hourly data spanning 5,567 households from November 2011 to February 2014 (approximately 121 million records). The original dataset contains 167 million rows of usage data along with hourly London weather data. Given the dataset's size, I plan to select specific households or periods to manage data processing in my local environment.

#### Qualitative Variables

-   **Time:** Timestamp for the energy consumption or weather data (weather data is hourly).
-   **LC Lid:** Unique identifier for each household (energy data only).
-   **Std or ToU:** Tariff category applied to the household (energy data only).

#### Quantitative Variables

- **Energy consumption data:**
    -   `energy (kWh/hh)`: Electricity consumed per household each half-hour (kWh).

- **Weather data:**
    - `temperature`: Air temperature (°C)
    - `visibility`: Distance of clear visibility (km)
    - `windBearing`: Wind direction (degrees from true north)
    - `dewPoint`: Temperature of air saturation (°C)
    - `pressure`: Atmospheric pressure at sea level (hPa)
    - `apparentTemperature`: Perceived temperature (°C)
    - `windSpeed`: Wind speed (km/h)
    - `precipType`: Type of precipitation
