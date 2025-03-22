# Final Project: Ideation and High-Level Description

## Overall Motivation
For my final project, I have chosen two topics related to energy consumption. After graduation, I will be working as an analytics engineer for an energy tech company, and I see this as an excellent opportunity to familiarize myself with industry data while applying practical machine learning techniques. The energy sector offers numerous impactful applications for machine learning, making it an ideal area for exploration.

## Idea 1: Energy Theft Detection

### 1. Summary
The first idea focuses on building a model to detect energy theft—a significant challenge in the energy sector with serious economic, safety, and environmental implications. There is an existing dataset well-suited for developing a model to address this issue.

My approach will involve leveraging supervised classification algorithms such as logistic regression and decision trees. Additionally, I may explore combining these with unsupervised clustering methods to enhance accuracy. The primary goal is to develop a model with robust predictive performance while maintaining interpretability and ease of understanding for human stakeholders.

The project will be structured in the following stages:
1. **Data Exploration**
2. **Data Cleansing**
3. **Algorithm Selection and Feature Engineering**
4. **Model Development**
5. **Model Evaluation and Validation**

### 2. About Dataset

#### Dataset Name
[Electricity Theft Detection Dataset](https://data.mendeley.com/datasets/c3c7329tjj/3)

#### Grain of Data
Each record represents a consumer’s electricity usage, recorded month-by-month over a continuous 12-month period.

#### The number of records
560,655

#### Qualitative Variables in the Dataset
- **Consumer Type:** Category of consumer (e.g., FullServiceRestaurant, MidriseApartment, SuperMarket).
- **Theft Label:** Indicator of whether the consumer is normal or theft (theft1 through theft6)

#### Quantitative Variables in the Dataset
1. `Electricity:Facility [kW] (Hourly)`: Total facility electricity consumption per hour.  
2. `Fans:Electricity [kW] (Hourly)`: Electricity used by fans per hour.  
3. `Cooling:Electricity [kW] (Hourly)`: Energy consumed by cooling systems hourly.  
4. `Heating:Electricity [kW] (Hourly)`: Electricity used for heating systems per hour.  
5. `InteriorLights:Electricity [kW] (Hourly)`: Power used by interior lighting hourly.  
6. `InteriorEquipment:Electricity [kW] (Hourly)`: Electricity consumed by interior equipment hourly.  
7. `Gas:Facility [kW] (Hourly)`: Total gas consumption at the facility per hour.  
8. `Heating:Gas [kW] (Hourly)`: Gas used for heating systems per hour.  
9. `InteriorEquipment:Gas [kW] (Hourly)`: Gas consumed by interior equipment hourly.  
10. `WaterHeater:WaterSystems:Gas [kW] (Hourly)`: Gas used by water heating systems hourly.

