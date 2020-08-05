# Hot Spots for Fitness
Capstone project for the IBM Data Science Certification

# Introduction
In my home city of Austin, fitness groups are attracting a following of customers by moving away from traditional large gyms and moving closer to their customers. Companies such as Camp Gladiator setup outdoor meetup locations across the city in areas that would be convenient for people looking to workout. They focus on areas with higher density populations of people that are more likely to be active, around office parks, schools, suburban areas, and more.

My program will help companies like Camp Gladiator identify the best locations to setup a new outdoor location. It will recommended "hot spots" by identifying areas that have trending venues related to health (healthly restaurants, active wear shopping, etc) and no gyms within close promixity.

# Data
To develop the program, I will use location and venue data from the Foursquare API for Toronto, Canada. These are the specific endpoints that will be used:

• Trending: get trending venues

• Categories: get venue categories

• Explore: get venue recommendations


I will also use two other data sources to identify neighborhoods in Toronto:

• Neighborhood names: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

• Neighborhood locations: https://cocl.us/Geospatial_data

# Methodology

The process to analyze this data will be as follows:

• Identify neighborhoods in Toronto (https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M)

• Identify latitude and longitude of each neighborhood (https://cocl.us/Geospatial_data)

• Lookup top 5 trending venues for each neighborhood (Foursquare API - Trending)

• Filter neighborhoods that have a health venue in top 5 trending venues (Foursquare API - Categories)

• Verify if a gym is within 5 miles of the filtered list of neighborhoods (Foursquare API - Explore)

• Present final list of "hot spots"
