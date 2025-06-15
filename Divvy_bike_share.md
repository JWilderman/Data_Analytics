# Divvy Bike Share
## Business Task: 
Explain how annual members and casual riders use Divvy bikes differently.

## Data Sources Used:
* Divvy 2019 Q1
* Divvy 2020 Q1

The data used was made available by Motivate International under their Data License Agreement.
This data has been made public to allow us to explore how different customer types use Divvy bikes.
Data privacy laws protect the personally identifiable information of all riders.

## Cleaning and Manipulation of Data:
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

## Summary of Observations:
For the median ride length, Members averaged 13.7 minutes per ride. Casuals averaged 91.31 minutes per ride. 
The daily median ride length shows a steady line for Member ride length throughout the week. See figure 1 in Visualizations for reference.
Casual ride length starts at a slow decline at the beginning of the week, with a large spike occurring on Thursdays, then returning to normal ride length over the next 3 days of the week. See figure 1 in Visualizations for reference.

Members ride frequently during the weekdays. See figure 2 in Visualizations for reference.
The number of casual riders drops at the start of the work week and starts to increase as the work week comes to a close. See figure 2 in Visualizations for reference.

During Q1 of 2019 and Q1 of 2020, member rides maintained over 340 thousand. See figure 3 in Visualizations for reference.
During Q1 of 2019, there were fewer than 25 thousand casual rides. In Q1 of 2020, we see this value almost doubling, increasing to 44 thousand casual rides. See figure 3 in Visualizations for reference.

Members ride more frequently at hours between 6 am to 9 am and 4 pm to 6 pm. See figure 4 in Visualizations for reference.
Casual users ride more frequently between the hours of 11 am to 5 pm. See figure 4 in Visualizations for reference.

## Visualizations:
Figure 1:

![image](https://github.com/user-attachments/assets/1a26805d-8312-43c1-abcc-0798a5c7b30f)

Figure 2:

![image](https://github.com/user-attachments/assets/fcf6eb9a-472e-46b6-b782-f26072901cfe)

Figure 3:

![image](https://github.com/user-attachments/assets/31b6d5c6-f309-4515-aad6-99c69de01cf0)

Figure 4:

![image](https://github.com/user-attachments/assets/f0502a93-b830-4a42-805a-557428ee8973)


## Analysis of Data:
Members of Divvy appear to prefer shorter ride lengths than casual users, but they ride frequently throughout the entire work week. Members likely use Divvy bikes as transportation to commute to and from work. This would explain consistently shorter ride times throughout the week, with slight shifts occurring on the weekends. 

Casual users of Divvy prefer longer ride lengths, but ride more infrequently than members do. Casual users appear to use Divvy bikes for longer activities such as sightseeing, running errands, or leisure purposes.

## Recommendations:
1. With casual Divvy users preferring to ride less frequently with longer ride times, casual users would be more likely to become members if members were given lower rates on rides exceeding a specified ride time. With a discounted rate offered on longer rides, it can turn even infrequent Divvy users into subscribers due to the savings that are offered.
2. If members were offered discounts during slower hours, such as between 12 pm to 3 pm, casual users would be incentivised to become members since more of their hours of use fall in that period.
3. Offering incentives for use during the weekends for members might be another method that Divvy could use to try to get more casual users to become members, as well as increasing usage by current members.
