# Divvy Bike Share
## Business Task: 
Explain how annual members and casual riders use Divvy bikes differently.

## Data Sources Used:
* Divvy 2019 Q1
* Divvy 2020 Q1

The data used was made available by Motivate International under their Data License Agreement.
This data has been made public to allow us to explore how different customer types use Divvy bikes.
Data privacy laws protect the personally identifiable information of all riders.

## Cleaning and Manipulation of Data
* Column created for ride_length, calculated by subtracting ride start time from ride end time. Data was formatted using the HH:MM:SS time format.
* Column created for day_of_week, calculated by calling the WEEKDAY command using 1 = Sunday and 7 = Saturday.
* Data was exported to be used in R Studio.
* Column names for Divvy_Trips_2019_Q1 were changed to match that of Divvy_Trips_2020_Q1.
* Column data types were converted to allow for data to be consolidated between 2019 Q1 data nd 2020 Q1 data.
* Dropped unneeded data from the combined data frame, including columns start_lat, start_lng, end_lat, end_lng, birthyear, gender, and tripduration.
* Reassigned the present values of Subscriber and Customer from the member_casual column to match the member and casual values to match updated formatting.
* Created a new column to store the date of the start of the ride.
* Created additional columns to store the individual values for the month, day, and year.
* The day_of_week column was changed to contain the string for the day of the week, no longer storing an integer to represent the day.
* A file was exported containing the mean ride_length data per day of the week for each member_casual group.

## Summary of Analysis



## Visualizations




## Recommendations:
* asd
* asd
* asd
