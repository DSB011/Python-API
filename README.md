# Python API - What's the Weather Like?

## Overview:
Whether financial, political, or social -- data's true power lies in its ability to answer "What's the weather like as we approach the equator?"

## Part I - WeatherPy:

Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. Utilized a Python library, the OpenWeatherMap API, to create a representative model of weather across world cities.
Created a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Fig1.png"> 
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Fig2.png"> 
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Fig3.png"> 
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Fig4.png"> <br><br>

For the second requirement did a linear regression on each relationship, only this time separating them into 
Northern Hemisphere (greater than or equal to 0 degrees latitude) 
and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude <br><br>

<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Northern%20Hemisphere%20Latitude%20vs%20Max%20Temp%20on%202020-06-25.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Southern%20Hemisphere%20Latitude%20vs%20Max%20Temp%20on%202020-06-24.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Northern%20Hemisphere%20Latitude%20vs%20Humidity%20on%202020-06-25.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Southern%20Hemisphere%20Latitude%20vs%20Humidity%20on%202020-06-25.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Northern%20Hemisphere%20Latitude%20vs%20Cloudiness%20on%202020-06-25.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Southern%20Hemisphere%20Latitude%20vs%20Cloudiness%20on%202020-06-25.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Northern%20Hemisphere%20Latitude%20vs%20Windspeed%20on%202020-06-25.png">
<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/Southern%20Hemisphere%20Latitude%20vs%20Windspeed%20on%202020-06-25.png"> <br><br>

## Part II - VacationPy:
Used jupyter-gmaps and the Google Places API for this part.<br>
* Created a heat map that displays the humidity for every city from the part I.
* Narrow down the DataFrame to find the ideal weather condition. 
    * A max temperature lower than 80 degrees but higher than 70.
    * Wind speed less than 10 mph.
    * Zero cloudiness.
* Used Google Places API to find the first hotel for each city located within 5000 meters of the coordinates.
* Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.<br>

<img src = "https://github.com/DSB011/Python-API/blob/master/output_data%20/hotel_map.png"> <br>

## Tech Environment Used:
Jupyter Notebook, Pandas, Matplotlib, API, Python libraries, Gmaps, Openweather API, Google Places API.

## References:
* [Citipy Python Library](https://pypi.org/project/citipy/)
* [Geographic Co-ordinate System](https://desktop.arcgis.com/en/arcmap/10.3/guide-books/map-projections/about-geographic-coordinate-systems.htm)
* [Open WeatherMap API](https://openweathermap.org/api)

