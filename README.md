# STATS447B-Project
##  Prediction on insurance claim of cars
* Image identification of damaged cars
* Prediction on claim of damaged cars 
# convolutional neural network
* A typical CNN has several convolution plus pooling layers and fully connected layers in the end 
* Each responsible for feature extraction at different levels of abstraction
* Filters in first layer detect horizental, vertical, and diagonal edges
* Filters in the next layer detect shapes
* Filters in the last layer detect collection of shapes
* Filter values randomly initialized, learned by learning algorithm
* convolutional layer 

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
