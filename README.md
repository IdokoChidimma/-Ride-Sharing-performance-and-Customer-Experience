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
  
### 5. Interactivity with Slicers:
Slicers are implemented for key categorical fields like Day of Week, Ride Status, and Traffic-Level. These slicers are connected to all relevant PivotTables and Pivot Charts on the dashboard, enabling dynamic filtering and cross-sectional analysis.

### 6. Dashboard Assembly:
All calculated KPIs, PivotTables, and Pivot Charts are consolidated onto a single, interactive Excel dashboard sheet, formatted for clarity and ease of use.

## DATA ANALYSIS AND INSIGHTS

- THE KEY PERFORMANCE INDICATORS (KPIs);
To effectively evaluate and optimize the ride performance, several core KPIs were established using excel based calculations:

💰 Total Revenue : $ 600,938

This shows the sum of all rides amount, helping to assess financial performance and the impact of pricing strategies, especially under surge conditions.

🚗 Total Rides completed: 8495

It measures the count of successful rides, serving as a primary indicator of platform usage and reliability.

⭐ Average Customer Rating : 3.73

Reflects customer satisfaction and correlates with driver behavior, traffic level, and ride experience.

⌛ Average Ride Duration (min): 54.03

Indicates the average time spent per trip or Ride, which varies with traffic levels, route, and weather condition. it is necessary for estimating service efficiency and planning improvements.

📈 No-show Rate(%): 5.27%

It captures the rides cancellations or missed pickups, which signal operational inefficiencies or user dissatisfaction.

## ANALYSIS QUESTION AND INSIGHTS

# 1. Customer Behavior & Preferences:-

- What are the most popular pickup and drop-off locations?
  
Top Pickup Points: “Downtown,” “Financial District,” and “University” show consistently high ride starts, hinting at business travelers and students as core user groups.
Drop-Off Diversity: Drop-offs are more spread out than pickups, Financial District, Mall, and Airport showing slightly higher counts. This suggests users often head home or to shopping areas helpful for targeted campaigns or partnerships.

- How do weekend vs weekdays impact ride demand?
  
Analysis of ride data reveals a clear pattern: weekday demand is consistently higher, driven primarily by commuter traffic during morning and evening hours, with Monday recording the peak volume at 4240. In contrast, weekend demand is less predictable, influenced by leisure activities and events, often peaking in the late afternoon and evening.
This trend highlights the need for adaptive driver scheduling and flexible pricing models to optimize operations across different days.

- Which vehicle types (SUV, Sedan, Motorcycle, Electric) are most preferred?
  
Sedans Dominate: 40% of users choose sedans, followed by SUVs (30%), showing clear preferences for comfort and space.
Low Use of Shared, Motorcycle, & Electric Options: Shared, Motorcycle, and Electric vehicles only contribute 10% each, suggesting either limited supply or lower customer trust opportunity areas for education, incentives, or availability improvements.

# 2. Driver Performance & Efficiency:-

- Which drivers have the highest and lowest rating?

Top-Performing Driver: These high-performing drivers reflect a strong commitment to punctuality, professionalism, and customer satisfaction contributing significantly to ride completion and platform reliability.
Low-Performing Driver: Low ratings may stem from issues such as customer complaints, delays, or poor communication. These drivers could be negatively affecting customer retention and overall platform reputation.

# 3. Operational & Financial Insights:-

- Which payment methods are most commonly used?
  
Payment Behavior: Credit Card Dominate: With 4,946 transactions, credit card are the most popular payment mode, showing strong digital adoption. Cash (3,028) and Mobile Wallet (2,026) still play significant roles, suggesting a need to maintain multi-channel payment support.

- How does surge pricing affect fare amount?
 Total Revenue: The platform generated over $600K in total revenue, reflecting strong market demand and operational performance over the analysis period.
Surge Pricing Impact: Approximately $480,566 of this revenue (80%) was earned during periods when surge pricing was active.
In contrast, only $120,372 was generated without surge pricing.

# 4. External Factors:-

- How does weather condition (Rainy, Snowy, Foggy) impact ride duration and customer rating?
  
The bar chart shows that ride duration is highest during thunderstorms (56 mins) and gradually decreases to 53 mins in foggy and snowy weather condition. Meanwhile, the line chart indicates that customer ratings are lowest during thunderstorms (3.66) and peak slightly during rainy weather (3.76). This suggests that longer rides in extreme weather, especially thunderstorms, negatively impact user satisfaction, while moderate weather like rain may be more tolerable.
These delays may be caused by reduced visibility, cautious driving, and slower traffic flow.

- What is the effect of traffic level (Low, Medium, High) on ride fare amount?
  
The platform recorded the highest revenue of $302,046 during medium traffic, indicating an ideal balance between trip frequency and duration without delays. Under low traffic conditions, revenue reached $179,850 suggesting faster rides but lower demand or shorter trip distances. High traffic, despite increasing per-trip fares due to longer durations, resulted in the lowest total revenue $119,043 likely due to fewer completed rides and increased delays.
Insight: Medium traffic offers the sweet spot for operational efficiency, while high traffic reduces volume, and low traffic may reflect off-peak demand.

## 💡 RECOMMENDATION:

📌 Deploy more drivers in high -demand zones (eg, downtown, Financial districts) during peak hours. Use location heatmaps to dynamically adjust driver positioning and reduce rider wait time.

📌Adjust driver scheduling to match high-demand weekday commute periods, and boost driver presence during weekend evenings when demand is more event-driven.

📌 Expand the sedan and SUV fleet to match customer preferences. Encourage the use of less-utilized vehicle types, such as electric and shared rides, by offering promotional discounts or launching eco-friendly ride campaigns to support sustainability goals.
📌 Recognize and reward top-rated drivers through bonuses or performance programs. For low-rated drivers, implement mentorship by top performers, and monitor improvement through regular reviews.

📌Surge pricing should be used during peak periods to maximize revenue, but must be communicated to riders. Transparent pricing builds trust and prevents user dissatisfaction.

📌 Strengthen supports for digital payments ( Mobile wallet and cards) as they dominate usage. Promote cashless incentives and ensure seamless processing to improve customer experience and financial tracking.

📌 Alerts user and drivers in advance during poor weather. Provide real-time updates on delays and consider offering fare reduction during extreme conditions to preserve satisfaction.

📌 If a trip takes longer because of heavy traffic, adjusting the fare makes pricing fair for both the rider and the driver, keeping everyone satisfied.

## 🛠 TOOLS USED
- Microsoft Excel
- PivotTables and Charts
  


## 🧠 CONCLUSION
In conclusion, this Excel-based dashboard effectively provides a comprehensive view of the ride-sharing platform’s performance and customer experience. By centralizing key metrics and interactive visualizations, it empowers stakeholders to quickly identify operational trends, assess the impact of various factors, and understand customer behavior. This data-driven approach is crucial for optimizing driver efficiency and enhancing overall customer satisfaction.






