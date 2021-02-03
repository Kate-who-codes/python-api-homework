# UCD-SAC-DATA-PT-12-2020-U-C

Background
The Python script was created to visualize the weather of multiple  cities across the world of varying distance from the equator

To run the code:
Install citypy in your python environment (https://pypi.python.org/pypi/citipy)
Save OpenWeatherMap API Key (https://openweathermap.org/) as 'weather_api_key'
Google API Key (https://console.developers.google.com/getting-started) as 'g_key'
Create API Keys and store it in the 'api_keys.py' file before running the Jupyter notebooks.


Part I - WeatherPy
Python script was written to to visualize the weather of cities across the world of varying distance from the equator. To complete this, I used  Python library and OpenWeatherMap API, gkey.


Observation
Southern Hemisphere climates tend to be slightly milder than those at similar latitudes in the Northern Hemisphere. This is because the Southern Hemisphere has significantly more ocean and much less land; water heats up and cools down more slowly than land.

Highest temperature is found at 0 latitude and as the latidude increases or decreases, temperature drops. This happens as equatorial region receives sunlight straight with less or no angle due to curvature shape of earth.

Latitude doesn't have a strong iinfluence on wind speed. The speed of the wind is controlled by the strength of the air pressure gradient, the stronger the pressure gradient the higher the wind speed. 

Objectives
Objective 1

Temperature: Highest temperature is found at 0 latitude and as the latidude increases or decreases, temperature drops.

Humidity: Polar regions have lower humidity and as latitude gets higher,humidity gets higher in southern hemisphere.

Cloudiness: Cloudiness data is widely spread across the latitude.

Wind: Wind speed data is widely spread across the latitude.


Objective2: is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude)

The r-squared is : -0.83 There is a strong negative correlation between latitude and max temperature for northern hemisphere.

Southern Hemisphere - Temperature (F) vs. Latitude :The r-squared is : 0.46 There is a moderate positive correlation between latitude and max temperature for southern hemisphere.

Northern Hemisphere - Humidity (%) vs. Latitude : The r-squared is : 0.47 There is a moderate positive correlation between latitude and humidity for northern hemisphere.

Southern Hemisphere - Humidity (%) vs. Latitude :The r-squared is : 0.29 There is a moderate positive correlation between latitude and humidity for southern hemisphere.

Northern Hemisphere - Cloudiness (%) vs. Latitude: The r-squared is : 0.23 There is a weak positive correlation between latitude and cloudiness for northern hemisphere.

Southern Hemisphere - Cloudiness (%) vs. Latitude: The r-squared is : 0.08 There is a weak positive correlation between latitude and cloudiness for southern hemisphere.

Northern Hemisphere - Wind Speed (mph) vs. Latitude: The r-squared is : 0.1 There is a weak positive correlation between latitude and windspeed for northern hemisphere.

Southern Hemisphere - Wind Speed (mph) vs. Latitude: The r-squared is : -0.24 There is a weak negative correlation between latitude and wind speed for southern hemisphere.



Part II - VacationPy
Create a heat map that displays the humidity for every city from the part I of the project.

Narrow down the DataFrame to find my ideal weather condition. For example:

A max temperature lower than 80 degrees but higher than 70.
Wind speed less than 10 mph.
Zero cloudiness.
Drop any rows that don't contain all three conditions.



