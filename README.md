# Citi_Bike_Analysis_with_Tableau
## Overview 
### Purpose
Citi Bike it the largest bike sharing program in the US located in New York City. The goal of this project was to use NYC Citi Bike trip data to determine if estabilishing a Citi Bike program in Des Moines would be worthwhile for investors. Data trip was gathered from the Citi Bike System Data page which links to an [index of trip data](https://s3.amazonaws.com/tripdata/index.html). The data used for this analysis is from August 2019 trips and can be found in the index under the label "201908-citibike-tripdata.csv.zip". Data from August was used becasue there is likely more traffic during the summer.
### Analysis Roadmap 
Trip data was downloaded as a CSV file. Python and Pandas were used in Jupyter Notebook to create a dataframe from file and make an adjustment to the "tripduration" column. To make the data in the "tripduration" column useful for visualizations in Tableau, the *to_datetime()* function was used to convert the data from an integer to a datetime datatype so that the time was accessible in hours and minutes. Once converted, the dataframe was exported as a new CSV file which was then imported into Tableau for analysis. The code for this process can be found in the [Jupyter Notebook file](NYC_CitiBike_Challenge.ipynb) in this respository. 

Visualizations were then made in Tableau to create a story about:
- The length of time that bikes are checked out for all riders and genders 
- The number of bike trips for all riders and genders for each hour of each day of the week
- The number of bikes for each type of user and gender for each day of the week
### Link to Tableau Story 
The Tableau Story can be accessed [here](https://public.tableau.com/app/profile/gabrijela.odak/viz/NYCCitiBikeAnalysisforDesMoinesBusinessProposal/NYCCitiBikeAnalysis?publish=yes). Below is a summary of the results in this story. 
## Results
Seven visualizaitons were created using NYC Citi Bike trip data. Below is a screenshot of each worksheet used to create each visualization complied into a Tableau story. This section only reports the results with a breif summary. In the summary section below, a conclusion is made based on the results as well as suggestions for two visuals that may further support the conclusion.
### Checkout Times for Users
The overwhelming majority of trips lasted less than 15 minutes. 

![Screen Shot 2022-09-20 at 2 43 26 PM](https://user-images.githubusercontent.com/104794100/191342004-a8e8b4b2-ea1e-46d6-ba00-58868b95f295.png)

### Gender Breakdown of Users
Even if all unknown users were females, the majority of users are males.

![Screen Shot 2022-09-20 at 2 46 48 PM](https://user-images.githubusercontent.com/104794100/191342155-fa7a6874-b0e3-441d-ae27-c8d9fb38213a.png)

### Checkout Times by Gender
Even if all unknown users were females, males tend to use the bikes for longer periods of time.

![Screen Shot 2022-09-20 at 2 43 47 PM](https://user-images.githubusercontent.com/104794100/191342382-7d5b68b5-d7b4-4419-9331-0c70a7e435e0.png)

### Trips by Weekday per Hour
During the *weekdays*, trips were more likely to be taken *before 9 am or after 5 pm*. During the *weekends*, trips were more likely to be taken *between 9 am and 5 pm*.

![Screen Shot 2022-09-20 at 2 44 04 PM](https://user-images.githubusercontent.com/104794100/191342988-346d9b7a-4be6-4b5c-a2b4-b37ea0556f4c.png)

### Trips by Gender (Weekday per Hour)
Males took more trips bewteen the hours of 9am and 5pm on weekdays.

![Screen Shot 2022-09-20 at 2 45 48 PM](https://user-images.githubusercontent.com/104794100/191342809-4caf0b74-5c29-4ff8-8de1-a822cfb857b7.png)

### Usertype Breakdown 
The majority of users are subscribers.

![Screen Shot 2022-09-20 at 2 46 31 PM](https://user-images.githubusercontent.com/104794100/191342888-50977c34-2c44-4788-a1c0-d5b79a58b31d.png)

### Usertype Trips by Gender per Weekday
Customers with an unknown gender used bikes more often than both known male and known female customers every day of the week. Male subscribers used bikes more often than female subscribers everyday of the week. Both female and male subscribers used bikes the most often on Thursdays.

![Screen Shot 2022-09-20 at 2 46 13 PM](https://user-images.githubusercontent.com/104794100/191342849-8aeb797e-f625-4bf5-8ead-bd4bdd60ac30.png)

## Summary
Based on the visualizations above, I summarize a conclusion below and make suggestions for two more visualizaitons that may support this conclusion. 
### Conclusion
Based on the type of users, the hours of use, and the trip duration, I think bikes are used most often for getting to work or coming home from work. The discepancy between male and female bike users may be becasue of the type of clothes males and females sterotypically wear to work, but this is only a speculation. If Des Moines has a population that lives relatively close to their place of work, say, close enough that a bike trip would only take them 15-20 minutes, I think investing in a Citi Bike program for the city would be a great idea. 
###Suggestions 
- Data is collected only on user type for NYC Citi Bike users. If data can be collected on the purpose a of use, a visual could be made to show the difference between the amount of users using bikes for work realted purposes versus users using bikes for recreational purposes. 
- An effort should be made to collect data on the Des Moines population for the purpose of seeing how near to work the population lives. This would be a good next step for investors to take to see if their target population is similar to the experimental population without implementing any sort of test run with a Citi Bike program within Des Moines.  




