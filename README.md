# Weather_App_API

The 'Weather Data Fetcher' is a Python script that leverages the [OpenWeatherMap API] (https://openweathermap.org/api) to fetch real-time weather data for any city.

## Getting Started

To run this script, you will need Python 3.6+ installed on your machine, as well as the `requests` library. You can install this library using pip:

pip install requests

You will also need an API key from OpenWeatherMap. You can obtain this key by creating a free account on their [website](https://home.openweathermap.org/users/sign_up). 
Once you have the key, replace the `YOUR_API_KEY` placeholder in the script with your actual key.

API_KEY = "YOUR_API_KEY"

## Usage
To use the script, run it using the Python interpreter. The script will prompt you to input the name of a city. The script will then fetch and display the current weather for that city.

python weather_fetcher.py

When prompted, enter the name of the city you want to check the weather for:

Enter the city name: London

## Functions
The script consists of two main functions:

get_weather_data(city_name): This function makes a GET request to the OpenWeatherMap API and fetches the weather data for the specified city. 
The function takes as input a string representing the name of the city, and returns a JSON object containing the weather data.

display_weather_data(data): This function takes the JSON response from the get_weather_data() function and prints the city's weather data in a user-friendly format.

## Error Handling
The script includes basic error handling. If the GET request to the OpenWeatherMap API fails for any reason, the script will print an error message. Similarly, if the returned data cannot be parsed correctly, the script will print an error message.

## Conclusion
This script provides a simple way to fetch and display real-time weather data for any city. It serves as a basic demonstration of how to interact with a web API using Python.
