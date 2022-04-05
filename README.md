# Where Should I Live? **|||** Where Should I Go? 

I use OpenWeather's API to gather weather and location data, then perform exploratory analysis and generate regressions on various weather variables to identify correlations with the latitude of the cities in the dataset. I narrowed down my list of observations of the data to the following insights:
1. The strongest correlation is between latitude and max temperature of cities in the northern hemisphere.
2. Since the r-value is positive when comparing latitude and max temperature of cities in the southern hemisphere, this suggests that as we move closer to the equator (latitude increases) the max temperature will most likely increase.
3. The weakest correlation is between latitude and wind speed of cities in the northern hemisphere.

After running this analysis, I then generate a heatmap using humidity data and identify areas in the world that match specific climate/weather criteria. 

![image](https://user-images.githubusercontent.com/87830922/161860954-d756f921-145f-4508-a55e-6d40f1fad5cd.png)

Finally, I then use Google's geocoding API to find hotels within 50 miles of the narrowed down locations (if they exist) and plot them on the heatmap.

![image](https://user-images.githubusercontent.com/87830922/161861614-8c793fc1-ea2d-4285-8c78-135a629887da.png)

## Files:
* `WeatherPy.ipynb` - Creates a dataset of cities from randomly generated latitudes and longitudes, pulls weather data on those cities from OpenWeatherAPI and stores it in a dataframe, plots and performs linear regressions on each of the weather variables vs latitude
* `VacationPy.ipynb` - Creates a heatmap of the humidity measurements of data gathered in _WeatherPy_, filters the cities on specific weather criteria, pulls data from Google's API to find hotels near the filtered cities, adds a layer to the heatmap of pins identifying the hotels found on Google
* `Weather_Trends` - Conatins three observations from the data found in the analysis stored in this repiository

## Instructions to recreate the project:
1. Clone this repository to your computer
2. Open the `WeatherPy.ipynb` jupyter notebook and run each cell
3. Open the `VacationPy.ipynb` jupyter notebook and run each cell
