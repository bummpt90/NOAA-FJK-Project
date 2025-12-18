# JFK Airport Precipitation Analysis & Forecasting
### US Weather Forecast Firm - Data Science Project

![RStudio](https://img.shields.io/badge/RStudio-4285F4?style=for-the-badge&logo=rstudio&logoColor=white)
![Tidyverse](https://img.shields.io/badge/Tidyverse-blue?style=for-the-badge)

## 🌦️ Project Overview
This project simulates the role of a Data Scientist at a US Weather forecast firm. The objective is to analyze historical climatological data from **JFK International Airport (Queens, NY)** and develop a predictive model for daily precipitation.

### Business Questions
* What are the primary historical drivers of precipitation at JFK?
* How accurately can we predict rainfall using local variables like Humidity, Pressure, and Wind Speed?
* Which meteorological factors have the strongest correlation with rainy days?

## 📊 Dataset Description
The data originates from the **NOAA National Centers for Environmental Information**. It includes daily observations of:
* **Temperature** (Dry Bulb)
* **Humidity** (Relative)
* **Wind Speed**
* **Station Pressure**
* **Dew Point**
* **Precipitation** (Target Variable)

## 🛠️ Data Pipeline (7-Step Workflow)
1. **Data Ingestion:** Imported raw NOAA CSV files into R Studio.
2. **Data Wrangling:** Handled "Trace" (T) values by converting them to 0 and cleaned missing entries.
3. **EDA:** Conducted descriptive statistics and visualized relationships using `ggplot2`.
4. **Modeling:** Developed a **Multiple Linear Regression** model.
5. **Prediction:** Tested the model on "unseen" historical data to simulate real-world forecasting.
6. **Visual Assessment:** Used Correlation Heatmaps to single out the best predictors.
7. **Numerical Assessment:** Evaluated performance using **MSE** and **RMSE**.

## 📈 Key Findings
* **Strongest Predictor:** Average Relative Humidity showed a significant positive correlation (0.41) with precipitation.
* **Barometric Influence:** Air Pressure showed a negative correlation (-0.21), confirming that falling pressure is a reliable indicator of incoming rain.
* **Model Accuracy:** * **RMSE:** 0.2206 (On average, predictions are off by ~0.22 inches).

  
  * **R-Squared:** 0.261 (The model explains 26% of the precipitation variance).

