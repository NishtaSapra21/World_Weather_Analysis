# World Weather Analysis

## __Overview__

This analysis generates a set of random latitudes and longitudes to retrieve the nearest city and retrieve its weather data including weather description using API calls. This weather data is used to set range for max and min temperatures to identify customer’s preferred travel destinations and nearby hotels showing them on a marker layer map with pop-up markers. Also, a travel itinerary showing a route between four cities  chosen form customer’s preferred travel destinations is created  using Google Directions API and marker layer map with pop-up marker for each city.

## __Weather Database__

* Approximately 2000 random latitudes and longitudes have been generated to get nearby cities using “citypy” module. 
* Looping through all the cities to get weather data for each city including city, country, maximum temp, latitude, longitude, percent humidity, percent cloudiness,     wind speed and weather description.
* New DataFrame is created to save this weather data.
* DataFrame is exported as a CSV file.

## __Vacation Search__

* Using CSV file created previously, a new DataFrame  is created according to customer’s maximum and minimum temperature criteria with the help of __Pandas’ loc()__     method.
* After checking and eliminating __NULL__ values, a new DataFrame is created  to store hotel names along with city, country, max temp, and coordinates.
* Get the hotel information by setting parameters to search for hotels with 5000 meters and verify that there must be no NULL for hotels. 
* Using hotel information and their locations, a marker layer map with pop-up markers is displayed using Google map and places  APIs.

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/107717882/181152173-3a53f346-6f67-4576-b0c5-e984c6446b91.png)


## __Vacation Itinerary__

* Using Google Direction API a route map and marker layer map are generated for four cities in the itinerary.

![WeatherPy_travel_map](https://user-images.githubusercontent.com/107717882/181152878-93bbe39f-b066-4bfb-821e-663965714db3.png)


![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/107717882/181152962-8ec4b296-d99d-4b48-a5b2-cf2fea4ef65d.png)


## __Results__

Here , we are not observing any trend or making decisions from data but here we are providing choice to customer to set his criteria for travel destinations (maximum and minimum temperatures) and from that we are getting weather data using APIs. This analysis emphasis on how to use __Application Programming Interface__ using Pandas and Python within the Jupyter Notebook. 

This analysis shows how to get data from other applications or companies through APIs for data analysis, modeling and engineering.  

