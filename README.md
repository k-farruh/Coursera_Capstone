# Applied Data Science Capstone

## Peer-graded Assignment: Capstone Project - The Battle of Neighborhoods


_Kushnazarov Farruh_  
_IBM Data Science Professional_
 

## 1) Introduction/Business Problem
The idea of this study is to help people who are planning to open a new restaurant in Toronto to choose the right location by providing data about each neighborhood's income and population and the competitors already present in the same regions.


## 2) Data
To provide the stakeholders with the necessary information, I'll be combining Toronto's 2016 Census with population, the average income per Neighborhood with Toronto's Neighborhoods shapefile, and Foursquare API to collect competitors in the same neighborhoods

Toronto's Census data is publicly available at this **[website](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#8c732154-5012-9afe-d0cd-ba3ffc813d5a)**

Toronto Neighborhoods' shapefile is publicly available at this **[website](https://www.toronto.ca/city-government/data-research-maps/open-data/open-data-catalogue/#a45bd45a-ede8-730e-1abc-93105b2c439f)**


Based on definition of our problem, factors that will influence our decission are:
* number of existing restaurants in the neighborhood (any type of restaurant)
* number of and distance to Italian restaurants in the neighborhood, if any
* distance of neighborhood from city center

We decided to use regularly spaced grid of locations, centered around city center, to define our neighborhoods.

Following data sources will be needed to extract/generate the required information:
* centers of candidate areas will be generated algorithmically and approximate addresses of centers of those areas will be obtained using **Google Maps API reverse geocoding**
* number of restaurants and their type and location in every neighborhood will be obtained using **Foursquare API**
* coordinate of Toronto center will be obtained using **Google Maps API geocoding** of well known Toronto location (Scarborough)



## 3) Methodology
For this report I used a few different maps that could help a new investor to decide the best neighborhood to open a restaurant 
in Toronto based on it's income, population and available competitors. In order to do that I've used the 2016 Census information 
combined with choropleth maps to visually display the wealthier and more populational neighborhoods and Foursquare data to display 
the current restaurants in each region.


## 4) Results
Comparing the maps we can notice the majority of the restaurants grouped on main streets and on the south of the city, although 
some of the welthiest neighborhoods are up to the north. Also, the areas with a dense population don't reflect on the number of 
restaurants.


## 5) Discussion
When I first decided to create this study I was expecting to find clusters of restaurants in certain regions and the final result 
didn't meet that expectation.


## 6) Conclusion
This report may be helpful for someone planning on opening a restaurant in Toronto, by comparing the current offers and 
neighborhoods profiles, however it may not cover all variables such as access to public transportation or even the restaurants 
profiles, so it shall not be used as a single decidion making tool.

