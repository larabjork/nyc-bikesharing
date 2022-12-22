# New York Citi Bike Data
Data Bootcamp week 15 - Tableau

## Overview of Analysis
This exercise involved analyzing data from a provided csv file using Tableau Public. The data represents information about New York City's bikesharing program (Citi Bike), and we were asked to use this data to help make a case for replicating this program in Des Moines, Iowa.

For the guided homework portion of the exercise, I produced multiple data visualizations of different types and combined four of them in a Tableau Dashboard.

For the independent challenge portion of the exercise, I:

* Used Python and Pandas to convert tripduration data from an integer to a dateime datatype (i.e., turning it into a time with hours, minutes, and seconds);
* Created five additional visualizations; and
* Compiled selected visualizations from the homework and the independent challenge into a Tableau Story.

## Results
The first deliverable for the challenge was the conversion of tripduration data to datetime format, as shown in [this Jupyter notebook](https://github.com/larabjork/nyc-bikesharing/blob/main/NYC_CitiBike_Challenge.ipynb) and [the resulting csv](https://github.com/larabjork/nyc-bikesharing/blob/main/201908_citibikes_converted_duration.csv).

The following visualizations are all available at [my Tableau Public profile](https://public.tableau.com/app/profile/larabjork/viz/citibike-challenge_16713902175970/NewYorksCitiBikes?publish=yes), in Tableau Story form.

### Basic Information from Guided Homework
In my Tableau Story, I started with three visualizations from the guided homework, because they help set the context for total Citi Bike use and basic demographics about users.

#### Number of Rides
![Number of rides in August 2019: 2,344,224](https://github.com/larabjork/nyc-bikesharing/blob/main/images/number_of_rides_total.png)
This shows the total number of rides (aka the number of times Citi Bikes were checked out) in August 2019.

#### Customers vs Subscribers
![Pie chart showing percentage of subscribers versus customers](https://github.com/larabjork/nyc-bikesharing/blob/main/images/customer_v_subscriber.png)
This pie chart shows that most of the rides in August were taken by subscribers, rather than pay-as-you-go "customers".

#### Gender Breakdown
![Pie chart showing percentages of riders in August 2019 in these categories: female, male, unknown](https://github.com/larabjork/nyc-bikesharing/blob/main/images/gender_breakdown.png)
This pie chart shows that most of the rides in August were taken by male riders, followed by female riders, and then riders of unknown gender. The dataset did not provide more information about how these outdated/problematic gender categories were defined for users.

### August Peak Hours
![Horizontal bar chart with number of rides on x axis and hour of the day on y axis](https://github.com/larabjork/nyc-bikesharing/blob/main/images/august_peak_hours.png)
This bar chart was also part of the guided homework and is included to help set the context for the more detailed looks into peak riding times to come. It shows that the highest-use times are roughly around commute hours and the lowest-use times are from midnight to 6 AM.

### Checkout Times by Hour
![Line chart that shows trip duration by hour (x-axis) versus number of bikes (y-axis)](https://github.com/larabjork/nyc-bikesharing/blob/main/images/checkout_times_users.png)
This line graph allows the user to filter by hour to show the number of bikes that were checked out at a given time. The longest checkout times occurred from midnight to 4 AM.

### Checkout Times by Gender
![Line chart that shows trip duration by hour (x-axis) versus number of bikes (y-axis), by gender](https://github.com/larabjork/nyc-bikesharing/blob/main/images/checkout_times_by_hour_by_gender.png)
Like the previous line graph, this allows the user to filter by hour to show the number of bikes that were checked out at a given time, but also by gender. It shows that female riders generally take shorter rides that male riders and riders of unknown gender.

### Trips by Weekday per Hour
![Heat map that shows start/stop times for all riders by day of the week](https://github.com/larabjork/nyc-bikesharing/blob/main/images/trips_by_weekday_per_hour.png)
This heat map show that, for all riders, the busiest hours of the day for weekdays are more dramatic than for the weekends. 

### Trips by Weekday per Hour by Gender
![Three heat maps, by gender, that show start/stop times for riders by day of the week](https://github.com/larabjork/nyc-bikesharing/blob/main/images/trips_by_gender_weekday_per_hour.png)
These heat maps show that start and stop times  for female and male riders follow largely the same pattern, albeit with less intensity among female riders. RIders of unknown gender show a similar but less discernible pattern.

### User Trips by Gender and User Type
![Heat map showing intensity of ridership, split by gender and user type](https://github.com/larabjork/nyc-bikesharing/blob/main/images/trips_by_gender_customer_type_weekday.png)
This heat maps shows that ridership for pay-per-use riders ("customers") has little difference by gender across day of the week, with some increased use on weekends. For subscribers, the gendered pattern of the previous visualization continues: male riders with highest use, especialy on Thursdays, female riders with a similar but less intense use, and riders of unknown gender without a clear pattern of use by day of the week.

## Summary
* high level summary 
* two additional viz for future analysis