# bikesharing
For learning Tableau from Module 14

## Project Overview
The purpose of this task is to convince investors that a bike-sharing program in Des Moines is a solid business proposal. To solidify the proposal, one of the key stakeholders would like to see a bike trip analysis.
Following Analysis will be made with the citibike trip data from Newyork City
1. Length of time that bikes are checked out for all riders and genders
2. Number of bike trips for all riders and genders for each hour of each day of the week
3. Number of bike trips for each type of user and gender for each day of the week.
4. Add these new visualizations to the two you created in this module for your final presentation and analysis to pitch to investors.

## Resources
- jupyter notebook, python, Visual Code
- 201908-citibike-tripdata.csv
## Challenge Overview
Prerequisite:
1.  Download the NYC_CitiBike_Challenge_starter_code.ipynb


## Deliverable 1:  Change Trip Duration to a Datetime Format

Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

1. Download the NYC_CitiBike_Challenge_starter_code.ipynb file into your bikesharing folder, and rename it NYC_Citibike_Challenge.ipynb.
2. reate a DataFrame from the 201908-citibike-tripdata.csv file.
3. Check the datatypes of each column in the DataFrame.
4. Convert the "tripduration" column to a datetime datatype by passing the DataFrame column and the units inside the to_datetime() function.
5. Check the datatypes of the DataFrame.
	The conversion of the trip duration column to a datetime object.
6. Export the DataFrame as a new CSV file without the index column. Use this new CSV file for Deliverable 2.

## Deliverable 2: Create Visualizations for the Trip Analysis

1. Using Tableau, create visualizations that show:
	How long bikes are checked out for all riders and genders.
	How many trips are taken by the hour for each day of the week, for all riders and genders.
	A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender.

2. Open Tableau and import the new CSV file that contains the conversion of the "tripduration" column to a datetime datatype in a new Tableau workbook.


3. Create the Checkout Times for Users Viz
	In this visualization, you’ll graph the length of time that bikes are checked out for all riders.

	a. Add the number of records or the generated field that counts the number of records in the CSV file to the Rows.
	b. Add the "tripduration" column you converted to the Columns, and filter the "More" option by "Hour".
	c. Add the "tripduration" column again to the Columns, and filter the "More" option by "Minute", and then change the values from "discrete" to "continuous".
	d. Add the "tripduration" column that shows the "Hour" to the Filters field, and select "Show Filter".
	e. Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".


4. Create the Checkout Times by Gender Viz
	In this visualization, you’ll graph the length of time that bikes are checked out for each gender.

	a. Add the number of records or the generated field that counts the number of records in the CSV file to the Rows.
	b. Add the "tripduration" column you converted to the Columns, and filter the "More" option by "Hour".
	c. Add the "tripduration" column again to the Columns, and filter the "More" option by "Minute", and then change the values from "discrete" to "continuous".
	d. Add the "tripduration" column that shows the "Hour" to the Filters field, and select "Show Filter".
	e. Add the converted column for gender as a color to the Marks field, add it to the Filters field, and select "Show Filter".
	f. Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".

5. Create the Trips by Weekday for Each Hour Viz
	In this visualization, you’ll graph the number of bike trips by weekday for each hour of the day as a heatmap.

	a. Add the "Starttime" column to the Rows, and filter the "More" option by "Hour".
	b. Add the "Stoptime" column to the Columns, and filter the “More” option by "Weekday".
	c. Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.
	d. Format the Y axis of the Starttime by Hour to show the 12-hour format, as shown in the following image:
	e. Format the X axis of Stoptime by Weekday as "Abbreviation".

6. Create the Trips by Gender (Weekday per Hour) Viz
	In this visualization, you’ll graph the number of bike trips by gender for each hour of each day of the week as a heatmap.

	a. Add the "Starttime" column to the Rows, and filter the "More" option by "Hour".
	b. Add the "Stoptime" column to the Columns, and filter the “More” option by "Weekday".
	c. Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.
	e. Add the converted column for "Gender" to the Columns and to the Filters field, and select "Show Filter".
	f. Format the Y axis of the Starttime by Hour to show the 12-hour format.
	g. Format the X axis of Stoptime by Weekday as "Abbreviation".

7. Create the User Trips by Gender by Weekday Viz
	In this visualization, you'll create a heatmap that shows the number of bike trips broken down by gender for each day of the week by each Usertype.

	a. Add the converted column for "Gender" to the Columns and to the Filters field, and select "Show Filter".
	b. Add the "Usertype" to the Rows and to the Filters field, and select "Show Filter".
	c. Add the "Starttime" column to the Rows, and filter the "More" option by "Weekday".
	d. Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.

## Deliverable 3:  Create a Story and Report for the Final Presentation 

    In Tableau, create a new Story using visualizations that will support the key findings you want to show.
1. You must use the five visualizations that you created in Deliverable 2.
2. You must use at least two visualizations that you created in this module.

## bikesharing Results 
  
  - link to Tableau Dashboard/Story - https://public.tableau.com/app/profile/raney.mathew.john/viz/NYC_CitiBike_Challenge_16539620907050/FinalPresentation?publish=yes

  - Checkout Time for Users
    ![image_name](https://github.com/raneymjohnGit/bikesharing/blob/main/Resources/Checkout_Time_for_Users.png)
  
    it appears that most users uses the bike for 30 to 40 minutes

  - Checkout Time by Gender
    ![image_name](https://github.com/raneymjohnGit/bikesharing/blob/main/Resources/Checkout_Time_by_Gender.png)

    it appears that MALE users uses the bike more than any other gender types

  - Trips by Weekday for Each hour
    ![image_name](https://github.com/raneymjohnGit/bikesharing/blob/main/Resources/Trips_by_Weekday_for_Each_hour.png)

    it appears that morning 7 to 10 and evening 5 to 7 users uses the bike more on Weekdays and on weekends (saturdays and sundays), the trips are evenly distributed from 9 AM to 9 PM.

  - Trips by Gender (Weekday per hour)
    ![image_name](https://github.com/raneymjohnGit/bikesharing/blob/main/Resources/Trips_by_Gender_Weekday_per_hour.png)

    it appears that MALE users are in majority during the rush hours (Weekdays - 7 AM to 10 AM and 5 PM to 7 PM, Weekends 9 AM to 9PM)

  - User Trips by Gender by Weekday 
    ![image_name](https://github.com/raneymjohnGit/bikesharing/blob/main/Resources/User_Trips_by_Gender_by_Weekday.png)

    it appears that subscriber user uses bike more weekdays than on weekends and customer user usage is evenly distributed among all days


## bikesharing Summary
1.  Subscribers uses more trips than regulat customers. So when we start the business in Des Moines we need to start with a subscription
2.  Following two additional visualizations are needed to determine the feasibility of bike sharing business in Des Moines.
    
	a.  We might need information on the tourist spots and need a visualization against the number of trips started near to that toirist spots (Example: Empire Estate building)

    b. We might need a visualization against the Age group and no of trips (The inforamtion currently have may not be accurate since it has birth year upto 1885)