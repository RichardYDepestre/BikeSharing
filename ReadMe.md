# Module 14 Challenge - Bike Sharing Analysis

## Project Overview

Use Pandas to change the "tripduration" column from an integer to a datetime datatype.
The converted datatype will be used to  create a set of visualizations to:

1) Show the length of time that bikes are checked out for all riders and genders,
2) Show the number of bike trips for all riders and genders for each hour of each day of the week,
3) Show the number of bike trips for each type of user and gender for each day of the week.

## Resources

Software:       Visual Studio Code Version: 1.56.2, Tableau Desktop (Public Edition): 2021.1.1
Files:          NYC_CitiBike_Challenge_starter_code.ipynb,
                201908-citibike-tripdata.csv

## Data Preparation and Manipulation

We used the pandas library and created a DataFrame from the 201908-citibike-trip data file. Then, we checked \
the datatypes of the columns in the newly created dataframe ["Dataframe column data tyes"](..\\resources\\images\\citibike_df.png). \
The dataframe was manipulated and the column 'tripduration' data type changed to datetime. \
["Integer to date time conversion"](..\\resources\\images\\citibike_inttodt.png)
Through out the manipulation we checked the datatypes of the columns and made sure that they were per requirements. \
Finally, we confned and saved all the changes above to the dataframe onto a new CSV file without the index. \
["Index-less dataframe"](..\\resources\\citibike_df_less_index.csv).

## Data Analysis

In Tableau, we imported the dataset: citibike_df_less_index.csv, from the previous step, and created visualizations that show: \

- Checkout Times for Users and by Gender
  These charts show a correlation between trip duration and number of bicycles that get checked out. For instance, for short trips, ~5 minute, 145K+ bicycles get checked out. Their users travel short distances. The data also shows that of the genders, identified, male check out 100+K bikes whereas females, for the same trip duration, account less that 40K bikes.
- Trips by weekday for each hour and by Gender
  The data also reveals that bike utilization, during a week-day within 24 hours, is high in the morning and the evening. Trips are taken within 8:00 AM neighbours the 30+k with an increase on Thursdays. Between 17:00 and 18:00 there is a higher number of trip taken, with Thurdays showing heavier that other weekdays.
  When the same data is filtered by gender, male bike riders outnumber the other categories.
- Trips by Gender and by Weekday.
  This chart corroborates that males take more trip that females and unknowns and maintain a subscription to the service.

From the dataset we can infer that male subscribers are steady users of the bike riding service. Their utilization of the service peak in the morning and afternoon of weekdays. We noticed that Thurdays are busy for both male and female riders.

[checkout-times-by-gender](..\\resources\images\\check-out-times_genders.png) \
[check-out-times_users](..\\resources\\images\\check-out-times_users.png) \
[heat-map_user-trips-by-gender](..\\resources\\images\\../resources/images/heat-map_user-trips-by-gender.png) \
[trip-by-gender-week-day-per-hour](..\\resources\\images\\trip-by-gender_week-day-per-hour.png) \
[trip-by-weekday-hours](..\\resources\\images\\trip-by-weekday_hours.png)
