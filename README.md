# Python-API-Analysis

Greetings,

Welcome to the Python-API-Analysis repository! This project utilizes Python and specifically levarages Matplotlib, Pandas, Numpy, Requests, ScipyStats, Hvplot, and CitiPy libraries to demonstrate API proficiency. The first part of the analysis ("WeatherPy.ipynb"), generates a randomized list of cities and subsequently initiates a get request that calls on the "OpenWeatherMap" API to retrieve specific city attributes such as latitude, longitude, maximum temperature, humidity, cloudiness metric, wind metric, etc. After parsing the JSON payload and enriching the original city DataFrame, scatter plots were generated to visualize the relationship between weather variables and latitude to showcase how weather changes for geographies that are closer to the equator. Furthermore, bivariate linear regression equations were calculated and described for each of these relationships within both the northen and southern hemispheres (Latitude vs. Temperature, Latitude vs. Humidity, Latitude vs. Cloudiness and Latitude vs. Wind Speed).

The second part of this analysis ("VacationPy.ipynb"), imports the generated and enriched city data created in part one and creates map visualizations thereafter. The initial plot shows the location of all cities in the dataset represented by a point sized indicatively of the city's relative humidity. The next and final visualization maps cities that have been filtered to only include locations defined by "ideal" weather conditions (Max temperature between 27 and 21 degrees Celsius, wind speed less than 4.5 m/s and 0 cloudiness). This plot also includes hover columns that shows the first hotel located within 10,000 meters of each ideal city - hotel data was retrieved via the "Geoapify" API.

**Repository Structure:**

  - 'WeatherPy' directory:
    
    -  'output_data' directory - contains generated cities CSV dataset and scatter plots depicting the impact latitude has on weather variables
    -  "WeatherPy.ipynb" - Executed code for part 1
    -  "VacationPy.ipynb" - Executed code for part 2

Thanks!
