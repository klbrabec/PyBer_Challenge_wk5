# Pyber Analysis 

## Overview of Analysis 
### Purpose 
The scope of this project is to review and create a DataFrame that contains ride sharing details by city type (Urban, Suburban, Rural).  The goal is to visualize the number of rides and the average fares for each city type.   The results of this analysis will assist the Pyber organization to determine where to focus marketing efforts, hiring strategies, and other organizational priorities.  

### Data 
The foundational data in this project comes from two datasets: 
- city_data.csv - This dataset contains city type designations and the number of drivers in each city 
- ride_data.csv - This dataset contains city, ride date, and fare amount

Data was merged into a single dataset using the city name as the unique value to link the datasets together.  2375 records are in the merged dataset.

![Merged_Dataset](https://github.com/klbrabec/PyBer_Challenge_wk5/blob/main/Resources/merged_dataset.png)

Note:  Assumptions were made on null values and duplicates in the merged dataset due to the types of data being used. 
- Duplicates are unlikely for date/time values. 
- Rides will only have one city type value assigned. 
- Cities may have multiple rides
- Dates may have multiple rides 

## Results
The summary details for the merged dataset are below: 
![Summary_Table](https://github.com/klbrabec/PyBer_Challenge_wk5/blob/main/Resources/summary_table.png)

### Results summary
- Rides 
    -- The majority of rides occurred in cities in the Urban designation.  
- Drivers 
    -- The majority of drivers are in cities in the Urban designation 
- Total Fares
    -- The highest level of total fares are from cities in the Urban designation
- Average Fare per Ride 
    -- The highest average fare per ride are in cities in the Rural designation
- Average Fare per Driver 
    -- The highest average fare per driver are in cities in the Rural Designation 

### Fares by City Type 
The plot above below the fares by city type over a four month period.   
![Fig1.png](https://github.com/klbrabec/PyBer_Challenge_wk5/blob/main/analysis/Fig1.png)


## Summary and Recommendations 
### Urban Average Fare per Driver Improvements 
The data reviewed as part of this analysis shows that ride share usage in Urban areas is currently healthy, but can be improved on, not only for Pyber, but for the individual drivers that participate in the program.   For urban drivers, the average fare per driver is $16.57.  This is due to two factors, ride length and total number of driveres.  Due to the geographical nature of urban areas, it is not feasible to extend ride length (and fare amount), however there is a much higher percentage of drivers than total rides taken during the study period.  Currently, there are approximately 32% more drivers than rides taken.  If inactive drivers are removed from the service, this will increase the average fare per driver. Further studies should be conducted to determine how many drivers are only active during 'surge' periods, and how many are active on a regular basis. 

### Rural Average Fare per Ride 
Average fare per ride and average fare per driver are higher in rural areas.  This is most likely due to the fact that there is greater distance between points in a rural setting, resulting in longer rides and higher fares.  in order to grow this market, it is recommended that additional drivers are hired (or perhaps transferred from urban areas).  This will provide more rides to people living in rural areas.  Additionally, people living in rural areas may not be aware that the Pyber service is available to them.  Increased marketing efforts in this area will inform people about the ride service.  It may also be beneficial to coordinate with local social service organizations to provide discounted rides for people to appointments as a significant amount of people may not have other transportation options.  

### Surge Pricing 
Looking at the plot of fares, it appears that in late February and throughout March there are peaks of ride usage.  Because there are surges in usage, it is recommended that 'surge' pricing (increased pricing for high use time periods) be considered.  This change would benefit drivers working during high use time periods, as well as encourage additional drivers to join Pyber to participate in the program.  These programs would want to be considered carefully as mentioned above, a high number of inactive drivers drives down the average fare per driver and could be a negative to particpation.  
 
