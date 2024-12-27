# Energy-Consumption-Forecasting-for-Non-Residential-Buildings

This project aims to analyze and predict electricity consumption patterns across diverse non-residential buildings using a robust dataset derived from the Building Data Genome Project 2. By leveraging advanced predictive modeling techniques, the project delivers actionable insights that support energy optimization, cost reduction, and sustainability efforts.

**Dataset Description**

Dataset Source: Building Data Genome Project 2
https://www.kaggle.com/datasets/claytonmiller/buildingdatagenomeproject2?select=electricity_cleaned.csv

Key Features:

Scope: Includes hourly electricity consumption (kWh) from non-residential buildings across North America and Europe (2016-2017).

Structure: Columns represent buildings; rows represent hourly timestamps.

Variables:

Electricity consumption (kWh): Target variable.

Time-based attributes: Hourly, daily, and seasonal trends.

Building characteristics: Type, size, and location.

Weather data: Temperature, wind speed, and pressure.

**Pre-Processing Steps**

Metadata Cleaning: Removed redundant columns and aligned building details with electricity consumption data.

Data Transformation: Converted hourly data to daily intervals for ease of prediction.

Outlier Handling: Applied the Interquartile Range (IQR) method to exclude anomalous values.

Feature Engineering: Added lag variables, weekend flags, and time-based attributes.

Missing Value Imputation: Filled predictors with zeros for continuity.

**Exploratory Data Analysis (EDA)**

Seasonality Check: Peaks observed in summer and winter, indicating increased cooling and heating needs.

Correlation Analysis: Strong relationships between electricity consumption and weather attributes such as temperature.

Usage Patterns: Identified inefficiencies during non-operational hours.

**How to Run the Project**

Dependencies: Install Python 3.9+ and required libraries (e.g., pandas, scikit-learn, matplotlib).

Pre-Processing: Ensure data cleaning steps are applied to the raw dataset.

Model Training: Run the provided script to train the Random Forest model.

Visualization: Generate graphs to compare predicted and actual electricity usage.
