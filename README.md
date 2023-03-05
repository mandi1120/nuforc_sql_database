# Amanda Hanway - Databases for Analytics, Module 7
- Project: Create a SQL database and query the data  
- Date: 10/2/22

## Overview:  
This project was created as a final assignment for a master's course at NWMSU, Databases for Analytics.  

### Requirements  
- Create a database  
- Your database must include at least three tables
- One table must have at least 1,000 rows, and two other tables must have at least 100 rows
- There must be at least one date data type, one numeric data type, and one string data type

### SQL Database Procedure Overview   
Step 1: Create a new database named nuforc
Step 2: Create a table in the nuforc database called Ufo_Sighting_Data and insert the raw data from UFO_Sighting_Data.csv     
Step 3: Clean the UFO data and insert it into a new table  
    - Create a new table called Ufo_Sightings to hold the cleaned dataset  
    - Select the raw data from Ufo_Sighting_Data table  
    - Create new column date_time_key  
    - Create new column date_documented_key  
    - Remove special and non-numeric characters from the latitude and longitude columns  
Step 4: Create a calendar table in the nuforc database called dim_date and insert the data from Calendar.csv  
Step 5: Create a cities table in the nuforc database called dim_cities and insert the data from US_Cities_Top_1K.csv  
    - Update column state_code using a case statement  
Step 6: Create a view in the nuforc database called US_Sightings_After_2000 to extract sightings in the US on or after 1/1/2000
Step 7: Create a temporary table in the nuforc database called US_Sightings_by_City that joins the latitude and longitude to the UFO data

### Data Files
- [UFO_Sighting_Data](files/UFO_SIGHTING_DATA.CSV)
- [Dim_Date](files/CALENDAR.CSV)
- [Dim_Cities](files/US-CITIES-TOP-1K.CSV)

### Data Sources
- UFO Sighting Data: [kaggle](https://www.kaggle.com/datasets/camnugent/ufo-sightings-around-the-world)  
- Date data: [data.world](https://data.world/cegomez22/dimdate) 
- City data: [github](https://raw.githubusercontent.com/plotly/datasets/master/us-cities-top-1k.csv)  

## Screenshots:

### Database:
![Database](files/database.png)

### UFO_Sighting_Data:
![UFO_Sighting_Data](files/ufo_sighting_data_screenshot.png)

### Dim_cities:
![Dim_cities](files/dim_cities_screenshot.png)

### Dim_date:
![Dim_date](files/dim_date_screenshot.png)

### UFO_sightings (cleaned):
![UFO_Sightings (cleaned)](files/ufo_sightings_screenshot.png)

### UFO_Sightings_After_2000:
![UFO_Sightings_After_2000](files/ufo_sightings_after_2000_screenshot.png)

### US_Sightings_by_City:
![US_Sightings_by_City](files/us_sightings_by_city_screenshot.png)

### Query: Count of Rows:
![Query: Count of Rows](files/table_size_screenshot.png)

### Query: Aggregated by Shape and Weekday:
![Query: Aggregated by Shape and Weekday](files/weekday_shape_aggregate_query_screenshot.png)

### Query: Aggregated by City Population:
![Query: Aggregated by City Population](files/population_aggregate_query_screenshot.png)






