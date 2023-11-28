# Predicting-Airline-Passenger-Satisfaction

## 1. Research background 

This dataset contains an airline passenger satisfaction survey, which serves as a valuable resource for understanding and analyzing the factors influencing passenger satisfaction in the airline industry. With the increasing competition and the growing significance of customer experience, airlines are recognizing the importance of ensuring high levels of passenger satisfaction to maintain a competitive edge in the market. 

The airline industry is a complex ecosystem where various factors contribute to the overall passenger experience. From ticket booking to check-in, boarding, in-flight services, and baggage handling, each stage of the passenger journey can significantly impact their satisfaction levels. Understanding the key drivers of passenger satisfaction is crucial for airlines to identify areas of improvement and develop effective strategies to enhance the overall customer experience. 

The dataset provides comprehensive information about passengers of an airline. It encompasses various attributes related to passenger demographics, travel details, and satisfaction ratings. By analyzing large-scale datasets like the one at hand, researchers can gain valuable insights into passenger perceptions, preferences, and expectations, allowing for a comprehensive understanding of the factors that shape passenger satisfaction. 

## 2. Research objective

In this project, we're diving into the world of air travel to understand what makes passengers happy or dissatisfied. We have a bunch of data, including details about passengers, their flights, and how they rate different aspects of their journey. 

Our goal is to figure out what factors influence passenger satisfaction, how airlines can make travelers' experiences better and what can be improved in the future. We'll use data analysis and machine learning to find insights that can help airlines improve and keep their customers happy. So, let's take off on this data-driven journey to explore what makes passengers smile when they fly. 

## 3. Methodology
### 3.1. Dataset

TJ Klein (2019). Airline Passenger Satisfaction. Retrieved from: 
 https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction/data. 
 
This dataset contains an airline passenger satisfaction survey. It is related to customer satisfaction ratings and travel details. The attributes in this dataset may provide information on gender, customer type, age, travel purpose, seat class, flight distance, various services and amenities provided during the flight, departure and arrival delays, and customer satisfaction levels. 

### 3.2. Data
This dataset contains 24 attributes: 

**id**: An identification number or unique identifier for each customer entry. 

**Gender**: The gender of the customer. 

**Customer Type**: Indicates whether the customer is a loyal or disloyal customer.

**Age**: The age of the customer. 

**Type of Travel**: Specifies the purpose of travel, such as business or personal. 

**Class**: The class or category of travel, such as Economy (Eco) or Business. 

**Flight Distance**: The distance of the flight in units not specified. 

**Inflight wifi service**: A rating indicating the satisfaction level with the inflight Wi-Fi service. 

**Departure/Arrival time convenient**: A rating indicating the satisfaction level with the convenience of departure and arrival times. 

**Ease of Online booking**: A rating indicating the satisfaction level with the ease of online booking process. 

**Gate location**: A rating indicating the satisfaction level with the gate location. 

**Food and drink**: A rating indicating the satisfaction level with the quality of food and drinks. 

**Online boarding**: A rating indicating the satisfaction level with the online boarding process. 

**Seat comfort**: A rating indicating the satisfaction level with the comfort of seats. 

**Inflight entertainment**: A rating indicating the satisfaction level with the inflight entertainment options. 

**On-board service**: A rating indicating the satisfaction level with the on-board service. 

**Leg room service**: A rating indicating the satisfaction level with the leg room space. 

**Baggage handling**: A rating indicating the satisfaction level with the handling of baggage. 

**Check-in service**: A rating indicating the satisfaction level with the check-in service. 

**Inflight service**: A rating indicating the satisfaction level with the inflight service. 

**Cleanliness**: A rating indicating the satisfaction level with the cleanliness of the aircraft. 

**Departure Delay in Minutes**: The duration of departure delay in minutes. 

**Arrival Delay in Minutes**: The duration of arrival delay in minutes. 

**Satisfaction**: Indicates the customer satisfaction level, which can be "satisfied," "neutral or dissatisfied," or potentially other values. 

### 3.3. Process

The data processing is carried out using the following steps and methods: 

**Step 1:** Importing necessary libraries: 
The code begins by importing the required libraries. These libraries include NumPy, Matplotlib, Pandas, Seaborn, and various modules from scikit-learn. These libraries provide essential functions and tools for data manipulation, visualization, and machine learning. 

**Step 2:** Checking data size: 
The code utilizes the shape method of the "train" DataFrame to obtain the dimensions of the data. This provides information about the number of rows (instances) and columns (features) in the dataset. 

**Step 3:** Patching scikit-learn: 
The sklearnex library is used to patch scikit-learn with the Intel(R) Extension for Scikitlearn*. This extension enhances the performance of scikit-learn algorithms by leveraging Intel's optimized implementations. 

**Step 4:** Checking and updating scikit-learn version: 
The code checks the version of scikit-learn installed in the environment. If a newer version is available, it is recommended to update scikit-learn for potential bug fixes and improvements. 

**Step 5:** Importing modules and functions: 
Several modules and functions from scikit-learn are imported to support various tasks in the data processing and modeling pipeline. These include functions for confusion matrix calculation, ROC AUC score computation, accuracy score calculation, as well as classes and methods for different machine learning algorithms, such as K-nearest neighbors (KNeighborsClassifier), support vector machines (SVC), ensemble methods, neural networks (MLPClassifier), linear regression (LinearRegression), logistic regression (LogisticRegression), random forest (RandomForestClassifier), and evaluation metrics (metrics). 

**Step 6:** Importing and processing data: 
The code reads data from two CSV files, "train.csv" and "test.csv", and stores them in separate Pandas DataFrames named "train" and "test". These DataFrames contain the raw data for training and testing purposes. Additionally, the code defines several functions, such as transform_gender, transform_customer_type, transform_travel_type, transform_class, and transform_satisfaction, to preprocess the data. These functions handle tasks such as transforming categorical variables into numerical representations, handling missing values, and scaling numerical features. 

## 4. Result and figures

![Figure 1. Percentage of customers Satisfied - Neutral or Dissatisfied](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%201.%20Percentage%20of%20customers%20Satisfied%20-%20Neutral%20or%20Dissatisfied.png)

 Satisfied (43.3%): Passengers who are satisfied with the airline service.
Neutral or Dissatisfied (56.7%): Passengers who have neutral or negative sentiments about the airline service. This classification problem involves using the provided dataset attributes to determine the level of passenger satisfaction, which is a critical aspect for airlines to understand and improve their services.

![Figure 2. Correlation coefficient of Train.csv’s attributes](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%202.%20Correlation%20coefficient%20of%20Train.csv%20%E2%80%98s%20attributes.png)

Each intersection square shows the correlation coefficient between 2 attributes: 
Closed to 1: Strong positive relationship.
Closed to -1: Strong negative relationship.
Closed to 0: Weak relationship.

![Figure 3. Correlation between Arrival Delay in Minutes and Departure Delay in Minutes](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%203.%20Correlation%20between%20Arrival%20Delay%20in%20Minutes%20and%20Departure%20Delay.png)

The analysis reveals a clear relationship between departure delays and arrival delays in the airline industry. The majority of delays in both departure and arrival are concentrated within the range of 0-600 minutes, with occasional instances of longer delays up to approximately 1400 minutes. Moreover, it is evident that as the duration of departure delays increases, there is a corresponding increase in the duration of arrival delays. This finding highlights the interconnected nature of these two factors and emphasizes the importance of effectively managing and minimizing delays in both departure and arrival processes for improved efficiency and customer satisfaction.


![Figure 4. Distributions of Categorical Features](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%204.%20Distributions%20of%20Categorical%20Features.png)

Gender: Female (1): 51% ; Male (0): 49%
Customer Type: Loyal Customer (1): 82% ; Disloyal Customer (0): 18%
Type of travel: Business Travel (1): 69% ; Personal Travel (0): 31%
Class: Business (2): 48% ; Eco (0): 45% ; Other (1): 7% 
We can easily see that: 
The number of men and women in this sample was approximately equal.
The majority of this airline's customers are loyal customers.
Most customers fly for business reasons rather than for personal reasons.
About half of the passengers were in business class.
More than 60% of passengers are satisfied with the baggage handling service (rating 4-5/5).
More than 50% of passengers felt comfortable in their seats (seat comfort: rated 4-5/5).

![Figure 5.  Distributions of Customer Type](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%205.%20%20Distributions%20of%20Customer%20Type.png)

From the two charts below, it is noticeable that there are two types of client: loyal and disloyal customer. 
The age range of loyal customers is between 20 and 60 years old, with particular emphasis on the age groups of 20-30 and 40-50. The level of loyalty gradually decreases as customers reach the age of 60. 
The age group of 20-30 years old has the highest proportion of disloyal customers.

![Figure 6.  Class distribution by age](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%206.%20%20Class%20distribution%20by%20age.png)

From the chart, we can observe three main seat classes: Eco Plus, Eco, and Business, which are compared based on their popularity among different age groups. 
Observations show that the average age of business class passengers is similar to that of loyal customers. Based on this observation, it can be assumed that loyal customers mainly buy business class tickets for themselves.

![Figure 7. Class distribution by Flight Distance](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%207.%20Class%20distribution%20by%20Flight%20Distance.png)

Passengers on long - distance flights mainly choose to travel in business class.
In addition, customers mainly take flights from 1000km in all classes but mainly business class.

![Figure 8. Distribution of Inflight entertainment and Leg room service by Flight Distance](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%208.%20Distribution%20of%20Inflight%20entertainment%20and%20Leg%20room%20service.png)

Passengers who travel longer distances on flights tend to exhibit higher levels of satisfaction with the inflight entertainment options and appreciate the leg room service. This suggests that the duration of the flight has an impact on passengers' preferences and expectations for these amenities. Airlines may consider prioritizing the quality and variety of inflight entertainment and ensuring comfortable leg room for longer flights to enhance passenger satisfaction.

![Figure 9. Satisfaction Comparison by Class](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%209.%20Satisfaction%20Comparison%20by%20Class.png)

The data reveals that Business class (2) has the highest customer satisfaction rate, as indicated by the highest proportion of satisfied votes (1). On the other hand, Eco class (0) has the lowest customer satisfaction rate, as reflected by the highest proportion of unsatisfied votes (0). This suggests that passengers in Business class generally have a more positive experience and higher satisfaction levels compared to those in Eco class. Airlines may need to focus on improving the overall experience and addressing any issues specific to Eco class to enhance customer satisfaction in that class.

![Figure 10. Satisfaction Comparison by Inflight wifi service](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%2010.%20Satisfaction%20Comparison%20by%20Inflight%20wifi%20service.png)
 
There is a clear correlation between the quality of inflight WiFi service and customer satisfaction. The data indicates that when the inflight WiFi service is better, customers tend to be more satisfied with their overall flying experience. Conversely, when the inflight WiFi service is poorer, customer satisfaction decreases. This highlights the importance of a reliable and high-quality inflight WiFi service in meeting passengers' expectations and enhancing their satisfaction levels. Airlines should strive to provide robust and efficient WiFi connectivity to improve the overall customer experience and meet the increasing demand for connectivity during flights.

![Figure 11. Satisfaction Comparison by Seat Comfort and Leg room service](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Figure%2011.%20Satisfaction%20Comparison%20by%20Seat%20Comfort%20and%20Leg%20room%20service.png)

The analysis clearly demonstrates that there is a direct relationship between seat comfort, leg room service, and customer satisfaction when flying. When the seat comfort and leg room service are better, customers tend to be more satisfied with their overall flying experience. Conversely, when seat comfort and leg room are lacking, customer satisfaction decreases.

## 5. Model Evaluation

Now to the models! We will be trying out a few different models to see which one is the best choice for our problem. I have created a small function below which will train, predict, and evaluate all of our models. We will be evaluating the performance of our models with the ROC_AUC metric. This metric is good for the classification of a dataset which a relatively balance dataset in terms of our target. We will also be looking at the confusion matrix for our model to best understand how our model is mischaracterizing predictions (Are we seeing majority false positives? etc.)

**Correlation**

![image47.png](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/image47.png)

**RandomForest**

![RandomForest.png](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/RandomForest.png)

**LightGBM**

![LightGBM.png](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/LightGBM.png)

**Catboost**

![Catboost.png](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/Catboost.png)

**XGBoost**

![XGBoost.png](https://github.com/khvu0610/Predicting-Airline-Passenger-Satisfaction/blob/70a029ada967d5f367d2df4df7b068bd2d501aa1/Images/XGBoost.png)


Based on the roc_auc metric, we have a clean winner. Our Random forest classifier outperformed all of our other models. One thing to keep in mind is that both the Catboost and the XGBoost classifiers just used default parameters without any hyperparameter tuning.


## 6. Conclusion

**1. 	What factors are highly correlated to a satisfied (or dissatisfied) passenger?**
 
50% of passengers feel comfortable in their seats (rated 4-5/5). 

More than 60% of passengers are satisfied with the luggage transportation service (rating 4-5/5). 

The majority of passengers who rated seat comfort and leg room service at 4 and 5 out of 5 were satisfied with the flight.

Most passengers who rated the inflight wifi service 5/5 were satisfied with the flight. 

**2. 	Can we predict passenger satisfaction?**

We can predict  passenger satisfaction: 

The farther airline passengers travel (the longer they stay on the flight), the more satisfied they are with in-flight entertainment and the more legroom they have (on average). 

Most passengers flying straight or in Eco Class were unsatisfied with the flight, while those flying in Business Class were satisfied. 

**3.  What can be improved in the future?**

**Seat Comfort**: Since 50% of passengers feel comfortable in their seats, we focus on enhancing seat comfort by investing in seats with better cushioning, adjustable features, and ergonomic designs.

**Luggage Transportation Service**: While more than 60% of passengers are satisfied with the luggage transportation service, we need enhancement to improve this aspect such as providing clearer instructions to passengers in order to minimize the lost or damaged luggage.

**Inflight WiFi Service**: Since passengers who rated the inflight WiFi service 5 points were satisfied with the flight, we should ensure a high-speed WiFi connection throughout the flight. Monitoring and upgrading to the WiFi can improve passenger satisfaction in this aspect.

**Legroom**: Considering that passengers who have more legroom tend to be more satisfied, it is better to explore options for increasing legroom in all classes. This could be to arrange seat layouts, optimizing legroom, or offering seating options with extra legroom for passengers who prefer more space.

**Class of Travel**: To address the disparity (dəˈsperədē) in satisfaction between different classes, we can assess and identify the specific factors contributing to dissatisfaction in Eco Class and passengers flying straight. 

**Passenger Feedback**: Collecting feedback from passengers by implementing a system for collecting feedback, such as online feedback forms to gather specific suggestions and identify areas for improvement directly from the passengers.

