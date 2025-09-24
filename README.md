F1 Race Lap Time Prediction
Overview

This project predicts Formula 1 race outcomes by modeling lap times of drivers based on historical data, driver performance metrics, and team statistics. Using machine learning techniques, the model estimates each driver's predicted lap time and the total race time, helping to forecast the likely race winner.

The dataset includes lap times from the 2024 season, driver-specific metrics like qualifying performance, clean air pace, wet-weather skill, and team performance scores.

Features Used
Feature	Description
QualifyingTime	Driver's qualifying lap time at the race circuit
team_performance_score	Team's historical performance metric
CleanAirPace	Driver's pace in free air without traffic
drive_wet_perf	Driver's wet-weather performance factor
team_points	Team championship points prior to the race
Target Variable

LapTime: Average lap time of a driver for the race (converted to seconds for modeling)

Predicted lap times are converted to total race times by multiplying with the number of laps at the circuit.

Approach

Data Collection

Lap times fetched from the FastF1 API

Weather and track data fetched from OpenWeatherMap API

Data Preprocessing

Missing values handled using median imputation

Timedelta lap times converted to seconds

Modeling

XGBoost Regressor is used to predict lap times per driver

Hyperparameter tuning performed using cross-validation for optimal performance

Predicted lap times are multiplied by total race laps to get full race time

Evaluation

Performance metric: Mean Absolute Error (MAE)

Typical MAE: ~0.44 seconds per lap