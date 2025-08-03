# 🌦️ Interactive Weather Analytics Dashboard  

![Dashboard Preview](./images/dashboard_preview.png)  

## 📌 Overview  
This project is an **interactive Weather Analytics Dashboard built with Power BI**, designed to provide real-time weather and air quality insights.  
The dashboard integrates **temperature forecasts, air quality indices, and environmental parameters** with an intuitive and modern UI for easy analysis.  

It demonstrates the complete **data analytics workflow** — from data collection and modeling to DAX measures and visualization — making it a strong fit for enterprise analytics use cases.  

---

## 🚀 Features  
- **City Selection**: Filter weather data by location using dynamic slicers.  
- **Current Weather**: Displays real-time temperature, condition, and last updated timestamp.  
- **7-Day Forecast**: Visualizes average daily temperature with min/max tracking.  
- **Air Quality Index (AQI)**:  
  - Dynamic **color-coded indicators** (Green to Maroon).  
  - **Health suggestions** based on AQI levels.  
- **Environmental Factors**:  
  - Humidity, Wind Speed, Visibility, Pressure, UV Index, and Precipitation.  
- **Sunrise & Sunset Times**: For better day planning.  
- **Chance of Rain Forecast**: Daily probabilities for the week ahead.  

---

## 🗂️ Data Model  
![Data Model](./images/data_model.png)  

The dashboard uses a relational model for efficient analysis:  

- **Locations**: Stores city names.  
- **Current**: Real-time weather conditions and air quality metrics.  
- **Forecast_Day**: 7-day forecast data.  
- **Forecast_Hour**: Hourly weather breakdown for advanced insights.  
- **_Measures**: Contains custom DAX measures for KPIs and visualizations.  

---

## 🧮 Key Measures (DAX)  
- `Curr_Temp_C` → Displays current temperature in °C.  
- `Last_Update_Date_Curr` → Shows last updated timestamp using `FIRSTNONBLANK`.  
- `Avg_Temp_Day` → Calculates average forecasted daily temperature.  
- `PM10 Color` → Returns hex color code based on AQI.  
- `AQI Suggestion` → Provides health recommendations based on AQI levels.  
- Additional measures for pollutants: CO, SO2, NO2, O3, PM2.5.  

---

## 🔧 Prerequisites  
- **Power BI Desktop** (latest version recommended).  
- **Weather dataset** from API (e.g., OpenWeather) or pre-collected CSV/JSON files.  
- Internet connection if using live API integration.  

---

## ▶️ How to Use  
1. Clone or download this repository.  
2. Place your **data files/API connection** in the specified path.  
3. Open the `.pbix` file in **Power BI Desktop**.  
4. Select a **city** from the slicer to update the dashboard dynamically.  
5. Explore:  
   - Hover over charts for detailed tooltips.  
   - View AQI colors and corresponding health suggestions.  
   - Track upcoming forecast trends.  

---

## 📸 Screenshots  

### Dashboard View  
![Dashboard View](./images/dashboard_preview.png)  

### Data Model  
![Data Model](./images/data_model.png)  

---

## 📘 Key Learnings  
- Data modeling with **relationships in Power BI**.  
- Writing **custom DAX measures** for calculated KPIs.  
- Implementing **dynamic color coding** with SWITCH and SELECTEDVALUE.  
- Designing **intuitive dashboards** with slicers and KPI cards.  
- Combining multiple data sources (Current, Daily Forecast, Hourly Forecast).  

---

## 🏆 Acknowledgment  
This project builds upon the skills gained from the **Cisco Data Analytics Certification** (Networking Academy), integrating hands-on experience with tools like **Excel, Power BI, Tableau, and SQL** for better analytics and visualization.

---
