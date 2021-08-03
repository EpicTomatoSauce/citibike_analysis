# Citi Bike Analysis
An analysis into the Citi Bike 2020 (Jersey City) Dataset using a combination of Jupyter Notebook and Tableau. The purpose is to explore any trends within the data and to assist with any future decision making about the program. This includes decisions about the stations, assets and / or membership to the program.

* Which are the most / least popular stations?
* Is there a relationship between the station popularity any socio-demographic factors such as median income per zip code?
* Is there any seasonality in the program? i.e. popularity across months / seasons?
* How can the existing data provide exploratory analysis to bike condition?
* 
## Data
```
Data sourced from [Citi Bike System Data](https://www.citibikenyc.com/system-data) using the 2020 Jersey City, City of New Jersey data from 2020.
Additional information pertaining to the stations was sourced from the live [GBFS Feed](http://gbfs.citibikenyc.com/gbfs/gbfs.json). Specifically, the [Station Information](https://gbfs.citibikenyc.com/gbfs/en/station_information.json) data was used.

Data was extracted, transformed and loaded using Jupyter Notebook and can be reference in the etl.ipynb file. To add further detail to the analysis, data for the station information was also imported and saved as a csv file to allow a Tableau union to be formed between the datasets.
```
## Tableau:

### Introduction to Analysis

Introductory page to the Tableau story which outlines the dataset and what are some the questions which can be answered through it.
![Story 1](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%201.png?raw=true)

### Seasonality of Trips in the Dataset
Unsurprisingly, the seasons of Summer and Fall (June through to December in the USA) are the most popular for the use of Citi Bikes. This is likely due to the climate at the time. Winter and Spring are similar in popularity likely due to the onset or melting of the snow through winter and fall.
![Story 2](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%202.png?raw=true)

### Trip Starting Times based on Popular / Unpopular seasons
As it can be quite warm during Summer, it is unsurprising to see that the overwhelming number of trips are taken later in the evening. Perhaps this is from people wanting to unwind after their day at work, or using the Citi Bike system to return home from the office.
![Story 3](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%203.png?raw=true)

### Gender Representation in the Riders
Not only does this visualisation show the relationship between the seasonalisation of the use of the system through the year, but it also highlights that the overwhelming number of rides through the year are taken by males. Visually, it would appear that on average, around 60% of the riders are male. In Winter particularly, the vast majority of users are male. However, when you then compare the trip duration of the riders through the seasons, there appears to be a relatively even distribution between males, females and the unknown category. That being said, if the Unknown category could be eliminated and the results accurately distributed between the Male and Female categories, perhaps other inferences could be made. That being said, the data as is may indicate that the nature of use between Males and Females do not differ through the year.
![Story 4](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%204.png?raw=true)

### The Most Popular and Unpopular Stations
This visualisation highlights the most popular and unpopular stations in Jersey City (based on the dataset). The map overlays the 2018 Per Capita Income deliniated by Zip Code. Overall, it would appear that the majority of Citi Bike stations are concentrated closer to the Holland Tunnel connecting Jersey City to Manhattan Island. This, in conjunction to the per capita income concentrated in this area of Jersey City, it can be inferred that the users of the Citi Bikes are using the service to commute to work. Additionally, the most popular station is Grove St which is also in close proximity to the Grove Street station.
![Story 5](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%205.png?raw=true)

### Route Map
From the above, this visualisation demonstrates some of the routes taken from each station. You can view the trips month on month in addition to by season.
![Story 6](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%206.png?raw=true)

### Gender and User Type
All gender categories tend to follow the same trend in terms of usage of the Citi Bike. Males definitely use the service more than Females. However, the average time spent per trip is higher with Females compared to Males.

Across all three gender categories, it would appear that the 'Customer' category of users tend to take longer trips across all months than 'Subscribers'. This could be due to 'Customers' using the service as tourists as opposed to 'Subscribers' who would presumably be residents of the area. This could support the above theory that the shorter commutes could be a result of users taking the service to work.
![Story 7](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%207.png?raw=true)

### Age and Average Trip Duration
At first glance, it would appear that the service is dominated primarily by older users. Given the nature of the commutes however, this seems unlikely. The inference here is that there is likely inaccurate information being captured by the system perhaps as a result of users being concerned about their privacy. This is further supported by there being a number of users above the age of 90.
![Story 8](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%208.png?raw=true)

### Most Used Bikes - Repair / Replacement Planning
This visualisation aims to illutsrate which bike IDs are most used. The size of each bike ID is determined by the average trip duration and the color of the cell indicating the total number of hours on the bike. With further analysis, it would be possible to ascertain where these frequently hired bikes originate from and determine whether they are used in high traffic areas (e.g. by Tourists). If so, we can perhaps identify strategies which can be implemented to better maintain this fleet of bikes.
![Story 9](https://github.com/EpicTomatoSauce/citibike_analysis/blob/main/Images/Story%209.png?raw=true)

## Deployment to Tableau Public:
Our analysis has been having issues with its deployment to Tableau Public. It intermittently seems to be available here - [Click Me](https://public.tableau.com/app/profile/matt.vella/viz/CitiBikeSystemAnalysis/CitiBikeAnalysis)

Packaged workbook is available for download [here](https://drive.google.com/file/d/1kCFszrZY-wVOyYpHH-zlzRrhBHfELSbZ/view?usp=sharing).

## Contributors
- [@Matt](https://github.com/EpicTomatoSauce)