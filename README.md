# CIS-627 Big Data Capstone

NFL Play Type Analysis

Last Modified 04/29/2020


# Problem Statement

Which Machine Learning Algorithm will produce the best accuracy for predicting NFL play type success based on Field Position
Summary: The goal of this analysis was to determine which play type would be selected based on location on the field of play. 5 ML algorithms were used to train and test our data to determine which algorithm provided the best accuracy  


# Requirement

Script written in R. Packages used: `tidyverse` `ggplot2` `dplyr` `corrplot` `caTools` `caret` `ROCR` `MASS` `randomForest` `neuralnet`
`e1071`

# Summary

The goal of this analysis was to determine which play type would be selected based on location on the field of play. Five ML algorithms were used to train and test our data to determine which algorithm provided the best accuracy 

# Execution 



# Results

The results of the analysis are very interesting. Many question can be answered about why team call the plays they do. I discovered that if a team is on their side of the field between their goal line and the 50 yard line the pass play was predicted play of choice. Pass plays which are complete usually net teams more yardage than run plays. 
Conversely, when team were on the oppsing teams side of the field the predicted play of choice was the run play. When a teams passes the 50 yard line they are now thinking they have a realistic chance of scoreing point on that drive. Their play selection becomes more balanced between run and pass.
5 ML algorithms are used to train and test our data. SVM. Random Forest, Linear Regression, Neural Network and Logistic Regression. SVM, RF, NN were used as the primary ML algorithms in training and testing the data to predict play type based on fiel position. LM model was used to determine what teams should do on 4th down and short with < 3 yards to go to reach a 1st down and being at least at the teams own 40 yard line. I found that on average the LM model preidcted that a team would reach the yards to gain for a 1st down. 
GLM was used to determine what play type a team should used on 3rd down and long > 5 yard and the team being at at least their own 40 yard line. The most used play was a pass play. 

![picture](capture.png)
![picture](capture1.png)



