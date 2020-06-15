# PyBer Analysis Report

## Background and Results

### Purpose
  The purpose of this analysis was to give the ride sharing company Pyber analysis of its ride data to improve its service to customers and grow its business.  
  
### Technical Analysis
  This required importingt raw data files into dataframes to be analyzed. Analysis on the dataframes included insuring the data was cleaned and merged, sorting and grouping the data by city type (Rural, Suburban, and Urban).  Descriptive statistics were computed for different ride data by city type.  Finally, graphic visuals of the data were generated using matplotlib.

### Results
Table 1: Summary of ride data by city type.
![Summary of ride data by city type](https://github.com/mauricio4337/PyBer-Analysis/blob/master/Analysis/summary_df.png)


Figure 1: Plot of Total Fares by city type.
![Plot of Total Fares](https://github.com/mauricio4337/PyBer-Analysis/blob/master/Analysis/Fig_Challenge.png)
### Summary
Analysis of Figure 1 shows a farely steady use of Pyber rides over time by each city type, with only minor changes in the fares collected up or down over time.  The disparity in total fares collected over time by city type is stark between Urban/Suburban areas and Rural areas.  Table 1 confirms this disparity also in both the number of rides taken and the number of drivers in Urban/Suburban areas versus Rural areas.

## Challenges Encountered and Overcome
I encountered the most challenges with manipulating the data by the type of data structure encountered.

### Challenges and Difficulties Encountered

* Programming:
Extracting/Inserting data into series and dataframes efficiently. Finding and applying the correct syntax for the method needed.
* Data analysis:
Once the correct method was selected with the correct syntax the data analysis was very straight forward.
* Graphing, etc:
Generating graphical analysis was fairly straight forward, although many customizations are available that leave a number of details left to be discovered.
### Technical Analyses Used
Data was grouped by city type using the groupby() method. Sum, count, and summary statistic methods were added to this to compute the total rides, the total number of drivers, the mean fare per ride and per driver for each city type.  Matplotlib was used to generate a variety of chart types both in the module work and in the challenge for Pyber to use for abalysis.  Chart types included line plots, scatter plots, bar charts, box-whisker plots, bubble charts, and pie charts.  Each chart was formatted to include proper titles, axes labels, scales, legends (if applicable), and notes if needed.  Each figure generated was saved to a file in the analysis folder.   
## Recommendations and Next Steps
Pyber should investigate the underlying causes of this disparity since the Table 1 indicates that average fare per ride and per driver are higher in Rural areas.  It should be determined if customers would increase their use of the service if more drivers were available.  
### Recommendations for Future Analysis
To help identify satisfaction with Pyber's service, Pyber should collect driver and ride ratings. Length ride and wait times might also be collected.
### Additional Analysis 1
Collect a simple rating (0 - 5 stars) for each driver. A driver id would also need to be assigned.
* Description of Approach
Get the mean rating for each driver and the mean rating for drivers by city type.
* Technical Steps
Once the rating has been added to the complete dataframe, the driver ratings can be grouped by city type and summary statistics can be applied to the driver ratings.  Box-whisker plots can be generated from this data to determine how consistent driver service is by city type. The mean driver rating by city type would indicate which area has the best drivers in general.  The spread of the data in the box-whisker plot would tell you which city type has the most predictable driver rating.  
### Additional Analysis 2
Collect a simple rating (0 - 5 stars) for each ride.
* Description of Approach
Determine rating for each ride by city type.
* Technical Steps
Once the rating has been added to the complete dataframe, the ride ratings can be grouped by city type and summary statistics can be applied to the driver ratings.  Box-whisker plots can be generated from this data to determine how consistent ride service is by city type. The mean ride rating by city type would indicate which area recieves the best service in general.  The spread of the data in the box-whisker plot would tell you which city type has the most predictable predictable service.  A line plot or scatter plot could be used to check if any correlation exist between ride rating and driver rating both by city type and overall.  A line plot or scatter plot could be used to check if any correlation exist between the ride rating and the ride fare.
