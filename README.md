# MOTOR-VEHICLE-THEFT-ANALYSIS
![car theft](https://github.com/EsabellB15/MOTOR-VEHICLE-THEFT-ANALYSIS/assets/123163220/b3558ae1-c38e-4a07-8220-b2deffe06a3e)

## Introduction
This is a Power BI project from Maven Analytics on motor theft vehicle analysis.  I worked on this project to practice my skills in data cleaning, analysis, and visualization.

## Problem Statement
1.	What day of the week are vehicles most often and least often stolen?
2.	What types of vehicles are most often and least often stolen? Does this vary by region?
3.	What is the average age of the vehicles that are stolen? Does this vary based on the vehicle type?
4.	Which regions have the most and least number of stolen vehicles? What are the characteristics of the regions?

In summary, my objective is to find out when, where, and which vehicles are likely to be stolen.

## Power BI concepts applied:
-	DAX Concepts: Calculated column, custom column, Format (), Year(), Count().
-	DATA Modelling: Star Schema (*:1)

## Data Sourcing
I downloaded the CSV file from the Maven Analytics website and extracted it into Power BI for cleaning, analysis, and visualization.

It contains 3 sheets/tables:
1.	STOLEN_VEHICLES with 4,554 rows and 8 columns.
2.	MAKE_DETAILS with 139 rows and 3 columns.
3.	LOCATIONS with 17 rows and 5 columns.

## Data Transformation
Data was efficiently cleaned and transformed with the Power Query Editor of Power BI. 

Some of the applied steps included : 
-	Changed Date format from South Africa dd,mm,yyyy to United States M,D,YYYY
- Created a new column for the Day of the week vehicles are stolen and the name is DayofWeek
-	Created a new column YearStolen by extracting the year of the Date Stolen column to calculate the age of the vehicle to calculate the average age of the vehicles stolen.
-	Created a new column to calculate the sum of vehicles stolen.

![Data_cleaning](https://github.com/EsabellB15/MOTOR-VEHICLE-THEFT-ANALYSIS/assets/123163220/909c9b48-5a40-4e56-9d3e-48486892c4d1)

## Data Modelling
Power BI automatically connected related tables resulting in a star schema model. The 'stolen_vehicles' table is the fact table of the model. The remaining are two-dimension tables; the 'make_details' table and the 'Locations' table are connected to the 'stolen vehicles' table via the common columns: 'make_id and ‘location_id’ respectively.

![model view](https://github.com/EsabellB15/MOTOR-VEHICLE-THEFT-ANALYSIS/assets/123163220/0b659731-c853-4a19-81ec-f6501009af04)

## Data Analysis and Visuals

![MotorVechicletheft](https://github.com/EsabellB15/MOTOR-VEHICLE-THEFT-ANALYSIS/assets/123163220/f672cb82-05ce-4c0c-9b4d-6c96ed18c297)

- From the dashboard, it is observed that most vehicles are stolen on Sundays, and the least stolen on Fridays. 
- The top 3 most stolen vehicles are station wagons, Saloons, and Hatchbacks and the respective Top 3 Make_names of the most stolen vehicles are Toyota, Nissan, and Mazda.
-	From the Dashboard, we can find that most vehicles are stolen in Auckland and least stolen in the southland, of which Auckland has the highest population in New Zealand.

You can interact with this report [here](https://app.powerbi.com/groups/13bfa296-3bf8-4464-86eb-f48267f0fff7/reports/8b7ea864-c323-48f9-9eec-d7c787962628/ReportSection?redirectedFromSignup=1&experience=power-bi)

## Recommendations 
- Investigate reasons for the low theft rate in Southland and consider replicating successful practices in other regions.
- Evaluate the economic impact of vehicle theft based on the total value of stolen vehicles in 2021 and 2022.
- Encourage community members to be especially vigilant on Sundays, given the higher likelihood of vehicle theft. Remind them to double-check that vehicles are securely parked and encourage the use of additional security measures.





