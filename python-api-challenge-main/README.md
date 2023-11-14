In this project contains two scripts. 
First script weather_data_analysis.py generates a set of random cities, fetches weather data for each city using the OpenWeatherMap API, and then creates scatter plots for latitude vs. maximum temperature, humidity, cloudiness, and wind speed. Additionally, it performs linear regression analysis on these relationships for both the Northern and Southern Hemispheres.

The resulting plots are saved in the output_data directory.

Output
The script generates scatter plots in PNG format:
Fig1.png: Latitude vs. Maximum Temperature
Fig2.png: Latitude vs. Humidity
Fig3.png: Latitude vs. Cloudiness
Fig4.png: Latitude vs. Wind Speed
Data Files
The weather data for the cities are saved in output_data/cities.csv.
Second sript python hotel_finder.py reads a CSV file created in a previous step, filters cities based on specific criteria, and then utilizes the Geoapify API to find hotels within a given radius.

The results are displayed on an interactive map, providing details about each city, its country, the nearest hotel, and the humidity level.

Output
The script generates an interactive map of selected cities and another map with identified hotels, saved as map_plot_1.html and map_plot_2.html, respectively.
Data Files
The script requires a CSV file named cities.csv (created in a previous step) to load the city data.
Notes
The hotel search is based on criteria such as maximum temperature, wind speed, and cloudiness.
