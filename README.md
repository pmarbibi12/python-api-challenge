# python-api-challenge
# by Panfilo Marbibi

WeatherPy/  
- VacationPy.ipynb  
- WeatherPy.ipynb  
- output_data/  
-- Fig1.png  
-- Fig2.png  
-- Fig3.png  
-- Fig4.png  
-- cities.csv  
  
WeatherPy.ipynb -- jupyter notebook   
  - This notebook generates a number of randomly selected geographic coordinates and finds the nearest cities to those coordinates  
  - From the list of cities generated, the code will then gather information from those cities and append them to lists:  
  --- latitude, longitude, max temperature, humidity, cloudiness, wind speed, country, date  
  - if a city is not found, it will skip the city and display "City not found. Skipping..."  
  - The lists are then placed into a dataframe : city_data_df  
  - The dataframe is exported as a csv into the output_data directory: cities.csv  
  - From the dataframe, the notebook will create scatter plots:  
  --- City Latitude vs. Max Temperature  
  --- City Latitude vs. Humidity  
  --- City Latitude vs. Cloudiness  
  --- City Latitude vs. Wind Speed  
  - The notebook then separates the data by hemisphere and creates 2 dataframes : northern_hemi_df , southern_hemi_df  
  - The notebook will use the data to calculate the linear regression for each of the above mentioned plots, separating by north and south hemisphere  
  - Analysis of each pair is included  


VacationPy.ipynb -- jupyter notebook     
  - This notebook takes the csv created by WeatherPy.ipynb to determine the best vacation spots using the user's preferences  
  - humidity_map - geomap with dots where the cities found in cities.csv  
  --- the dots are sized by how humid the city is  
  - ideal_crit - dataframe with the desired Max Temp, Humidity level, and Cloudiness  
  - hotel_df - finds the nearest hotel within 10,000 meters of each of the cities  
  - hotel_map - geomap with dots to the cities that fit within the user's desired parameters  
  --- hovering over the dots now show the nearest hotel from the city along with the city's country  
  
  
  Code used for each notebook came from the activities done in class
