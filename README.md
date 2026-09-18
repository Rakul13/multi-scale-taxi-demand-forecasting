# Multi-Scale Taxi Demand Forecasting Using GeoAI

MSc Artificial Intelligence and Data Science research project investigating
short-term taxi-demand forecasting at two spatial levels: Origin-Destination
(OD) pairs and pickup zones in Manhattan, New York City.

## Objective

The project investigates how the spatial representation of taxi demand
affects forecasting performance.

## Dataset

NYC TLC Yellow Taxi Trip Records – January 2024.

- Raw trips: 2,964,624
- Cleaned trips: 2,891,287
- Manhattan OD pairs: 2,418
- Manhattan pickup zones: 64
- Forecast horizon: 1 hour

## Models

- Persistence baseline
- Random Forest
- LSTM
- GAT-GRU

## Technologies

Python, Pandas, NumPy, Scikit-learn, TensorFlow/Keras, SQL,
Matplotlib, GeoPandas, Jupyter Notebook

## Results

### OD-Level Forecasting
Best model: LSTM

- MAE: 0.7614
- RMSE: 1.4113
- R²: 0.7905
- WMAPE: 56.87%

### Zone-Level Forecasting
Random Forest achieved the lowest MAE and WMAPE:

- MAE: 9.1915
- WMAPE: 16.85%

## Key Finding

Forecasting difficulty changes depending on spatial representation.
OD-level forecasting retains detailed movement information but is highly
sparse, while zone-level aggregation provides a denser demand signal and
improves forecastability.

## Author

Rakul Kulanthasamy Saravana Kumar  
MSc Artificial Intelligence and Data Science  
University of Hull
