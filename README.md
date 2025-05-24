# Carbon-Monoxide-prediction
#  Carbon Monoxide (CO) Level Prediction

##  Overview

This project focuses on building a machine learning model to **predict hourly carbon monoxide (CO) levels** based on environmental conditions such as **temperature, humidity, and time-based features**. Elevated CO concentrations are hazardous to public health and industrial safety. By forecasting CO levels, this project supports proactive interventions in both **urban air quality management** and **industrial safety** scenarios.


##  Problem Statement

**Carbon monoxide (CO)** is an invisible and harmful gas produced by incomplete combustion. High concentrations can pose serious health risks. Predicting CO levels helps:

 **Urban authorities** issue air quality alerts
**Industries** protect workers via timely safety measures

> **Objective:** Build a machine learning model that predicts hourly CO concentrations using temperature, humidity, and temporal features (e.g., hour, day, month).



##  Use Case Scenarios

### 1. **Urban Air Quality Monitoring**
Government agencies use CO predictions to alert citizens and reduce exposure to pollution from traffic, industry, and residential heating.

### 2. **Industrial Site Safety Monitoring**
Factories use CO level forecasts to activate ventilation or evacuation protocols, ensuring worker safety.

---

##  Dataset Features

| Feature       | Description                              |
|---------------|------------------------------------------|
| `Temperature` | Ambient temperature in Celsius           |
| `Humidity`    | Relative humidity (%)                    |
| `Hour`        | Hour of the day (0–23)                   |
| `Day`         | Day of the week                          |
| `Month`       | Month (1–12)                             |
| `CO_Level`    | Target variable – concentration of CO (ppm) |

---

##  Model Summary

- **Type:** Regression  
- **Algorithm:** Random Forest Regressor (best-performing model)  
- **Goal:** Predict hourly CO levels with high accuracy



##  Project Workflow

### 1. **Data Preprocessing**
- Parsed time-based features from timestamps
- Handled missing/null values
- Performed feature engineering (e.g., extracting `hour`, `day`, `month`)

### 2. **Exploratory Data Analysis (EDA)**
- Analyzed seasonal trends and correlations
- Visualized CO levels against temperature and humidity

### 3. **Model Building**
- Tested multiple models:
  - Decision Tree Regressor
  - Random Forest Regressor  (best)
- Train-test split and cross-validation
- Hyperparameter tuning for optimization

### 4. **Evaluation Metrics**
- **R² Score:0.9627558650027471
- **MAE / MSE / RMSE**: 2.0436467 / 12.169901819078563 /3.4885
- Residual plots and prediction vs actual comparison


##  Results

- Random Forest model delivered **strong predictive performance**
- Feature importance:
  - **Temperature** and **Hour** were top influencers
- Visual comparison of actual vs predicted CO levels showed strong alignment



