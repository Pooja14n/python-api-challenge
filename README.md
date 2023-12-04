# python-api-challenge
![map-6](https://github.com/Pooja14n/python-api-challenge/assets/144713762/92f872bf-2f9d-47c2-b2cb-dbe0e181b3e4)

In this challenge, we need to visualize the weather of over 500 cities of varying distances from the equator using weather data skills to plan future vacations. And, if pressed for more information, how would we can prove that.

# Requirements
We will be using Pandas, Jupyter Notebook, Matplotlib, Python requests, APIs, and JSON traversals for this Analysis, along with the geoViews Python library, and the Geoapify API.

This activity is broken down into two deliverables: WeatherPy and VacationPy.

# Part 1: WeatherPy
In this deliverable, we have to create a Python script to visualize the weather of over 500 cities of varying distances from the equator, for which we use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and our problem-solving skills to create a representative model of weather across cities.

# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
1. Use the OpenWeatherMap API to retrieve weather data from the cities list generated. 

![2](https://github.com/Pooja14n/python-api-challenge/assets/144713762/48730b0d-1910-4af9-804c-eedc8a641467)

![1](https://github.com/Pooja14n/python-api-challenge/assets/144713762/736b3d77-d7f6-47be-b423-d44fe9383174)

![3](https://github.com/Pooja14n/python-api-challenge/assets/144713762/c2dae362-d157-4eb2-99ed-559522cee1f1)

![5](https://github.com/Pooja14n/python-api-challenge/assets/144713762/8fea80df-131e-452a-9091-f6122e8c5781)

![4](https://github.com/Pooja14n/python-api-challenge/assets/144713762/b147f1e1-5efb-422b-a27c-db78394dcc29)

2. Next, we create a series of scatter plots to showcase the following relationships:

  a. Latitude vs. Temperature

  ![6](https://github.com/Pooja14n/python-api-challenge/assets/144713762/7e99104f-f4cf-4509-822f-3419db89a29a)

  b. Latitude vs. Humidity

  ![7](https://github.com/Pooja14n/python-api-challenge/assets/144713762/35111297-0463-4d6f-ab2c-307232fab4e3)

  c. Latitude vs. Cloudiness

  ![8](https://github.com/Pooja14n/python-api-challenge/assets/144713762/35b8b94b-1acb-43f6-995a-5cd72c69adcb)

  d. Latitude vs. Wind Speed

  ![9](https://github.com/Pooja14n/python-api-challenge/assets/144713762/32b95a71-1d07-4171-b045-b532edebbee6)

# Requirement 2: Compute Linear Regression for Each Relationship
1. Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 

![11](https://github.com/Pooja14n/python-api-challenge/assets/144713762/45850521-e7bc-4f64-ae59-c9d17ef28200)

![10](https://github.com/Pooja14n/python-api-challenge/assets/144713762/dff853b0-5ed2-4339-87c1-596c44641de2)

2. Next, create a series of scatter plots and include the linear regression line, the model's formula, and the r values for the following plots:

  a. Northern Hemisphere: Temperature vs. Latitude
  ![12](https://github.com/Pooja14n/python-api-challenge/assets/144713762/d1ac456d-9338-42a5-b2d9-298f7d4d8e24)

  b. Southern Hemisphere: Temperature vs. Latitude
  ![13](https://github.com/Pooja14n/python-api-challenge/assets/144713762/1178bd88-7ba8-4426-8e36-992cf1829d49)

  c. Northern Hemisphere: Humidity vs. Latitude
  ![14](https://github.com/Pooja14n/python-api-challenge/assets/144713762/3a95195b-0d19-4309-8cc2-80ce5051a977)

  d. Southern Hemisphere: Humidity vs. Latitude
  ![15](https://github.com/Pooja14n/python-api-challenge/assets/144713762/a9e60f9d-d16e-4422-84c5-7f7a8f9cbe26)

  e. Northern Hemisphere: Cloudiness vs. Latitude
  ![16](https://github.com/Pooja14n/python-api-challenge/assets/144713762/194649e8-8e69-4bf1-babc-e4b9baabb8a5)

  f. Southern Hemisphere: Cloudiness vs. Latitude
  ![17](https://github.com/Pooja14n/python-api-challenge/assets/144713762/dc417e25-a599-49fb-b149-9cf22430871f)

  g. Northern Hemisphere: Wind Speed vs. Latitude
  ![18](https://github.com/Pooja14n/python-api-challenge/assets/144713762/268259b5-8364-4eb5-8e3d-4dd4477a5d0f)

  h.Southern Hemisphere: Wind Speed vs. Latitude
  ![19](https://github.com/Pooja14n/python-api-challenge/assets/144713762/33361318-1905-4964-a582-c4b17f0f5ae3)

After each pair of plots, explain what the linear regression is modeling. Describe any relationships and any other findings you may uncover.

# Part 2: VacationPy
In this deliverable, we will use weather data skills to plan future vacations. 

1. Load the CSV file created in Part 1 into a Pandas DataFrame and display sample data

![1](https://github.com/Pooja14n/python-api-challenge/assets/144713762/57cdc783-f77e-49fe-91c8-2092c091dfb7)

The main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

2. Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

![2](https://github.com/Pooja14n/python-api-challenge/assets/144713762/4614a1d6-f8fb-4656-bd18-4324cd5c26d7)

3. Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:

  -> A max temperature lower than 27 degrees but higher than 21
  -> Wind speed less than 4.5 m/s
  -> Zero cloudiness

![3](https://github.com/Pooja14n/python-api-challenge/assets/144713762/b463acaa-8f49-4c5c-a965-148b28b642f5)

4. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

![4](https://github.com/Pooja14n/python-api-challenge/assets/144713762/d26315a4-20cc-463e-bb84-dcce46e69618)

5. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

![5](https://github.com/Pooja14n/python-api-challenge/assets/144713762/d13c0565-e31f-47f3-8731-3faf457c7c4d)

6. Add the hotel name and the country as additional information in the hover message for each city on the map:

![6](https://github.com/Pooja14n/python-api-challenge/assets/144713762/a9c5fa39-526b-449b-94b7-ece2f3715931)

