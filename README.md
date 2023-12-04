# python-api-challenge
![map-6](https://github.com/Pooja14n/python-api-challenge/assets/144713762/92f872bf-2f9d-47c2-b2cb-dbe0e181b3e4)

In this challenge, we need to visualize the weather of over 500 cities of varying distances from the equator using weather data skills to plan future vacations. And, if pressed for more information, how would we can prove that.

# Requirements
We will be using Pandas, Jupyter Notebook, Matplotlib, Python requests, APIs, and JSON traversals for this Analysis, along with the geoViews Python library, and the Geoapify API.

This activity is broken down into two deliverables: WeatherPy and VacationPy.

# Part 1: WeatherPy
In this deliverable, we have to create a Python script to visualize the weather of over 500 cities of varying distances from the equator, for which we use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and our problem-solving skills to create a representative model of weather across cities.

# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
Use the OpenWeatherMap API to retrieve weather data from the cities list generated.

![2](https://github.com/Pooja14n/python-api-challenge/assets/144713762/48730b0d-1910-4af9-804c-eedc8a641467)
![1](https://github.com/Pooja14n/python-api-challenge/assets/144713762/736b3d77-d7f6-47be-b423-d44fe9383174)
![3](https://github.com/Pooja14n/python-api-challenge/assets/144713762/c2dae362-d157-4eb2-99ed-559522cee1f1)

To fulfill the first requirement, we use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, we create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed

Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image

Sample scatter plot with the linear regression line.

You should create the following plots:

Northern Hemisphere: Temperature vs. Latitude

Southern Hemisphere: Temperature vs. Latitude

Northern Hemisphere: Humidity vs. Latitude

Southern Hemisphere: Humidity vs. Latitude

Northern Hemisphere: Cloudiness vs. Latitude

Southern Hemisphere: Cloudiness vs. Latitude

Northern Hemisphere: Wind Speed vs. Latitude

Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

Humidity map

Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21

Wind speed less than 4.5 m/s

Zero cloudiness

NOTE
Feel free to adjust your specifications but make sure to set a reasonable limit to the number of rows returned by your API requests.

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

Hotel map
