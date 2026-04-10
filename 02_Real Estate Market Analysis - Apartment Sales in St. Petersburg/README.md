# Project "Real Estate Market Analysis - Apartment Sales in St. Petersburg"

### Project Description

### Data

* airports_nearest — distance to the nearest airport in meters (m)
* balcony — number of balconies
* ceiling_height — ceiling height (m)
* cityCenters_nearest — distance to the city center (m)
* days_exposition — number of days the listing was posted (from publication to removal)
* first_day_exposition — publication date
* floor — floor
* floors_total — total number of floors in the building
* is_apartment — apartment (boolean)
* kitchen_area — kitchen area in square meters (m²)
* last_price — price at the time of removal
* living_area — living area in square meters (m²)
* locality_name — name of the locality
* open_plan — open plan (boolean)
* parks_around3000 — number of parks within a 3 km radius
* parks_nearest — distance to the nearest park (m)
* ponds_around3000 — number of ponds within a 3 km radius
* ponds_nearest — distance to the nearest pond (m)
* rooms — number of rooms
* studio — studio apartment (boolean)
* total_area — apartment area in square meters (m²)
* total_images — number of photos of the apartment in the listing

Explanation: Apartments are non-residential premises that are not classified as residential but have the necessary conditions for occupancy.

### Objective:
Data taken from the Yandex.RealEstate service — an archive of apartment listings in St. Petersburg and neighboring towns over several years.
We would like to learn how to determine the market value of real estate. The goal of the project is to establish key value parameters. This will allow us to build an automated system that will detect anomalies and fraudulent activity. Two types of data are available for each apartment for sale. The first is entered by the user, while the second is automatically obtained based on map data. For example, the distance to the city center, airport, nearest park, and pond.

### Tasks:
1. Data preprocessing
2. Calculation for:
* price per square meter;
* day of the week, month, and year the ad was published;
* apartment floor (options: first, last, other);
* ratio of living space to total area, as well as the ratio of kitchen area to total area.
3. Exploratory data analysis
* Study the following parameters: area, price, number of rooms, ceiling height.
* Study the time it took to sell the apartment. When can a sale be considered very quick, and when an unusually long one?
* What factors influence the price of an apartment the most?
* Select 10 towns with the largest number of listings. Calculate the average price per square meter in these towns.
* Select a segment of apartments in central St. Petersburg and analyze it.

### Conclusions:
To understand which factors influence apartment prices the most, the analysis was conducted using two databases:
- General database for St. Petersburg and the Leningrad Region
- Segment of apartments in central St. Petersburg.

The factors that most influence apartment prices are:
- Distance from the center
- Price per square meter
- Area

The following factors have a lesser influence:
- Number of rooms
- Floor
- Year of listing

No influence:
- Day of listing
- Month of listing

When comparing the data from the two databases, the following features were identified:

1. Apartment area in square meters

For the general database, the majority of apartments are 40-45 square meters.
In central St. Petersburg, the majority are 70-80 square meters.

2. Price

For the general database, the majority are apartments priced between 3-4 million rubles. In the central St. Petersburg apartment segment, the majority of apartments are priced between 8.5 and 9 million rubles.

3. Number of rooms

One-room apartments (also including studio apartments) make up the majority of the total inventory.
In the central St. Petersburg apartment segment, two-room apartments make up the majority.

4. Ceilings

In the central St. Petersburg apartment segment, the majority of apartments have ceilings in the 2.6-2.7 m range.
In the central St. Petersburg apartment segment, the majority of apartments have ceilings in the 2.7-2.8 m range.

On average, apartments take 45 to 60 days to sell.

A quick sale can be considered if the transaction closed within 25 days (25% quartile - 22 days).
A long sale can be considered if it took longer than 120 days (75% quartile - 199 days).

10 settlements with the most listings:

St. Petersburg, Murino, Shushary, Vsevolozhsk, Pushkin, Kolpino, Pargolovo, Gatchina, Kudrovo, Vyborg.

### Libraries and tools used
Pandas, plotly, matplotlib libraries, data preprocessing, exploratory data analysis, data visualization
