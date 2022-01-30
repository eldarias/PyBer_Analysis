# Ride-sharing Analysis

## Project Overview
The purpose of this project was to perform a new analysis on the city and ride datasets provided.  For this challenge, I used Jupyter Notebook and Pandas to inspect and merge data, perform mathematical calculations as well as create data series and DataFrame.  In addition, the matplotlib library was used visualize the data via charts.  The overall goal of the ride-sharing app company is to help improve access to ride sharing services and determine affordability.

## Technical Notes

### Deliverable 1
The goal for this deliverable was to create a ride-sharing summary by city type.  For this deliverable, the raw data was merged into a DataFrame, then summarized into series using functions/methods such as _groupby()_, _count()_, and _sum()_.  The series included total riders, total drivers and average fare for each city type.  The new series were then summarized into a new DataFrame, formatted and displayed for visualization as shown in the results below.

### Deliverable 2
The goal for this deliverable was to create a multiple-line chart of total fares for each city type.  For this deliverable, the **fare**, **type** and **date** columns/data were extracted from the merged DataFrame (from Deliverable 1) and added to a new DataFrame.  The index was reset then a pivot table DataFrame was created.  Other functions were used, such as _.loc()_, _to datetime()_, _.index()_and _resample()_ to extract only the required records, reset index, format dates and summarize based on dates.  Finally, the data was visualized via a multiple line plot chart using the object-oriented interface method, see the results section below..

## Results
Below are the results from the analysis:

- <image src="./analysis/Deliverable1_Pyber_Summary_DataFrame.png">
From the above results, I can conclude that the Rural cities have less rides, less drivers and the average fare per ride and per driver are more expensive compared to the Suburban and Urban cities.  Urban cities have more rides, more drivers and the average fare per ride and driver are cheaper/less.  It can also be said that although the number for drivers for the Rural cities is much lower, on average, the drivers have a higher number of rides compared to Urban cities.


- <image src="./analysis/PyBer_fare_summary.png">
The plot chart above depicts the total fare by city type for the months of January through April.  Here we can see that the total fare by city type follow a similar pattern for all three city types.  There is a fare increase for Urban and Suburban cities that begins early January and goes until around end of February, then it seems to fluctuate around March.  For Rural cities, the fare amount is much lower, it seems that there are random spikes in the total fares, but they don't remain steady.


## Summary
In summary, we can see that Rural cities have higher average fare per ride and per driver, which could make the ride sharing service less affordable.  Also, as the number of rides increate, there are more drivers, the total fares increase and the ride sharing service seems more affordable.  If one of the goals of the ride sharing service is to make the service more affordable, higher presence may be needed for rural and suburban cities.  Another important item to note is the total drivers to total rides ratio, which is important to understand specifically for company expenses/profits.  There is more data required to be able to determine if higher presence is possible and if it would be profitable to the company.  For example, the population would be needed to see if higher presence is possible.  The distance and expense per ride would also be beneficial to analyze and compare the distance and expenses for the city types to make proper conclusions.