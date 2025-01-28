# python-api-challenge
Python API Challenge for Data Analytics

VacationPy Analysis:

    The purpose of this analysis was to find a hotel at selected GPS locations based upon ideal weather for a vacation. 
    First the data is read into a Dataframe from a CSV file. These locations are plotted on a geographical plot. 
    Then the data is narrowed down to include only the locations that include the ideal weather specifications. 
    A new Dataframe was created to hold the narrow list and include the hotels found for each location within 10,000 meters. 
    I used the geoapify API to acquire the hotel data with the given GPS locations. If no hotel was found this 
    exception was just filled with a message stating that no hotel was found. After all of the data was stripped down to my
    ideal weather for a vacation there were around 15 locations worldwide. This code could be used as a base for a mobile 
    application or webapp to help people plan their ideal vacation based upon the weather. Other criteria could be added 
    as well for an even more precise vacation spot. Like hotels with a hospital close by or a large selection of restaurants. 


WeatherPy Analysis:

	What is the weather like as we approach the equator? It gets hotter. Now try to show that with data. For this part 
    of the challenge, we used citipy from the python libraries and the openweathermap API. First, I generated random 
    latitudes and longitudes to get a list of cities from citipy. Then we used openweathermap API to get weather data from
    the list of GPS points. This data was converted into a Dataframe. The Dataframe was written to a CSV file. Next, I 
    generated the scatter plots of latitude vs. max temperature, latitude vs. humidity, latitude vs. cloudiness, and 
    latitude vs. wind speed. I created a function to do the linear regression and plotting for me, as suggested in 
    the notes. This function takes two arguments. The x values and y values for linregress are passed to said function. 
    Then the values are used to create a plot and compute the r^2 value. The analysis was split between the northern 
    hemisphere and the southern hemisphere. The analysis clearly shows that the weather does indeed get hotter as we 
    approach the equator. Unfortunately, everything else is kind of all over the place. It doesn’t look like we can 
    accurately predict the wind speed, humidity, or cloudiness from our data.
