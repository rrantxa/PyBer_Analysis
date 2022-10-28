# PyBer Analysis
## Overview of the analysis:
### Purpose
The purpose of the PyBer Analysis was to review the data concerning "PyBer", a ride-sharing app. In order to analyze the zones that are currently underserved by the application, we had to look at the data related to the number of drivers, number of rides and average fares by city type (Urban, Suburban, and Rural). 

After carefully reviewing the information, this final analysis reviews, specifically, the ride-sharing data by city type, as well as the weekly fares by city type for the period that covers January to April of 2019. 

## Results: 

As stated earlier, for this analysis we had to work with the ride-sharing data provided by PyBer. After loading the two initial databases into two Pandas DataFrames and then merging them into one single DataFrame called "pyber_data_df", we started our analysis: 

#### Total Rides by City

Using our merged DataFrame, as well as the "groupby" and "count" functions, we discovered that the total ride distribution by city type was as follows: 

![1](https://user-images.githubusercontent.com/113153777/198699681-64b9caaf-e979-4f6c-82b8-17645c3ad4f4.png)

What we can clearly observe through this calculation is that Rural and Suburban cities have a much lower ride count than Urban cities. Rural cities get less than 10 times the amount of rides that Urban cities have, while Suburban cities get less than half of the rides that Urban cities get. 

#### Total Driver Count

To get out total driver count by city type, we continued to use the "groupby" function. We also used the "sum" function to help us calculate the total amount. The resulting sum gave us the following Series: 

![2](https://user-images.githubusercontent.com/113153777/198700903-15b0ead3-720d-4df5-bfc6-370b49c36a0c.png)

As suspected, Urban cities have the biggest driver count, while Suburban and Rural cities have far lower driver counts. 

#### Total Fares

To calculate the total fares by city type, we used the "groupby" and "sum" functions once again, getting the following result: 

![3](https://user-images.githubusercontent.com/113153777/198701314-db5e0599-f126-4c42-ac8b-66f2687e2ff8.png)

Considering our total amount of rides and drivers according to the city type, it makes sense that Urban cities have the biggest fare sum. The second spot is, again, held by Suburban cities, while Rural cities have the lowest total fare sum. 

#### Average Fare per Ride

In order to get the average fare per ride, we had to do a simple division using the variables we had already created for the "Total Fares" and "Ride Count". The results were as folows: 

![4](https://user-images.githubusercontent.com/113153777/198702305-ef9e1c60-600e-4118-8ff2-27c9c3c8de74.png)

Now, though the analysis of previous variables might make us infer that Urban cities would have the highest fares per ride, our analysis actually demonstrates that it is the complete opposite. However, if we take into account that Suburban and Rural Cities have a lower ride demand (See: Total Rides by City") the elevated prices make sense. 

#### Average Fare per Driver

To calculate the average fare per driver, we used a very similar formula to the previous one. Nevertheless, instead of dividing the total fares by the ride count, we divided them by the total driver count. The resulting Series gave us the following numbers: 

![5](https://user-images.githubusercontent.com/113153777/198703271-784cbfd0-97c8-496c-8527-099971537047.png)

These results follow the same trend as before, showing that Rural Cities have a much higher Average Fare per Driver than Suburban and Urban Cities. This, again, makes sense if we take into account the extremely low amount of drivers that Rural cities have compared to Suburban and Urban Cities. 

#### Data Summary

Finally, we constructed a Summary DataFrame for our analysis, where we could clearly inspect the data trends: 

![6](https://user-images.githubusercontent.com/113153777/198706109-f134e3a5-0a43-4854-a562-b1fd50b3b170.png)

## Summary: 
### Subheading
Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.
