# Explore-ML-models-on-IRIS-data-set

- For the IRIS data set :

- First I read and load the data set with its column names
- I did some inspections to examine  the data and its column types 
- I then checked for the outliers by drawing the boxplot from Seaborn library and I dropped down 3 rows of outliers 
- <img src = "https://user-images.githubusercontent.com/85246622/207584540-d549a312-17cd-45db-a52c-8f27482c9ba8.png" width="400" height="400"/> 
---------------------------------------------
- Then check the data for null values and look for duplicate rows and delete them
- Using the bar chart, we count the values of each class  to see if they are balanced or not
- <img src = "https://user-images.githubusercontent.com/85246622/207584563-26253b98-44fe-4b18-8678-552fd5e070de.png" width="400" height="400"/>
---------------------------------------------
- For each class I show the dist plot to see the variation in cm   
- <img src = "https://user-images.githubusercontent.com/85246622/207584573-5a5e4f2a-db03-4e49-8f3a-d1abd668ad24.png" width="400" height="400"> <img src = "https://user-images.githubusercontent.com/85246622/207584590-8c2fa1ef-0b56-4fd0-82b0-10bcfe82e9b0.png" width="400" height="400">
- <img src = "https://user-images.githubusercontent.com/85246622/207584618-84309268-e845-43c3-a74a-96648d7b00cc.png" width="400" height="400"> <img src = "https://user-images.githubusercontent.com/85246622/207584640-6d5a53e0-4e2f-4083-b835-16353f79441f.png" width="400" height="400">

---------------------------------------------
- And by using the seaborn pair plot I found the relationship between each column and the other
 - <img src = "https://user-images.githubusercontent.com/85246622/207584671-1f76accc-da6d-4ae3-affe-573c130b971b.png" width="400" height="400">
 ---------------------------------------------
- From sklearn.neighbors I import the KNeighborsClassifier to use in my KNN_model function , which I coded from scratch and contains the following :
* for the test size in the list of test sizes with 10 values from  0.15 to 0.55 increasing by 0.05 I split the data into train and test size then apply sklearn.preprocessing's MinMaxScaler to do the data normalization
* For each number of K in the K_list that contains integers I identify the model and fit the data to the model and then I get the score and for show the result I print the test size and the K and :
- print the accuracy for the train and test sets
- print the number of correct and incorrect predictions
- print the average number of correct predictions 
- draw the line graph to show the relationship between the number of the K_neighbors VS the correct & incorrect predictions AND the test size VS the train & test score
- <img src = "https://user-images.githubusercontent.com/85246622/207641559-c5bcce34-5347-41c6-a754-f6728fb7990c.png" width="400" height="400" > <img src = "https://user-images.githubusercontent.com/85246622/207641637-d7f2c1aa-04d0-482b-a978-9a91e6f729c6.png" width="400" height="400" >

---------------------------------------------
- For a general purpose function I coded a function that takes the data and the model as parameters to perform :
* for the test size in the list of test sizes with 10 values from  0.15 to 0.55 increasing by 0.05 I split the data into train and test size then apply sklearn.preprocessing's MinMaxScaler to do the data normalization 
* Using the parameter model I fit the data to it and get the train and test score and show the result that for each model name and the test size I :
- print the accuracy of the model on train and test sets 
- print the number of the correct & incorrect predictions
- draw the line graph to show the relationship between the test size VS the correct & incorrect predictions AND the test size and the train & test score 
- <img src = "https://user-images.githubusercontent.com/85246622/207642119-a3544a99-3324-4758-bc91-f663f66bef5b.png" width="400" height="400" > <img src = "https://user-images.githubusercontent.com/85246622/207642144-ae85e8b6-e6d3-4b01-a0a3-fb3895248a69.png" width="400" height="400" >
- <img src = "https://user-images.githubusercontent.com/85246622/207642410-9767b3b5-233c-49fd-b859-db9bfee98de4.png" width="400" height="400" > <img src = "https://user-images.githubusercontent.com/85246622/207642429-13f8164d-55b7-4427-b94a-ca2c659bb143.png" width="400" height="400" >
- <img src = "https://user-images.githubusercontent.com/85246622/207642540-b71919b5-82ff-427b-a53a-13294744afd9.png" width="400" height="400" > <img src = "https://user-images.githubusercontent.com/85246622/207642577-f84b5efa-4900-462c-96ce-12dbe641f65c.png" width="400" height="400" >
- <img src = "https://user-images.githubusercontent.com/85246622/207642671-24d92e05-2ea4-4d4c-bea9-5cfb92f128b0.png" width="400" height="400" > <img src = "https://user-images.githubusercontent.com/85246622/207642696-3c959fc5-fa05-45bf-8616-b56ad3348f5c.png" width="400" height="400" >
