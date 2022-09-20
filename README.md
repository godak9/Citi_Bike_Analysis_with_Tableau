# Citi_Bike_Analysis_with_Tableau
## Overview 
### Purpose
Citi Bike it the largest bike sharing program in the US located in New York City. The goal of this project was to use Citi Bike trip data to determine if estabilishing a Citi Bike program in Des Moines would be worthwhile for investors. Data trip was gathered from the Citi Bike System Data page which links to an [index of trip data](https://s3.amazonaws.com/tripdata/index.html). The data used for this analysis is from August 2019 trips and can be found in the index under the label "201908-citibike-tripdata.csv.zip". Data from August was used becasue there is likely more traffic during the summer.
### Analysis Roadmap 
Trip data was downloaded as a CSV file. Python and Pandas were used in Jupyter Notebook to create a dataframe from file and make an adjustment to the "tripduration" column. To make the data in the "tripduration" column useful for visualizations in Tableau, the *to_datetime()* function was used to convert the data from an integer to a datetime datatype so that the time was accessible in hours and minutes. Once converted, the dataframe was exported as a new CSV file which was then imported into Tableau for analysis. The code for this process can be found in the [Jupyter Notebook file](NYC_CitiBike_Challenge.ipynb) in this respository. 

Visualizations were then made in Tableau to create a story about:
- The length of time that bikes are checked out for all riders and genders 
- The number of bike trips for all riders and genders for each hour of each day of the week
- The number of bikes for each type of user and gender for each day of the week

The results of analysis are summarized below and the Tableau Story can be accessed [here](https://public.tableau.com/app/profile/gabrijela.odak/viz/NYCCitiBikeAnalysisforDesMoinesBusinessProposal/NYCCitiBikeAnalysis?publish=yes).
