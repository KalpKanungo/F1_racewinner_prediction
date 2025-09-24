# F1 Lap Time Prediction

This project predicts Formula 1 race lap times and potential race winners using historical race data, driver performance metrics, and machine learning models. The goal is to estimate the lap times for each driver in a given race and identify the likely winner.

## Features

- **Driver Performance Metrics**: Clean air pace, qualifying times, wet weather performance factors.
- **Team Performance Metrics**: Team points, historical race performance.
- **Race Data**: Historical lap times for each driver, sector times, and race conditions.
- **Weather Data Integration**: Option to include weather conditions for race-day predictions.

## Technology Stack

- **Python**: Core programming language.
- **FastF1**: To pull historical F1 race and lap data.
- **Pandas & NumPy**: Data manipulation and preprocessing.
- **Scikit-learn**: Data preprocessing, train-test split, metrics.
- **XGBoost**: Gradient boosting model for lap time predictions.
- **Matplotlib & Seaborn**: Data visualization.
- **OpenWeatherMap API**: For fetching weather data (optional).

```bash
git clone https://github.com/yourusername/F1_lap_time_prediction.git
