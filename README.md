# Boston Crime Data Analysis

## Introduction
Criminal activity can happen anywhere and anytime. It is not only important for residents to know to avoid areas where criminal activity is high, but also for people planning to move to a different district to understand the possibility of crimes in that area. Police can also use this information to prevent criminal activity. In this project, I will be analyizing trends and determining areas at a higher risk of criminal activity.
  1. Which (top 10) districts are crimes most likely to occur?
  2. Does the number of crimes decrease or increase depending on the month? Day of the week?
  3. What are the top 10 most common crimes?

## Data Selection
The dataset is from Kaggle [1] and has records of crimes in Boston June 14, 2015 and continue to September 3, 2018. The source of these records were obtained from Analyze Boston which is run by the organization, Boston Police Department.
The other has over 300,000 rows of crimes in Boston with 17 columns:
- Incident Number
- Offense Code
- Offense Code Group
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

Data Preview:
![data screenshot](graph/Sample_Data.PNG)

In the column for districts 1,765 rows are missing data. Instead of dropping this data, it will be filled with 0 to represent an unknown district to account for any data loss.


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

## Results
1. Which (top 10) districts are crimes most likely to occur?
The data had 12 districts including the unknown district which was labeled 0. Only the top 10 were used for the bar graph:
![data screenshot](graph/Top_10_districts.png)
District B2 had the most crimes occurring in the span of 3 years with almost 50,000 crimes. The top 3 districts ranged between 50,000 and 40,000 while lowest in the graph ranged between 10,000 to 20,000. The two districts (A15, 0) not on the graph had lower than 10,000 crimes recorded. 


3. Does the number of crimes decrease or increase depending on the month? Day of the week?
Because the data stops on September 3, 2018, the data in these bar graphs is missing half the data from the year 2018 and may be skewed.
Interesting, there was not a noticeably large gap between the crimes occuring per day of the week.
Bar Graph:
![data screenshot](graph/Crimes_per_Week.png)
They all ranged in the 40,0000 to 50,000 number of crimes with Sunday having the lowest number of crimes.
In the crimes per month:
![data screenshot](graph/Crimes_per_Month.png)
There is a noticeable gap between the first few months of the year and June to August. Since only the months after August are affected by the incomplete dataset, the months before it are not affected and is not skewed. 

5. What are the top 10 most common crimes?
There were 222 different types of offense codes in the dataset and the top 10 common crimes are shown:
![data screenshot](graph/Top_10_Crimes.png)
In those 3 years, there were more crimes relating to a sick/injured person and investigating a person.

## Discussion

## References
[1] [Boston, Analyze. “Crimes in Boston.” Kaggle, 4 Sept. 2018, www.kaggle.com/datasets/AnalyzeBoston/crimes-in-boston.] 
