Part 1 - Creating a Weather Database:

Imported Libraries: I imported necessary libraries like pandas and numpy to handle data manipulation.

Generated Random Coordinates: Using the numpy library, I generated random sets of latitude and longitude coordinates to represent various cities around the world.

Performed API Calls: I utilized the OpenWeatherMap API to retrieve weather information for each set of coordinates, including temperature, humidity, cloudiness, and wind speed.

Saved Data to CSV: After extracting weather data from the API responses, I saved the data to a CSV file named "cities.csv". This file contains city-related weather information.

Part 2 - VacationPy with Maps and Hotels:

Loaded CSV Files: I imported the pandas library and loaded two CSV files, "cities.csv" and "hotel_data_custom_name.csv", containing city weather data and hotel information respectively.

Created Humidity Heatmap: Using the folium library, I created a world map with circular markers placed at each city's coordinates. The size of these markers corresponds to the humidity level of each city.

Filtered Ideal Weather Conditions: I filtered the city data to identify cities with ideal weather conditions. This involved selecting cities with a maximum temperature between 21°C and 27°C, low wind speed, and no cloudiness.

Constructed Hotel DataFrame: I created a new DataFrame, "hotel_df", to store hotel-related information including city, country, coordinates, and humidity.

Added Hotel Information: I combined the filtered city data with the hotel information from the "hotel_data_custom_name.csv" file, appending the hotel name to the "hotel_df" DataFrame.

Plotted Hotel Map: Using folium, I generated another map displaying markers for hotels in the ideal weather condition cities. Each marker included information such as city name, country, and hotel name.
