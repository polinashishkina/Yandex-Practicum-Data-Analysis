# Project "Moscow Food Services Market Research"

## Project Description

### Data
***Table rest_data:***
* object_name — Name of Food Place;
* chain — Chain Restaurant;
* object_type — Type of Food Place;
* address — Address;
* number — Number of Seats.

***Table region_moscow:***
* street — Street Name;
* district — Name of the Administrative District (AD)
* quantity_district — Number of Districts through Which the Street Passes
* region — Name of the District
* quantity_region — Number of Districts through Which the Street Passes

### Objective:
Research the food market based on open data for investors

### Tasks:
Step 1. Data Preprocessing

Step 2. Data Analysis

2.1. Ratio of catering types by quantity

2.2. Ratio of chain and non-chain places

2.3. Type of places characterized by chain distribution

2.4. Chain places: the relationship between the number of places in a chain and the number of seats

2.5. Average number of seats for each type of places

2.6. Separating "streets" from the address into a separate column

2.7. Top 10 streets by number of places

2.8. Distribution of the number of seats for streets with a large number of catering places

2.9. Neighborhoods with streets containing only one places

Step 3. General Conclusion

### Conclusions:

1. Ratio of food service establishment types by quantity:

* Cafes account for the largest share of food service types by quantity - 39.7%
* Canteens are second - 16.8%
* Restaurants are third - 14.9%
* Fast food places are fourth - 12.5%
* The share of other places types is less than 6% (bars, buffets, cafeterias, snack bars, stores
(deli department))

2. Ratio of chain and non-chain places by quantity:

* Non-chain food services - 12,398 units
* Chain food services - 2,968 units

Thus, there are four times more non-chain food services in Moscow.

3. Types of catering services characterized by chain distribution:

* Chain distribution is primarily typical for fast food places. 41% of places are chains.

* Stores (deli departments) rank second, with 29% of places being chains.

* Restaurants and cafes rank third, with 24% and 23%, respectively.

4. Dependence of seating in chain places on the number of places within the chain:

According to the data, chain food services may not have seating. For example, in shopping mall food courts, where there is a pickup point and a common area with seating that is not assigned to a specific cafe or catering. Or, for example, a pickup window in fast food chains.

Places with no or one seating:

* These are primarily fast food services – 45.9%. They are located in a food court—a food court in a shopping center, airport, or, in some cases, a separate building (e.g., "Depot"), where customers are served by several food places sharing a common dining area.
* Cafés rank second at 19.4%
* Stores (deli department) rank third at 13.1%

Analysis of the number of seats for all chain food services:

* 25% of chain places have no more than 15 seats.
* The average number of seats for chain establishments is 40.
* 75% of chain places have no more than 72 seats.
* 90% of chain food service places have no more than 120 seats.

When analyzing the relationship between the number of places in a chain and the number of seats in those places, a negative linear correlation was found. The fewer places in a chain, the more seats they have, and vice versa, the more places in a chain, the fewer seats.

6. Average number of seats for each type of food service.

*Canteens* have the largest average number of seats – 103.
25% of canteens (lower quartile) have approximately 50 seats.

The upper quartile has approximately 200 seats.

*Restaurants* come in second. The average restaurant has 80 seats.
25% of restaurants (lower quartile) have approximately 45 seats.
The upper quartile has approximately 120 seats.

The third-largest group is *bars, buffets, and cafes*. These places have approximately 30-35 seats on average. 25% of places in this group (the lower quartile) have around 20 seats.
The difference lies in the upper quartile. While the upper quartile for cafes and bars is around 50 seats, for buffets it's higher – around 80.

The last group: *cafeteria, fast food place, diner, store (deli department)*. This group is characterized by minimal seating capacity. The lower quartile for places in this group is 0 seats. The upper quartile for cafeterias, diner, and store (deli department) does not exceed 13 seats, while fast food places have 25 seats. The average for this group ranges from 0 to 5.

7. Top 10 streets by number of food services:

Prospekt Mira, Profsoyuznaya Street, Leningradsky Prospekt, Presnenskaya Embankment, Varshavskoe Shosse, Leninsky Prospekt, Vernadskogo Prospekt, Kutuzovsky Prospekt, Kashirskoe Shosse, and Kirovogradskaya Street.

These streets pass through several districts of Moscow. For example, Varshavskoe Shosse and Leninsky Prospekt stretch across eight districts, and Prospekt Mira stretches across seven districts. The only exception is Presnenskaya Embankment, which is located in a single district. Consequently, these streets are long, which explains the large number of places located there.

8. Distribution of seating capacity for streets with a large number of food services:

We see a slight positive linear correlation. The more places on a street, the more seats they have.

9. Streets with one food service place: The dataframe contains 722 streets with one food service place. These streets are located throughout almost all of Moscow, namely in 77 districts. These districts are located in all administrative districts.

The Central Administrative District, located in the city center, has the highest number of streets with one food service place, with 21.1%. It can be assumed that the streets with one place each are small side streets in the city center.

District statistics:
- Central - 21.1%
- Southeast - 13%
- Northeast - 11.4%
- East - 11.4%
- West - 11.4%
- Northwest - 11.4%
- North - 8.94%
- South - 5.69%
- Southwest - 4.07%
- Troitsky - 0.8%
- Novomoskovsky - 0.8%

10. When choosing a café location, information about streets with one place or the largest number of places is not enough. The following factors must also be considered:

* The price range of our café: affordable or expensive, trendy. Based on this, one should choose a district/street and analyze one's closest competitors in the same price range.
* The number of people passing by the café entrance per unit of time. * Transportation accessibility (including public transportation), parking options
* The composition of the area's residents, workers, and casual visitors. This is important because, for example, if one locate in an office district, it can be quite difficult to fill the cafe on weekends.
* Analysis of nearby facilities – are there business centers, institutions, universities, shopping malls, etc.
* The place's cuisine is unknown (European, Asian, etc.). Once the initial interest in robots fades, customers will evaluate the place's cuisine. It's important to understand what competitors will be in the neighbouring area of the new cafe, and in what numbers; probably, there's no point in opening an eighth Italian café.

### Tools and skills used in the project:
Python, plotly, matplotlib, seaborn libraries, data visualization.
