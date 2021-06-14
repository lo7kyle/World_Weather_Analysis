# World_Weather_Analysis
Weather analysis using python, matplotlib, statistics, pandas, API's

## Overview:
In this challenge we were given a task to create an app that helps plan someone's trip around weather reccomendations. We were to use APIs to find cities with the user's maximum and minimum temperature for a vacation. We were then tasked to also create an itinerary and find potential travel destinations between the cities.

## Purpose:
The purpose of this challenge is to help us practice using different APIs to scrap data from the web. In this challenge we created data frames using data in JSON format and converting it into CSVs for analysis. This challenge is to familiarize ourselves with the different syntax of each APIs (gmaps, openweatherapi) and understand the basics of scraping the web data needed for analysis 

## Resources
* Data Source: WeatherPy_vacation.csv, WeatherPy_Database
* Software Python 3.8.8, Conda 4.10.1, Jupyter Notebook 6.3.0

## Breakdown

### Retrieve Weather Data

The first task was to create a data base out of randomly generated latitudes and longitudes. We used the Citipy module in python to search the nearest cities with the random latitudes and longitude. We then used the Openweather API to retrieve the following of each city: latitude/longitude, Maximum temperature, humidity, percent cloudiness, windspeed, and weather description (clouds, fog, rain, clear sky). We took this data in JSON format and stored it into a data frame using Pandas. We then exported it as a CSV to use it in our next task. 

### Create a Customer Travel Destinations Map

In our second task I had to create a map that recommended cities based off the user's input. The user would input a minimum temperature and a maximum temperature, and we were supposed to populate cities all around the world with those current temperatures and locate the nearest hotels. In this part of the challenge, I learned how to use the CSV created from the JSON data and use gmaps API to locate the nearest hotels. I also learned basic HTML with the markers layer. 

![World Map Markers](https://github.com/lo7kyle/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)


### Create a Travel Itinerary Map 

As our final task for this challenge, we were to add a feature in our current app that uses Google Directions API to create a travel itinerary that shows routes between 4 cities chosen. I chose 4 cities in Japan since many people love traveling to Japan. In this part of the challenge, we are to create a marker layer map along with a directions layer map. In this challenge I was trying to overlay the two, but I couldn't do so. I am not sure if we can include both the route and the hotel markers. Similarly, to part 2 of this challenge, we are to also include the hotels in the marker along with the city, Country, and current weather. 

![Japan Travel Route](https://github.com/lo7kyle/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

![Japan Travel Map Markers](https://github.com/lo7kyle/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
