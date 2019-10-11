# Chicago Ride Analysis (viz with Tableau)

## scrape data
Used socrata API to scrape 120,000 rows of data for trip ID, latitude, longitude, and pickup timestamp of ride-hailing service trips throughout Chicago.

## clean data
Used regex to convert timestamp to day of the week pickup occured as well as time of day in various formats for later use in Tableau.
Transformed the trip ID data to have the count of number of rides taken within buckets of time from the pickup timestamp.

## tableau
3 visualizations in tableau: Radial, Line, and Map.
You can view the visualizations [here](https://public.tableau.com/profile/thomas4018#!/vizhome/MostPopularTimePlacetoCallaRideinChicago/Dashboard13) on Tableau Public.

### Radial
Showed time of day within 15 minute intervals where the most pickups occured. Set up to display in a radial format to mimic that of an analog clock. Ability to filter by weekday or weekend (normalized weekday count by 5 and weekend count by 2).
### Line
Exact same data from radial, except in a line chart format. Easier to read, but not as aesthetically pleasing or novel.
### Map
Shows location of all pickups. Green for weekday and blue for weekend. Interactive in that it allows for the user to select any range of time throughout the day (smallest interval of 1 hour) to display where the density of ride pickups are occurring.

