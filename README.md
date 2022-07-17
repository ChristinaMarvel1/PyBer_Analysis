# PyBer_Analysis
# Deliverable 1: A ride-sharing summary DataFrame by city type
Using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns, get the total number of rides, total number of drivers, and the total fares for each city type. Then, calculate the average fare per ride and average fare per driver for each city type. Finally, add this data to a new DataFrame, then format the columns.

 - Download the PyBer_Challenge_starter_code.ipynb file into your PyBer_Analysis folder and rename it PyBer_Challenge.ipynb.
 - Use the step-by-step instructions below to add code where indicated by the numbered comments in the starter code file.
1. In Step 1, use the groupby() function to create a Series of data that has the type of city as the index, then apply the count() method to the "ride_id" column.
2. In Step 2, use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "driver_count" column.
3. In Step 3, use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "fare" column.
4. In Step 4, calculate the average fare per ride by city type by dividing the sum of all the fares by the total rides.
5. In Step 5, calculate the average fare per driver by city type by dividing the sum of all the fares by the total drivers.
6. In Step 6, create a PyBer summary DataFrame with all the data gathered from Steps 1-5, using the column names shown below:.
The unformatted PyBer summary DataFrame showing the “Total Rides,” “Total Drivers,” “Total Fares,” “Average Fare per Ride,” and “Average Fare per Driver by city type.

7. In Step 7, use the provided code snippet to remove the index name ("type") from the PyBer summary DataFrame.
8. In Step 8, format the columns of the Pyber summary DataFrame to look like this:
The formatted summary DataFrame showing the “Total Rides,” “Total Drivers,” “Total Fares,” “Average Fare per Ride,” and “Average Fare per Driver” by city type


# Deliverable 2 : Using your Pandas skills and two new functions, pivot() andresample(), create a multiple-line graph that shows the total fares for each week by city type.

 - Use the step-by-step instructions below to add code where indicated by the numbered comments in the starter code file:

1. In Step 1, create a new DataFrame with multiple indices using the groupby() function on the "type" and "date" columns of the pyber_data_df DataFrame, then apply the sum() method on the "fare" column to show the total fare amount for each date.

2. In Step 2, use the provided code snippet to reset the index. This is needed to use the pivot() function in the next step (Step 3).

3. In Step 3, use the pivot() function to convert the DataFrame from the previous step so that the index is the "date," each column is a city "type," and the values are the "fare."

After this step, you’ll see that each cell has the total fare for the date and time, as shown in the following image.

4. In Step 4, create a new DataFrame by using the loc method on the following date range: 2019-01-01 through 2019-04-28.
5. In Step 5, use the provided code snippet to reset the index of the DataFrame from the previous step (Step 4) to a datetime data type. This is necessary to use the resample() method in Step 7.
6. In Step 6, use the provided code snippet, df.info(), to check that the "date" is a datetime data type.
7. In Step 7, create a new DataFrame by applying the resample() function to the DataFrame you modified in Step 5. Resample the data in weekly bins, then apply the sum() method to get the total fares for each week.
 
6. Finally, in Step 8, graph the resampled DataFrame from Step 7 using the object-oriented interface method and the df.plot() method, as well as the Matplotlib "fivethirtyeight" graph style code snippet provided in the starter code. Annotate the y-axis label and the title, then use the appropriate code to save the figure as PyBer_fare_summary.png in your "analysis" folder.

Confirm that your multiple-line chart looks like the following image, where each week is a peak or dip in the line graphs.
The average weekly fare for each city from January 1, 2019 to April 28, 2019.


Deliverable 3 Instructions
Use your repository README file to write your analysis of how to address any disparities in the ride-sharing data among the city types.

The analysis should contain the following:

Overview of the analysis: Explain the purpose of the new analysis.
Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.

Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.


Three business recommendations to the CEO for addressing any disparities among the city types. 
