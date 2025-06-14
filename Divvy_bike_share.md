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
* Within Excel, ride_length unit was changed from seconds to minutes.

## Summary of Analysis
For the median ride length, Members averaged 13.7 minutes per ride. Casuals averaged 91.31 minutes per ride. 
The daily median ride length shows a steady line for Member ride length throughout the week. See figure 1 in Visualizations for reference.
Casual ride length starts at a slow decline at the beginning of the week, with a large spike occurring on Thursdays, then returning to normal ride length over the next 3 days of the week. See figure 1 in Visualizations for reference.

Members ride frequently during the weekdays. See figure 2 in Visualizations for reference.
The number of casual riders drops at the start of the work week and starts to increase as the work week comes to a close. See figure 2 in Visualizations for reference.

During Q1 of 2019, there were fewer than 1.5 million casual rides. In Q1 of 2020, we see this value triple to a bit over 4.5 million casual rides. See figure 3 in Visualizations for reference.
During Q1 of 2019 and Q1 of 2020, member rides maintained over 4.75 million. See figure 3 in Visualizations for reference.

## Visualizations
Figure 1:

![image](https://github.com/user-attachments/assets/1a26805d-8312-43c1-abcc-0798a5c7b30f)

Figure 2:

![image](https://github.com/user-attachments/assets/dae33708-8850-4e4e-8e0b-c4a6a449e55c)

Figure 3:

![image](https://github.com/user-attachments/assets/8a130b7e-c372-4305-aeb8-348964aea839)


## Recommendations:
* asd
* asd
* asd
