# SQLAlchemy-Climate-Analysis

### Part 1: Analyze and Explore the Climate Data
- Used Python and SQLAlchemy to do a basic climate analysis and data exploration of my climate database. Specifically, used SQLAlchemy ORM queries, Pandas, and Matplotlib.
- Used the SQLAlchemy create_engine() function to connect to my SQLite database.
- Used the SQLAlchemy automap_base() function to reflect my tables into classes, and then saved references to the classes named station and measurement.
- Linked Python to the database by creating a SQLAlchemy session.

![precipitation](https://user-images.githubusercontent.com/10196762/224149581-be1624bf-648e-486e-b2bd-4446f0f069bd.jpg)
![station-histogram](https://user-images.githubusercontent.com/10196762/224151120-1d8d8ea5-290e-4041-92f0-7af6067010e6.jpg)


### Part 2: Designed My Climate App
- Designed a Flask API based on the queries that I developed throughout part 1. 
- Converted the query results from my precipitation analysis (i.e. retrieved only the last 12 months of data) to a dictionary using date as the key and prcp as the value.
- Returned the JSON representation of my dictionary.
- Returned a JSON list of stations from the dataset.
- Queried the dates and temperature observations of the most-active station for the previous year of data.
- Returned a JSON list of temperature observations for the previous year.
- Returned a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.
- For a specified start, calculated TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.
- For a specified start date and end date, calculated TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.


