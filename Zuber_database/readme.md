# Zuber Database

Zuber, a new ride-sharing company that's launching in Chicago. My task were to find patterns to understand passenger preferences and the impact of external factors on rides. Working with a database, analyze data from competitors and test a hypothesis about the impact of weather on ride frequency. 

## Table schema
<img width="650" alt="image" src="https://github.com/user-attachments/assets/ef9ff12f-8951-4ebf-9fa3-0084568e65b9"/>

### Tables

The database consists of the following tables:

* **`neighborhoods:`** This table stores data on city neighborhoods.
    * **`name:`** (text) The name of the neighborhood.
    * **`neighborhood_id:`** (text) The neighborhood code.

* **`cabs:`** This table stores data on taxis.
    * **`cab_id:`** (text) The vehicle code.
    * **`vehicle_id:`** (text) The vehicle's technical ID.
    * **`company_name:`** (text) The company that owns the vehicle.

* **`trips:`** This table stores data on rides.
    * **`trip_id`:** (text) The ride code.
    * **`cab_id:`** (text) The code of the vehicle operating the ride.
    * **`start_ts:`** (datetime) The date and time of the beginning of the ride (time rounded to the hour).
    * **`end_ts:`** (datetime) The date and time of the end of the ride (time rounded to the hour).
    * **`duration_seconds:`** (number) The ride duration in seconds.
    * **`distance_miles:`** (number) The ride distance in miles.
    * **`pickup_location_id:`** (text) The pickup neighborhood code.
    * **`dropoff_location_id:`** (text) The dropoff neighborhood code.
  
* **`weather_records:`** This table stores data on weather.
    * **`record_id:`** (text) The weather record code.
    * **`ts:`** (datetime) The record date and time (time rounded to the hour).
    * **`temperature:`** (number) The temperature when the record was taken.
    * **`description:`** (text) A brief description of weather conditions, e.g. "light rain" or "scattered clouds".

### Relationships

* A neighborhood can have many taxi rides (one-to-many relationship between neighborhoods and trips tables).
* A taxi can have many rides (one-to-many relationship between cabs and trips tables).
* A ride starts in one neighborhood and ends in another neighborhood (many-to-many relationship between neighborhoods and trips tables).
* A weather record is associated with a specific date and time (one-to-one relationship between weather_records and ts).

## Step 1: Exploratory Data Analysis

1. Calculate the number of taxi rides for each taxi company on November 15-16, 2017. Name the result `trips_amount` and display it with `company_name`, sorted by `trips_amount` in descending order.
   
2. Calculate the number of rides for taxi companies with names containing "Yellow" or "Blue" from November 1-7, 2017. Name the result `trips_amount` and group the results by `company_name` field.

3. For November 2017, find the number of rides for "Flash Cab" and "Taxi Affiliation Services". Find the number of rides for these two companies and name the resulting variable `trips_amount` and group the rest of the companies as "Other", Group the data by taxi company names. sort the results by `trips_amount` in descending order.

## Step 2: Analyze Ride Duration on Rainy Saturdays

1. Retrieve the neighborhood identifiers for O'Hare and the Loop from the `neighborhoods` table.

2. For each hour, get the weather condition from the `weather_records` table. break statement into two categorize conditions as "Bad" if description contains(rain or storm), and "Good" for others. Include the `date`, `hour` (ts), and the weather condition field `weather_conditions`.

3. Retrieve all Saturday rides from the Loop (`neighborhood_id:` 50) to O'Hare (`neighborhood_id:` 63) and their weather conditions. Calculate the ride durations and exclude any rides without weather data.

### [Sql Queries](https://github.com/dpatel2512/projects_TripleTen/blob/main/Zuber_database/Zuber%20Database.pdf)

