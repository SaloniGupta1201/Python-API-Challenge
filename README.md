# Python-API-Challenge

**Submitted By:** Saloni Gupta\
_Date_: november, 5th, 2020\
Python API Homework - **WeatherPy** <br/>

![Equator image](./WeatherPy/Images/equatorsign.png)

## Purpose </br>
The purpose of this project was to see how weather of 500+ unique (non-repeat) cities across the world of varying distance from the equator changes with latitude using CitiPy, a simple Python library was used to find the nearest city to each randomly generated coordinate pair and perform a weather check on each of the cities using a series of successive API calls.The OpenWeatherMap API was then used to find the current temperature, humidity, cloud cover, and wind speed for each city.  </br>

The script accomplishes the following: </br>
1) Randomly selects at least 500 unique (non-repeat) cities based on latitude and longitude. </br>
2) Includes a print log of each city as it's being processed with the city name. </br>
3) Saved both a CSV of all data retrieved and png images for each scatter plot. </br>

The visualizations include a series of scatter plots to showcase the following relationships: </br>
Temperature (F) vs. Latitude | Humidity (%) vs. Latitude | Cloudiness (%) vs. Latitude | Wind Speed (mph) vs. Latitude </br>

Each of these parameters was plotted against the cities latitude to see how temperature varies with distance from the equator. 1500 random coordinate pairs were used to find over 500 cities to perform this analyses. The data and visualizations from this analysis can be found on this site. Click on any of the images in Images folder above to see more analysis. </br>

## Requirements
This notebook requires python to be installed. Python 3.8.3 was used during development. The pandas library used to store, manipulate, filter, merge and perform calculations with the data. The matplotlib and numpy libraries were used to generate the plots showing the trends of various parameters versus latitude. The citipy library was used to get the coordinate pairs used to call openweathermap api. The requests library was used to make the actual calls to the openweathermap api. The jupyter library was used to execute the python code and display results. </br>

We also need to create a api_keys.py file containing api keys for openweatherapi. </br>

## Running the Code
To run the notebook enter the following into the command line: $ jupyter notebook Open up the WeatherPy.ipynb notebook in your browser and then click the 'Kernel' and the 'Restart and run all option' </br>

## Results </br>
After performing the API call from OpenWeatherMap API the following Cities data was retrieved and dataframe was created: </br>
![DataRetrieval image](./WeatherPy/Images/Data_Retrieval.PNG)
![DataFrame image](./WeatherPy/Images/DataFrame.PNG) 

## Scatter ploting </br>
After generating the data a series of scatter plots were created to showcase the following relationships: </br>

### Latitude vs. Temperature Plot </br>
![Temperature image](./WeatherPy/Images/Temperature in World Cities.png) 

The above scatter plot showcase the relationship between Latitude at x-axis vs Max Temperature (F) at the y-axis. This result indicates that there is a higher temperature for cities that found near to the equater (Latitude 0),however when you go farther from the equator towards to the north and south the temprature will decrease. </br>

### Humidity (%) vs. Latitude </br>
![Humidity image](./WeatherPy/Images/Humidity in World Cities.png) 

The above scatter plot displayed the relationship between Humidity (%) vs. Latitude. From this result we can infer that humidity is fairly distributed troughout the plot, so we can say that high humidity occer for both cities found farther or near to the equator. </br>

### Cloudiness (%) vs. Latitude </br>
![Cloudiness image](./WeatherPy/Images/Cloudiness In World Cities.png) 

The above scatter plot showed that the relationship between the cities cloudness, and latitude. From this result we can tell that the data is evenly distributed, and there is no difference in Cloudiness when the cities farther or nearer to the equater(Latitude 0) </br>

### Wind Speed (mph) vs. Latitude </br>
![WindSpeed image](./WeatherPy/Images/Wind Speed In World Cities.png) 

The above scatter plot showed the relationship between wind speed (mph), and latitude. The plot displayed the lower wind speed when the cities closer to the equater (latitude 0) and somehow the wind speed increase for the cities farther from the equater.
