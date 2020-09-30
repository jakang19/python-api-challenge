# python-api-challenge

## Background
To use Python requests, APIs, and JSON traversals to definitively answer the question: "What's the weather like as we approach the equator?"

## WeatherPy
This script randomly selects a group of 500+ cities across the world using the Python library citipy and uses the OpenWeatherMap API to create a representative model of weather according to the following relationships:
- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

The data gathered is then split into cities located in the Northern and Southern Hemispheres and linear regression analysis is conducted on the data.

## VacationPy
This script contains code that uses the Google API to generate a heatmap based on the cities listed in `WeatherPy.ipynb` and hotel recommendations near cities that fit the user's ideal weather.

## Submission
This repository contains:
- Jupyter notebook script `WeatherPy.ipynb` with data analysis and observations on the generated plots
  - A CSV located in `Output/weather_df.csv` of all retrieved data
  - Images for all scatter plots in the `Output` folder
- Jupyter notebook script `VacationPy.ipynb`with code generating heatmaps and hotel recommendations
  - A screenshot `hotels_heatmap.png` of the percent humidity heatmap marked with recommended hotels
