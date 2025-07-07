# 🚗 Ride Sharing Performance and Customer Experience
![Ride Dashboard](https://github.com/user-attachments/assets/a006e2f0-109d-4463-a6f4-128f66bb3ac4)
## 📌INTRODUCTION
As a leading ride-sharing platform, the core objective is to enhance ride efficiency, optimize pricing strategies, and most importantly enhance and improve customer satisfaction. By thoroughly analyzing ride data, the aim is to uncover key insights into user behavior, driver performance, and existing operational bottlenecks. This approach enables the platform to make data-driven decisions which helps in growth and efficiency.
## ❓ PROBLEM STATEMENTS
This analysis address several business question based on the dataset provided;
### 1. Customer Behavior & Preferences:-
- What are the most popular pickup and drop-off locations?
- How do weekend vs weekdays impact ride demand?
- Which vehicle types (SUV, Sedan, Motorcycle, Electric) are most preferred?
  
### 2. Driver Performance & Efficiency:-
- Which drivers have the highest and lowest rating?
  
### 3. Operational & Financial Insights:-
- Which payment methods are most commonly used?
- What is the average fare amount per ride types?
- How does surge pricing affect fare amount?
  
### 4.External Factors:-
- How does weather condition (Rainy, Snowy, Foggy) impact ride duration and customer rating?
- What is the effect of traffic level (Low, Medium, High) on ride fare amount?
  
## 🎯 OBJECTIVE
The primary objective is to create an interactive excel-based dashboard that enable stakeholders to easily identify trends, optimize driver efficiency, and improve customer satisfaction. This will facilitate better decision making and lead to swift operation and improvement within the ride sharing platform.

## 📁 DATASET DESCRIPTION
The dataset used for this analysis is provided in the file Rise Sharing Data Table.csv. it contains detailed records of ride activity on a ride-sharing platform, which covers a range of important features, including: Ride_ID, User_ID,	Driver_ID,	Ride_DateTime, Day of Week,	Hour of the Day,	Pickup_Location,	Dropoff_Location,	Distance_km,	Ride_Duration_min,	Fare_Amount,	Payment_Method,	Ride_Status,	User_Rating,	Driver_Rating,	Surge_Pricing,	Promo_Code_Used	Vehicle_Type,	Weather_Condition,	Traffic_Level,	Driver_Experience_Years,	User_Type.

## 🔧 METHODOLOGY

### 1. DATA CLEANING AND PREPARATION: The raw data is loaded into excel. Essential columns are created, such as ‘Day of Week’ (using TEXT() function), ‘Hour of Day’ (using HOUR() function), to facilitate time-based analysis. Data parsing with “Text to Columns” is applied to ensure correct interpretation of date/time fields.

### 2. Data Types: All the data contained in the tables was properly checked and verify to ensure correct data type. This helps to ensure an error-free analyses and calculations.

### 3. Key Metrics & KPIs calculation: Core performance indicators like Total Revenue(SUM of Fare Amount), Total Rides completed, Average Customer Rating, Average Ride duration(Min), and No-Show Rate(%) are calculated. For dynamic KPIs like No-Show Rate that respond to filters, values are derived from two interconnected PivotTables.

### 4. Data Visualization(PivotTables & Charts):

- PivotTables: it was created for various aggregations such as rides count by days of the week, counts by pickup/drop-off locations, Ride-type distribution, Ride Orders By Weather Type, Fare Amount Distribution With Surge Pricing, Payment Type, Fare Amount vs Traffic Levels. Manual sorting and filters is applied where specific order is required, for instance, Pickup & Drop-off locations:(Filtered Top 10 locations), Traffic Level:(sorted Low, Medium, High).
- Pivot Charts: Bar and Columns charts are used for pickup/drop-off locations, Fare Amount vs Traffic Level. Line chart for Ride Demand By Days Of The Week, A pie chart visualizes ride type distribution, and Payment Type, Donut chart for Fare Amount Distribution With Surge Pricing, Combo for User Rating by Weather Condition & Duration.
  
### 5. Interactivity with Slicers: Slicers are implemented for key categorical fields like Day of Week, Ride Status, and Traffic-Level. These slicers are connected to all relevant PivotTables and Pivot Charts on the dashboard, enabling dynamic filtering and cross-sectional analysis.

### 6. Dashboard Assembly: All calculated KPIs, PivotTables, and Pivot Charts are consolidated onto a single, interactive Excel dashboard sheet, formatted for clarity and ease of use.

## DATA ANALYSIS AND INSIGHTS

- THE KEY PERFORMANCE INDICATORS (KPIs);
To effectively evaluate and optimize the ride performance, several core KPIs were established using excel based calculations:

![image](https://github.com/user-attachments/assets/39cc3e42-12fa-4e01-8d3d-5c7adb9e98d6) Total Revenue : $ 600,938
This shows the sum of all rides amount, helping to assess financial performance and the impact of pricing strategies, especially under surge conditions.

![image](https://github.com/user-attachments/assets/8e8be886-c263-4ad9-b5f6-e64ee6164b94) Total Rides completed: 8495
It measures the count of successful rides, serving as a primary indicator of platform usage and reliability.

![image](https://github.com/user-attachments/assets/9f6ee6cd-6bcd-4a1e-948e-be88d6dc9ca3) Average Customer Rating : 3.73
Reflects customer satisfaction and correlates with driver behavior, traffic level, and ride experience.

![image](https://github.com/user-attachments/assets/7448fd53-bed6-4596-b485-9ed226ac6f1d) Average Ride Duration (min): 54.03
Indicates the average time spent per trip or Ride, which varies with traffic levels, route, and weather condition. it is necessary for estimating service efficiency and planning improvements.

![image](https://github.com/user-attachments/assets/539d1460-0fbb-47e9-a2ac-10381a6b9d8f) No-show Rate(%): 5.27%
It captures the rides cancellations or missed pickups, which signal operational inefficiencies or user dissatisfaction.

## ANALYSIS QUESTION AND INSIGHTS

Customer Behavior & Preferences:-
What are the most popular pickup and drop-off locations?




