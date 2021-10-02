# Taxi-Fare-prediction
In this project i have been asked to predict amount of taxi fare 
# Packages used
>> os , pandas , matplotlib, seabron, Numpy, sklearn 
# Approach

**_Loading the data_**   
I have Load the data that is available in csv format 

# Summarise the dataset
Checked the rows, columns , and the datatypes of variables 

# Investigating the null values 
In this data set there are not any null values but there are some records that contain zeros and negative values

# Conducting investigation for outliers 
There are outliers in Geographical coordinates and in number of passenger traveling 

## Outlier treatment of Geogrphical coordinates
Geographical cordinates of Newyork is:{40.7128° N, 74.0060° W} any cordinates out of the above range are consider as outside from the city and treated as an outliers
capping the pickup latitude and longitude and dropoff latitude and longitude according to the geographical coordinates of NYC i.e {40.7128° N, 74.0060° W}

## Outlier treatment of number of passengers 

Here in this dataset i observe that in NYC, legally the highest no. of passenger that taxi can have is about 4 at max but in some records there are more than 4 passengers so i have consider them as an outlier by assuming the extreme or any urgent cases.

# Feature Engineering
### Distance calculation
Calculate the distance from longitude and latitude  using manhatten distance

##### Converting "date_time_of_pickup" into dtype datetime 

##### Extracting variables from date-time of pick up
>>> **Extracting**
>>>>>>pickup day    
>>>>>>pickup,day_no.    
>>>>>>pickup_hour     
>>>>>>pickup_month     
>>>>>>year and date 


# EDA

![taxi line 2](https://user-images.githubusercontent.com/87512268/135576091-2ce9a786-db90-4d62-88ea-ce9434b0f37a.png)





![taxi line 3](https://user-images.githubusercontent.com/87512268/135576177-ccaeba67-ba83-444f-bb75-33ad666c2119.png)



![taxi line 4](https://user-images.githubusercontent.com/87512268/135576278-cd47e5f2-9d0a-4615-8407-1b7808052519.png)

![taxi line last](https://user-images.githubusercontent.com/87512268/135576369-bad3376a-27df-48f9-8df6-96292b4fdd29.png)
![taxi bar last](https://user-images.githubusercontent.com/87512268/135576834-35d8de02-6922-4be9-964b-3a9efb59af88.png)

![taxi bar 2](https://user-images.githubusercontent.com/87512268/135576651-ae4272ce-df18-4348-b927-5572f5fdef96.png)


# Data Modelling

**creating the dummies of the variable having object dtype** 

**divide the data data into X and y (independent and targeted variable )**
**split the data into train and test**        
**import the ensemble model Random forest and save it into the variable**

**fit the model into X train and y train data**

### Evaluate the model    
Checking score      

#### Perform Hyperparameter tuning by using grid search   

Image result for what hyperparameters grid search tuning does
Hyperparameter tuning is choosing a set of optimal hyperparameters for a learning algorithm. A hyperparameter is a model argument whose value is set before the learning process begins. The key to machine learning algorithms is hyperparameter tuning.

# Check the model score   

# MSE
The mean squared error (MSE) or mean squared deviation (MSD) of an estimator (of a procedure for estimating an unobserved quantity) measures the average of the squares of the errors—that is, the average squared difference between the estimated values and the actual value.

#  r2_score
The proportion of the variance in the dependent variable that is predictable from the independent variable(s)



