# 🚕 NYC Uber Ride Data Analysis

A comprehensive data analysis project that explores NYC Uber ride data to uncover temporal patterns, geographic hotspots, fare distributions, and ride behaviors using data cleaned on Kaggle and visualized in Power BI.

---

## 👤 Owner Information

-  ISHIMWE Prince Cuthbert  
- ID: 27089  

---

## 📖 About the Project

This project analyzes NYC Uber trip records to understand ride demand fluctuations across time and geography, fare amount distributions, and ride durations. Leveraging Power BI’s visualization and Kaggle for initial data cleaning, the goal is to provide actionable insights for Uber’s operational improvements and strategic planning.

### Project Objectives

- Identify hourly, daily, and monthly ride patterns  
- Map pickup and dropoff hotspots  
- Analyze fare and trip distance distributions  
- Detect peak and off-peak periods  
- Generate recommendations based on data insights

---

## 🛠 Built With

### Tech Stack

- **Data Cleaning:** Kaggle Python environment (Pandas, NumPy)  
- **Visualization & Analysis:** Microsoft Power BI Desktop  

### Key Features

- Time series visualizations (line charts, bar charts)  
- Geographic heatmaps and cluster maps  
- Histogram and box plot fare analysis  
- Interactive dashboards with slicers and drill-downs  

---

## Methodology: Data Collection and Analysis Approach

The dataset was sourced from Kaggle, containing detailed NYC Uber trip records. Initial data cleaning and preprocessing—such as handling missing values, converting timestamps, and feature engineering (e.g., extracting hour, day, month)—were performed using Python (Pandas). The enhanced dataset was imported into Power BI for exploratory data analysis and visualization. Key insights were derived through time-series charts, geographic heatmaps, histograms, and clustering. Custom DAX measures and slicers were implemented to enable dynamic, interactive dashboard filtering.


## 📊 Dataset Structure

| Column            | Type           | Description                                  |
|-------------------|----------------|----------------------------------------------|
| pickup_datetime   | datetime       | Date and time when the trip started          |
| pickup_latitude   | float          | Latitude coordinate of pickup location       |
| pickup_longitude  | float          | Longitude coordinate of pickup location      |
| dropoff_latitude  | float          | Latitude coordinate of dropoff location      |
| dropoff_longitude | float          | Longitude coordinate of dropoff location     |
| fare_amount      | float          | Fare charged for the trip                      |
| trip_distance    | float          | Distance traveled during the trip (miles)    |
| passenger_count  | int            | Number of passengers during the trip          |
| day_of_week      | string         | Day name extracted from pickup_datetime       |
| week_category    | string         | Categorized day group (Early Week, Mid Week, Weekend) |
| hour             | int            | Hour of day extracted from pickup_datetime    |
| manual_peak      | string         | Manually categorized peak/off-peak hours      |

---
## 🔍 3. Analysis: Key Visualizations and Statistical Insights

### 🕒 A. Time-Based Ride Analysis
- **Hourly Trends:** Rides peak during 8–10 AM and 5–7 PM (commute hours).  
- **Day of Week Patterns:** Mid-week (Wednesday and Thursday) has the highest ride frequency.  
- **Monthly Distribution:** May shows the highest ride volume, possibly due to seasonal demand.  

### 📍 B. Geographic Ride Distribution
- **Pickup Heatmap:**  
  Created using `pickup_latitude` and `pickup_longitude`.  
  Used `trip_distance` as bubble size.  
  Identified hotspots in Manhattan and Brooklyn.

- **Dropoff Clusters:**  
  Used `dropoff_latitude` and `dropoff_longitude`.  
  Applied cluster visualization by drop count.  
  Noted dense activity in NYC business districts.

### 💵 C. Fare and Trip Distance Analysis
- **Histogram:**  
  Most common fare falls within the \$4–\$5 range (91,618 rides).  
  Very few high fares above \$100 (e.g., a fare of \$494.74 occurred only once).

- **Distance vs Fare:**  
  Positive linear trend showing higher distance correlates with higher fare.  
  Short trips with high fares identified as anomalies.

### ⏱ D. Ride Duration (Estimated)
- Calculated using:
- *Note:* Since only `pickup_datetime` was available, this analysis was either skipped or adjusted accordingly.

---

## 📌 4. Results: Key Discoveries
- **Rider Activity:** Highest on weekdays, especially Wednesdays.  
- **Peak Hours:** Align with typical work commute windows.  
- **High Demand Zones:** Concentrated in Manhattan core for both pickups and dropoffs.  
- **Most Rides:** Generally within short distances (under 2 miles).  
- **Fare Outliers:** Few rides were priced abnormally high despite short distances.

---

## ✅ 5. Conclusion: Summary
The dataset reveals consistent temporal patterns and geographic clustering in NYC Uber ride activity. Fare pricing closely aligns with trip distance, and peak hours support the expected commuter behavior. Data outliers were successfully identified and handled through Kaggle-based preprocessing.

---

## 💡 6. Recommendations
- Uber should optimize driver availability during peak mid-week and rush-hour windows.  
- Consider revising dynamic pricing to address short rides with disproportionately high fares.  
- Promote rides in underserved zones via location-based discounts and incentives.  
- Leverage ride duration and distance data to improve route prediction and fare transparency.


---

## 💾 Setup & Installation

### Prerequisites

- Power BI Desktop (free download from Microsoft)  
- Kaggle account or environment to run Python for cleaning  

### Links part

- GitHub Repository and cleaned data in google drive

```bash
https://github.com/PrinceCuthbert/NYC-Uber-Ride-Data-Analysis

```

```bash
https://docs.google.com/spreadsheets/d/1PJDPRu6pbmM3CRJKHau_T00qd9Ta4lkBs6LcsX9ivYo/edit?gid=406967966#gid=406967966

