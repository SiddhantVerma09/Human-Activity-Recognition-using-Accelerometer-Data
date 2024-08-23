# Human-Activity-Recognition-using-Accelerometer-Data

## Abstract -
The field of Human Activity Recognition (HAR) has become one of the trendiest research topics due to availability of sensors and accelerometers, low cost and less power consumption, live streaming of data and advancement in computer vision, machine learning, artificial intelligence and IoT.

Human activity recognition is the problem of classifying sequences of accelerometer data recorded by specialized harnesses or smart phones into known well-defined movements.
Movements are often normal indoor activities such as standing, sitting, jumping, and going up stairs.
Sensors are often located on the subject, such as a smartphone or vest, and often record accelerometer data in three dimensions (x, y, z).

## Challenges - 
It is a challenging problem because there is no clear analytical way to relate the sensor data to specific actions in a general way.
It is technically challenging because of the large volume of sensor data collected (e.g. tens or hundreds of observations per second) and the classical use of hand crafted features and heuristics from this data in developing predictive models.

## Literature Review - 
1)	When a device is held in its default orientation, the X axis is horizontal and points to the right, the Y axis is vertical and points up, and the Z axis points toward the outside of the screen face. Android smartphone sensors used – Accelerometer, Compass sensor, Gyroscope, Barometer.
2)	The system uses a 3-dimensional smartphone accelerometer as the only sensor to collect time series signals, from which 31 features are generated in both time and frequency domain. Activities are classified using 4 different passive learning methods, i.e., quadratic classifier, k-nearest neighbor algorithm, support vector machine, and artificial neural networks.Experiment results show that the classification rate of passive learning reaches 84.4% and it is robust to common positions and poses of cellphone.
3)	Due to the flexibility of using smartphones, the recognition accuracy will degrade with orientation, placement and subject variations. In this paper, we propose a robust human activity recognition system in terms of orientation, placement and subject variations based on coordinate transformation and principal component analysis (CT-PCA) and online support vector machine (OSVM). The proposed CT-PCA scheme is utilized to eliminate the effect of orientation variations.
![image](https://github.com/user-attachments/assets/46fb38a8-a543-4adc-8341-380bff7bf0bb)
![image](https://github.com/user-attachments/assets/24053df4-81a7-473e-b658-c7ef37c14810)
![image](https://github.com/user-attachments/assets/a7ffc223-8af1-41f3-ae19-5659152267d5)
![image](https://github.com/user-attachments/assets/8b2b678c-d936-4a10-ae2a-8b5d24ae3f33)

## Accelerometer Sensor - 
Accelerometers detect magnitude and direction of the proper acceleration, as a vector quantity, and can be used to sense orientation (because direction of weight changes). It can sense the vibrations.
1) Unit is m/s^2
2) X Y Z are the directions
STMicroelectronics LIS302DL 3-axis MEMS  is a popular model used in iPhone

## Methodology -
![image](https://github.com/user-attachments/assets/02c5fc56-345e-45d8-a2c5-fc557558d8fe)

## How do we collect data -
Historically, sensor data for activity recognition was challenging and expensive to collect, requiring custom hardware. Now smart phones and other personal tracking devices used for fitness and health monitoring are cheap and ubiquitous. 
50Hz as an optimal sensor update frequency.
Collect Accelerometer and data 3 axes for all the activities.
Feature extraction. 
UNIX Timestamp in milliseconds

![image](https://github.com/user-attachments/assets/7414f97d-5e3a-4e33-bb7a-e95c89e5adc6)

## Structure -
1. In this project we’ve used 4 machine learning algorithms namely:
Support Vector Classifier(SVC) 
Logistic Regression 
KNN Classifier 
Random Forest Classifier
2. There are 563 columns in the dataset where the last column depicts Activity  and Subject column is not of our use. Hence we drop both.
3. Rest 561 columns will be our features.

![image](https://github.com/user-attachments/assets/24fbeb67-f8fc-480c-b252-3060a2afe7fe)

## Structure - 
Inspecting a particular activity. (For eg: Standing activity)
Thus we plot line graph between time period of Standing activity and angle between X and mean gravity.
In reality, we need to inspect whether recorded value of this angle remains almost constant with minor human errors else readings can go wrong!
Final step is to classify the activities in test_data by predicting it.
Process of using all 4 algorithms is similar.

## Real-life applications - 
1. Fall detection/Jerks

2. Fitness monitoring(heart rate)and running distance measurement

3. Remote patient monitoring or kids monitoring

4. Event management/crowd management(activity +location)

5. Human productivity monitoring at workplace (location+activity)

## Conclusion -
Activity recognition is the problem of predicting the movement of a person, often indoors, based on sensor data, such as an accelerometer in a smartphone.
Streams of sensor data are often split into subs-sequences called windows, and each window is associated with a broader activity, called a sliding window approach.
Convolutional neural networks and long short-term memory networks, and perhaps both together, are best suited to learning features from raw sensor data and predicting the associated movement.















