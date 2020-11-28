# 06-Weather-Dashboard# Weather Dashboard App

A weather dashboard with search functionality to find current weather conditions and the future weather outlook for multiple cities.

### Purpose

Build my first app using an API. Retrieve data from a third-party weather API (OpenWeather API) and using it in context. 

### Functionality

Build a weather dashboard application with search functionality to find current weather conditions and the future weather outlook for multiple cities. 

Use the [OpenWeather API](https://openweathermap.org/api) to retrieve weather data for cities. The documentation includes a section called "How to start" that will provide basic setup and usage instructions. Use `localStorage` to store any persistent data.

## Links:
```
Code Repo: 
     https://github.com/achaudhry93/06-Weather-Dashboard

```
## Narrative to try to accomplish:
1.  Create an app that uses OpenWeather API to retrieve weather data for cities. 
2.  Each city search is stored into the list with use of local storage.
3.  User should be able to click on a stored list item to view weather conditions of that location again even after page refresh.
4.  Current conditions are listed for the city searched, which includes city name, the date, an icon to represent the weather conditions, temperature, humidity, wind speed and the UV index.
5.  Below the current conditions a five day forecast is listed with dates, weather icon, temperature and humidity listed. 
6. **bonus** create clear click event to clear out local storage to start a new list of city searches.

## Issues:
1. Had to write line by line to get the correct calls in the correct order to pull from the weather API correctly and understand what was being coded.
2. Syntax errors/spelling errors caused a lot of my time to be eaten up as I was trying to find them.
3. I tried to do a little more and create a clear button to clear all of the listed local storage items. This button has to be clicked to clear the local storage not a refresh of the page. However, when a refresh occurs the clear local storage button stops working until another city is listed, then it will work again. Need to find out why that happens. 
4. I realized that the form needs to be somewhat specific when typing location by city and state verses just city name. Some city names by themselves work while others do not. Other times listing just the city name populates the first popular city. For example Portland is for Portland Oregon not Portland Maine until specified by state.
5. Overall the look of the app of the example gif, I didn't want to spend more on the CSS as th JS took the most time.

## User Story:

```
AS A traveler
I WANT to see the weather outlook for multiple cities
SO THAT I can plan a trip accordingly
```

## Acceptance Criteria:

```
GIVEN a weather dashboard with form inputs
WHEN I search for a city
THEN I am presented with current and future conditions for that city and that city is added to the search history
WHEN I view current weather conditions for that city
THEN I am presented with the city name, the date, an icon representation of weather conditions, the temperature, the humidity, the wind speed, and the UV index
WHEN I view the UV index
THEN I am presented with a color that indicates whether the conditions are favorable, moderate, or severe
WHEN I view future weather conditions for that city
THEN I am presented with a 5-day forecast that displays the date, an icon representation of weather conditions, the temperature, and the humidity
WHEN I click on a city in the search history
THEN I am again presented with current and future conditions for that city
WHEN I open the weather dashboard
THEN I am presented with the last searched city forecast
