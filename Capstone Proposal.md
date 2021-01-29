# Comparing Venues and Amenities of London Neighhourhoods to Major EU Cities
# Maurice O’Neill

### 1. Introduction
#### 1.1 Background
London has been the financial capital of not only the United Kingdom but the European Union and Europe at large for decades. The prosperity of the city has drawn many to the city making it one of the most diverse and densely populated cities in the world. With the advent of Brexit, meaning that the United Kingdom has left the European Union, the future of London’s place as the financial capital of Europe remains to be seen. No longer having full access to the European single market and as well as a whole host of other benefits, many Londoners may be looking to migrate from the UK to cities within the EU.

#### 1.2 Problem
Moving to foreign countries can be a difficult task and finding the right areas with all of the amenities that one has become accustomed to could be difficult. This project aims to analyse the neighbourhoods of cities comparable to London to find similar areas in terms of amenities and venues.

#### 1.3 Interest
Any would be migrants to major European cities would be interested in finding areas similar to the areas that they live in in London.

### 2. Data Acquisition
#### 2.1 Data Sources and Cleaning
The cities used to compare in this project were London, Paris, and Berlin. Paris and Berlin were chosen as they are the financial centers of the two most wealthy nations in the EU. They are also the largest cities in their respective nations and the most populous, making them the most comparable 
    A dataset including the latitude and longitude of the neighbourhoods of each city were created through various means. Paris was the simplest as it has twenty neighbhourhoods each with a corresponding post code. These postcodes were obtained and through this their latitude and longitude were obtained. 
    Both London and Berlin have more complicated postcode systems with neighbourhoods sharing postcodes or having multiple postcodes. A list of neighbourhoods were obtained from [here](https://en.wikipedia.org/wiki/List_of_areas_of_London) and [here](https://en.wikipedia.org/wiki/List_of_cities_in_Germany_by_population). Only the London neighbourhoods with the London post town were used. The latitude and longitude of each of these locations was then generated.
    Using the Foursquare API, a list of venues within a five-hundred metre radius of the latitude and longitude of each neighbhourhood was scraped. These datasets were then converted into a format usable for KNN clustering through one-hot encoding.
