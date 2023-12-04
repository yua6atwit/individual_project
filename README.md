# Boston Crime Data Analysis

## Introduction
Criminal activity can happen anywhere and anytime. It is not only important for residents to know to avoid areas where criminal activity is high, but also for people planning to move to a different district to understand the possibility of crimes in that area. Police can also use this information to prevent criminal activity. In this project, I will be analyizing trends and areas at a higher risk of criminal activity.
  1. Which (top 10) districts are crimes most likely to occur?
  2. Does the number of crimes decrease or increase depending on the month? Day of the week?
  3. What are the top 10 most common crimes?

## Data Selection
The dataset is from Kaggle[1] and has 2 datasets: 
One has the name of the specific crime and the offense code.
The other has over 300,000 rows of crimes in Boston with 17 columns:
- Incident Number
- Offense Code
- Offense Code Group (name of crime group)
- Offense Description
- District
- Reporting Area
- Shooting
- Occured On Date
- Year
- Month
- Day Of The Week
- Hour (0 to 23)
- UCR Part
- Street
- Latitude
- Longitude
- Location

In the column for districts 1,765 rows are missing data. This will be dropped because it is only .55% of all the data.


## Methods
Tools: 
- Numpy and Pandas for data analysis
- Matplotlib for data visualization

Methods used with Numpy
- Functions: array, sum 

Methods used with Pandas
- Functions: DataFrames, Series
 
Methods used with Matplotlib:
- Functions: pyplot
- Bar graphs are useful for comparing different groups or to determine changes over time. Typically one axis show the groups and another shows the numeric value.


## References
[1] [Boston, Analyze. “Crimes in Boston.” Kaggle, 4 Sept. 2018, www.kaggle.com/datasets/AnalyzeBoston/crimes-in-boston.] 
