# Metis_EDA_Project
Varsha Garla

# Socioeconomic Status and MTA Ridership Decline during Peak Months of COVID-19

## Abstract
The goal of this project was to use exploratory data techniques to consider whether MTA ridership declined uniformly across all neighborhoods over the peak months
of the COVID-19 pandemic, or if ridership declined differently relative to the socioeconomic status of the neighborhood. I worked with [MTA turnstile data](http://web.mta.info/developers/turnstile.html)
and [Median Household Income data](https://www.psc.isr.umich.edu/dis/census/Features/tract2zip/) provided by the University of Michigan Population Studies Center.
I analyzed the change in subway usage of stations aggregated into income bracket groups based on the median income of that station's zip code.

## Design
This project utilizes MTA turnstile data from March, April, and May 2020 as a means of viewing the traffic through every subway station in the MTA. 
Understanding whether subway ridership declined more in low-income areas vs. high-income areas would allow the NY Department of Health to provide resources to the
communities with highest subway usage, in an effort to minimize subway usage and increase social distancing in order to lower the risk of spreading COVID-19. 
It may also shed light on health disparities due to socioeconomic factors.

## Algorithms

_Data Aggregation_
After cleaning the turnstile data, I calculated the daily entries into every station over the 3 month period (March, April, and May 2020). I then aggregated
the stations into income bracket bins according to the median incomes associated with their zip codes.

_Analysis_
I calculated one percent decline of subway usage value per every income bracket group using the total initial entries into all stations in a bin on March 2, 2020
and the total final entries of all stations in the bin on May 25,2020. Additionally, I calculated the daily percent decline from the initial entries on March 
2, 2020 for all stations, and aggregated them by income bracket group, so that this could be viewed over time.

## Tools
* SQL and SQLAlchemy for data organizing and accessing
* Numpy and Pandas for data manipulation
* Matplotlib and Seaborn for plotting

## Communication
Slides and visualizations summarizing project can be found in this repository.

![EDA_bar_chart](https://user-images.githubusercontent.com/87044440/126789450-c24504c8-1d02-4ea6-a959-22f0e90acdc7.png)

![EDA_line_graph](https://user-images.githubusercontent.com/87044440/126789460-f13be131-3e98-42cb-aec2-202db196a4a2.png)



