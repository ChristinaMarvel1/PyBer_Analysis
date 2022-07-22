# PyBer_Analysis
## Deliverable 1: A ride-sharing summary DataFrame by city type
Using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns, get the total number of rides, total number of drivers, and the total fares for each city type. Then, calculate the average fare per ride and average fare per driver for each city type. Finally, add this data to a new DataFrame, then format the columns.

 - Download the PyBer_Challenge_starter_code.ipynb file into your PyBer_Analysis folder and rename it PyBer_Challenge.ipynb.
 - Use the step-by-step instructions below to add code where indicated by the numbered comments in the starter code file.
1. In Step 1, use the groupby() function to create a Series of data that has the type of city as the index, then apply the count() method to the "ride_id" column.
![image 1-1](https://user-images.githubusercontent.com/107659667/179427072-e43b2a1f-44ae-499c-9c1a-df6d3c0d6a8f.jpg)


2. In Step 2, use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "driver_count" column.
![image 1-2](https://user-images.githubusercontent.com/107659667/179427087-489c13bd-d801-4852-b119-4625e9580f0e.jpg)


3. In Step 3, use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "fare" column.
![image 1-3](https://user-images.githubusercontent.com/107659667/179427090-ce7df87a-20c5-431d-b38e-0e741fd79ca4.jpg)

4. In Step 4, calculate the average fare per ride by city type by dividing the sum of all the fares by the total rides.
![image 1-4-1](https://user-images.githubusercontent.com/107659667/179427123-b5f8c683-3281-4382-942c-f077bf1b01fa.jpg)
![image 1-4-2](https://user-images.githubusercontent.com/107659667/179427124-ae268ca8-f6a8-4d75-a7c3-5e79875df4f1.jpg)
![image 1-4-3](https://user-images.githubusercontent.com/107659667/179427125-f7486e39-ca04-47af-9727-954c4927c86f.jpg)


6. In Step 5, calculate the average fare per driver by city type by dividing the sum of all the fares by the total drivers.
![image 1-5](https://user-images.githubusercontent.com/107659667/179427127-5850e7ca-51ac-40a3-a01d-1941ba321b16.jpg)


8. In Step 6, create a PyBer summary DataFrame with all the data gathered from Steps 1-5, using the column names shown below:.
The unformatted PyBer summary DataFrame showing the “Total Rides,” “Total Drivers,” “Total Fares,” “Average Fare per Ride,” and “Average Fare per Driver by city type.
![image 1-6](https://user-images.githubusercontent.com/107659667/179427132-197d69b6-d4f2-46ff-90dd-9fa69f6bf362.jpg)


7. In Step 7, use the provided code snippet to remove the index name ("type") from the PyBer summary DataFrame.
![image 1-7](https://user-images.githubusercontent.com/107659667/179427139-95dd1513-465b-41b7-93a3-442d1f888b87.jpg)


9. In Step 8, format the columns of the Pyber summary DataFrame to look like this:
The formatted summary DataFrame showing the “Total Rides,” “Total Drivers,” “Total Fares,” “Average Fare per Ride,” and “Average Fare per Driver” by city type
![image 1-8](https://user-images.githubusercontent.com/107659667/179427140-0e79ea43-3300-4afd-bcd7-44b48ec6e91f.jpg)


## Deliverable 2 : Using your Pandas skills and two new functions, pivot() andresample(), create a multiple-line graph that shows the total fares for each week by city type.

 - Use the step-by-step instructions below to add code where indicated by the numbered comments in the starter code file:

1. In Step 1, create a new DataFrame with multiple indices using the groupby() function on the "type" and "date" columns of the pyber_data_df DataFrame, then apply the sum() method on the "fare" column to show the total fare amount for each date.
![image 2-1](https://user-images.githubusercontent.com/107659667/179427150-70eee61b-4533-4ceb-83fc-151dfced56a4.jpg)


2. In Step 2, use the provided code snippet to reset the index. This is needed to use the pivot() function in the next step (Step 3).
![image 2-2](https://user-images.githubusercontent.com/107659667/179427156-936db841-bce9-4616-ab10-89ade4f027c5.jpg)

3. In Step 3, use the pivot() function to convert the DataFrame from the previous step so that the index is the "date," each column is a city "type," and the values are the "fare."
![image 2-3](https://user-images.githubusercontent.com/107659667/179427162-e2194091-64e1-47ac-87d4-90a9aa549bda.jpg)

4. In Step 4, create a new DataFrame by using the loc method on the following date range: 2019-01-01 through 2019-04-28.
![image 2-4](https://user-images.githubusercontent.com/107659667/179427189-707cbe0b-b9af-440c-a466-4163625c5caf.jpg)

5. In Step 5, use the provided code snippet to reset the index of the DataFrame from the previous step (Step 4) to a datetime data type. This is necessary to use the resample() method in Step 7.
![image 2-5](https://user-images.githubusercontent.com/107659667/179427192-48964b17-c5da-4e9d-a08c-9a8a8cdca11b.jpg)

6. In Step 6, use the provided code snippet, df.info(), to check that the "date" is a datetime data type.
![image 2-6](https://user-images.githubusercontent.com/107659667/179427197-a3ec9f08-721c-4def-bc4d-47b8b2c5fd66.jpg)

7. In Step 7, create a new DataFrame by applying the resample() function to the DataFrame you modified in Step 5. Resample the data in weekly bins, then apply the sum() method to get the total fares for each week.
 ![image 2-7](https://user-images.githubusercontent.com/107659667/179427200-1732d9c9-201e-464e-a2b5-97e5116ca2d5.jpg)

8. Finally, in Step 8, graph the resampled DataFrame from Step 7 using the object-oriented interface method and the df.plot() method, as well as the Matplotlib "fivethirtyeight" graph style code snippet provided in the starter code. Annotate the y-axis label and the title, then use the appropriate code to save the figure as PyBer_fare_summary.png in your "analysis" folder.
![image 2-8](https://user-images.githubusercontent.com/107659667/179427201-3d4f5d61-c329-4f4b-b66f-e5bb14169654.jpg)

Confirm that your multiple-line chart looks like the following image, where each week is a peak or dip in the line graphs.
The average weekly fare for each city from January 1, 2019 to April 28, 2019.

![PyBer_fare_summary](https://user-images.githubusercontent.com/107659667/179427380-d31b646e-f45a-4102-afd0-f5937dce8ca3.png)


## Deliverable 3 : Use your repository README file to write your analysis of how to address any disparities in the ride-sharing data among the city types.

The analysis should contain the following:

Overview of the analysis: Explain the purpose of the new analysis.
Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.


![PyBer_fare_summary](https://user-images.githubusercontent.com/107659667/180354024-36dcb5ba-7449-4085-87a8-1eb90d2be8f5.png)


![Fig5](https://user-images.githubusercontent.com/107659667/180354135-495073d4-1573-4838-b4fa-0dcd3325eccc.png)



![Fig6](https://user-images.githubusercontent.com/107659667/180354145-0d9035c1-2f96-4441-ac4f-6df634d4e104.png)


![Fig7](https://user-images.githubusercontent.com/107659667/180354153-370ae25f-c08d-401c-be3a-b997bcfd8b28.png)


![Fig1](https://user-images.githubusercontent.com/107659667/180354173-86669c5c-1f98-4b86-bd3c-caa2db7d000f.png)


Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.


Three business recommendations to the CEO for addressing any disparities among the city types. 
