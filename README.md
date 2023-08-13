# Car Rentals - Exploratory Data Analysis

An interactive dashboard is created on Tableau to perform exploratory data analysis (EDA) on the Car rentals dataset.

Before proceeding towards creating a dashboard, we need to make sure the data is cleaned and processed in order to produce accurate insights. 
The dataset Project.csv is a cleaned version of the original dataset. Preprocessing steps were performed.

##Data Preprocessing

There were no duplicates in this dataset. However, there were a few discrepancies in this dataset that was identified in the process and have been corrected using the following techniques - 

●	Missing values - There were 75 missing values in the FuelType feature, and 501 missing values in the rating feature. Dealing with the Fuel type feature, it was observed that 64 such values were missed out while fetching this information and can be filled using information having similar car model and make. There were 11 values that could not be filled using the information available in the dataset. 
  -	In case of the missing values of rating, we decided to delete these rows from the dataset for our analysis. This could be imputed with a mean value of 4.92 or a median value of 5. In doing this, the skewness of the data would be high towards the right, which could result in inappropriate insights in our analysis. Therefore, we decided to delete them.
  -	Therefore, we have deleted 512 rows from the dataset, and have moved ahead with 5339 observations for our analysis.

●	String Inconsistencies - For the vehicle make and model, there were many values that were spelled in different forms but belonged to the same make/model. These have been changed and made consistent throughout the dataset. In a few instances “Alfa Romeo” was spelled as “Alfa-romeo” and “Alfa Romeo” in the vehicle make a feature. Another example is a BMW 2 Series was spelled as “2 Series” and “2-series” in the vehicle model feature.

●	Data compatibility - There were a few instances whose the fuel type of the car was not matching with the car model. For example, the car Camry Hybrid is a Hybrid fuel type. However, the fuel type mentioned for this car was Gasoline. It is corrected to Hybrid for our analysis.

##Data Visualization

You can find the Tableau workbook in the folder

##Insights
- The average daily rate of the car rented is 91$, the average rating is 5, and the average number of trips taken is 37.
- California and Florida are the states where the cars are rented the most. 
- Tesla and BMW are the top car models that are rented in California. Toyota is rented the most in Colorado.
- There are a set of luxury cars whose avg rate is fairly higher than the rest. Among the luxury Cars, Porshe is a car that is rented for a longer time when compared to others.
- Hybrid cars are rented for longer trips the most, followed by gasoline, diesel, and electric.
- Cars and SUVs' daily rate is almost the same on average.

P.S. Interactive Dashboard is shared on the public server, and will be available until it expires. Link - [https://us-west-2b.online.tableau.com/t/protimatarafdar/views/USCarRentalsDashboard/Dashboard4](url)
