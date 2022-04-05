# Where Should I Live? **|||** Where Should I Go? 

I use OpenWeather's API to gather weather and location data, then generate a heatmap of the the data and identify areas in the world that match specific climate/weather criteria. Finally, I use Google's geocoding API to find hotels in those locations and plot them on the heatmap.

## Files:
* `WeatherPy.ipynb` - Creates a dataset of cities from randomly generated latitudes and longitudes, pulls weather data on those cities from OpenWeatherAPI and stores it in a dataframe, plots and performs linear regressions on each of the weather variables vs latitude
* `VacationPy.ipynb` - Creates a heatmap of the humidity measurements of data gathered in _WeatherPy_, filters the cities on specific weather criteria, pulls data from Google's API to find hotels near the filtered cities, adds a layer to the heatmap of pins identifying the hotels found on Google
* `Weather_Trends` - Conatins three observations from the data found in the analysis stored in this repiository

## Instructions to recreate the project:
1. Clone this repository to your computer
2. Open the `WeatherPy.ipynb` jupyter notebook and run each cell
3. Open the `VacationPy.ipynb` jupyter notebook and run each cell
