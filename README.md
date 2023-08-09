# python-api-challenge
Python script to visualize the weather of over 500 cities of varying distances from the equator.

Contributor: Brian Kath

Repository Structure - 

	- Main folder
		- README.md file
		- .gitignore file

	- Sub-folders
		- WeatherPy
			- output_data
				- cities.csv
				- Fig1.png
				- Fig2.png
				- Fig3.png
				- Fig4.png
			- VacationPy.ipynb
			- WeatherPy.ipynb

Overview - 

For this project, I first used a random number generator and the citipy library to create a list of 600 cities of varying distances from the equator. I then used the OpenWeatherMap api to retrieve weather data for each city in the list. I was able to gather information regarding weather characteristics such as maximum temperature, humidity, cloudiness, and wind speed for a total of 569 cities. This data was then compiled into a pandas dataframe and exported as a csv. I then used matplotlib to create several scatterplots showing the relationship between the latitude of the cities and the weather characteristics. The data was then broken up into northern and southern hempisphere cities and linear regression was calulated for the relationship between distance from the equator and the different weather characteristics.

For the second part of the project, I imported the city weather data csv and used that data to create a more narrowed down list of the 21 cities where the maximum temperature was less than 90 degrees, the cloudiness was less than 20%, and the humidity was less than 40%. I then used the new dataframe and the Geoapify api to find the nearest hotel to each city within 10,000 metres. The narrowed city dataframe was then updated to include the hotel name found for each city.