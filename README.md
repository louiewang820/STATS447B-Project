# STATS447B-Project
## Problem Statement
You have been hired as a Machine Learning expert by a leading car insurance company. Your task is to predict the insurance claim of the cars that are provided in the dataset.
* Condition: Predict if the vehicle provided in the image is damaged or not
* Amount: Based on the condition of a vehicle, predict the insurance amount of the cars that are provided in the dataset

source: https://www.hackerearth.com/en-us/challenges/competitive/hackerearth-machine-learning-challenge-vehicle-insurance-claim/
## Abstract
I apply deep learning skills to build a CNN model that predicts the insurance claim of the cars that are provided in the dataset. I have achieved test accuracy 
above 90% for image identification of damaged cars.
##  Prediction on insurance claim of cars
* Part I: Image identification of damaged cars 
* Part II: Prediction on claim of damaged cars 
## convolutional neural network
* A typical CNN has several convolution plus pooling layers and fully connected layers in the end 
* Each responsible for feature extraction at different levels of abstraction
* Filters in first layer detect horizental, vertical, and diagonal edges
* Filters in the next layer detect shapes
* Filters in the last layer detect collection of shapes
* Filter values randomly initialized, learned by learning algorithm


<img src="https://miro.medium.com/max/700/0*opZllXHxr_539y6K.gif" width="750" align="center">

Gif showing how a 3x3 kernel passes over the entire image. 
Source: https://www.machinelearninguru.com//computer_vision/basics/convolution/convolution_layer.html

<img src="https://img-blog.csdnimg.cn/img_convert/711b9168e49cff2547ca4c1d01fb2561.png" width="750" align="center">
Source: https://speech.ee.ntu.edu.tw/~hylee/ml/2021-spring.php


* max pooling layer 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20190721025744/Screenshot-2019-07-21-at-2.57.13-AM.png" width="750" align="center">

Image showing how a 2x2 filter selects the maximum element from the region of the feature map covered. 

Source: https://media.geeksforgeeks.org/wp-content/uploads/20190721025744/Screenshot-2019-07-21-at-2.57.13-AM.png

<img src="https://img-blog.csdnimg.cn/2a38a457ee224be6bd0cc1631b1adb82.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQzNzExNjk3,size_16,color_FFFFFF,t_70" width="750" align="center">

Source: https://speech.ee.ntu.edu.tw/~hylee/ml/2021-spring.php

* Example of CNN structure

<img src="https://i0.wp.com/developersbreach.com/wp-content/uploads/2020/08/cnn_banner.png?fit=1200%2C564&ssl=1" width="750" align="center">

Source: https://developersbreach.com/convolution-neural-network-deep-learning/

## Summary plots of Insurance_company in train and test dataset
![image](https://user-images.githubusercontent.com/72156683/157354377-a5f29d31-76d7-40f5-b900-159fa3193bc4.png)

# Data augumentation
* Our data set is imbalanced
* We need more images of undamaged cars
* augment each image twelve times
![image](https://user-images.githubusercontent.com/72156683/157355019-6b989c06-ba28-4761-ad29-a506d6848b82.png)

## Wrangling of Variables and Transformations
### Can we do a regression for continous response variable Amount?
- Are any of the features useful in estimating Amount?
![image](https://user-images.githubusercontent.com/72156683/157355266-725c6173-c942-4382-a5e7-d0b37da46164.png)
- No clear relationships with Amount. 
- Cost of Vehicle and Min Coverage looks identical
- Interesting distribution of Max Coverage
![image](https://user-images.githubusercontent.com/72156683/157355329-8e6168cc-dca7-45cd-afce-9c0c27792527.png)
### Possible Solutions
- Random forest
- XGBoost
- CNN with continuous output (combine part I and II together)


This project is ongoing
