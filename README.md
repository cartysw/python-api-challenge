# python-api-challenge

Hello!

This is a repository containing material for the Module 6 Python API Challenge through the UofM Data Analytics Bootcamp Course. You'll find folders containing both of the scripts and a folder that contains all the output data.

For the WeatherPy program we were tasked with:
- Generating random geographic coordinates and the closest city to those coordinates
- Using an api to pull live weather data from those cities
- Plot comparison scatter charts comparing the latitude of the cities to factors like temperature, humidity, wind speed, etc.
- Divide data into groups based on whether they are located in the northern/southern hemisphere of the globe
- Calculate a linear regression line for each hemisphere comparison chart and plot it
- Determine if there are any correlations and discuss any findings

For the VacationPy program we were tasked with:
- Importing data gathered from WeatherPy
- Create a hvplot map that displays the location and data of each city, with each point's size determined by it's reported humidity
- Set up some filters to find a desired vacation destination. The filters I chose were:
  -  Cities reporting temperatures between 10 and 20 degress celsius
  -  Cities reporting a humidity percentage of less than 72
  -  Cities reporting a wind speed of less than 4 m/s
- Creating a dataframe that contains hotel info for those cities
- Searching for a hotel within 10000 meters of a citie's coordinates
- Creating one last map plot that shows the resulting cities, an abbreviation for their country name, and info on the closest hotel (if found)

I hope this project proves to be helpful and insightful!

Some references were used during the creation of these scripts:

Got help from the Xpert learning assistant (through UofM course) with debugging my linear regression function, specifically for fixing something in the "plt.annotate()" code line. Here's a snippet of the prompt I used:
i correctly plotted a scatter chart comparing the northern hemisphere latitudes to max temperatures, but my plot doing the same but for the southern hemisphere isnt displaying the y=mx + b equation on the graph.

Also with the assistant, got some help with doing some city name data cleaning, specifically for vacationpy map plotting. heres a prompt snippet:
im using hvplot.pandas to plot out all those cities from the api challenge. ive imported the data correctly but i keep getting this error: ValueError [Call holoviews.ipython.show_traceback() for details].

Referenced this for my function that filters the gathered cities by a given temperature range:
https://stackoverflow.com/questions/31617845/how-to-select-rows-in-a-dataframe-between-two-values

Referenced this to help write my function that makes a copy of the filtered weather data dataframe in vacationpy:
https://stackoverflow.com/questions/34682828/extracting-specific-selected-columns-to-new-dataframe-as-a-copy

Referenced this when adding additional info to the hover message for each city in the step 5 plot:
https://discourse.holoviz.org/t/how-to-add-an-extra-variable-to-hover-on-image-or-contourf-plot/1664

Referenced this when changing fontsize of the legend for the step 5 plot:
https://stackoverflow.com/questions/59070661/change-fontsize-in-holoviews-or-hvplot
