# NFL Play Type Analysis Using Machine Learning 

CIS-627 Big Data Capstone Project

Last Modified 04/30/2020


# Problem Statement

Which Machine Learning Algorithm will produce the best accuracy for predicting NFL play type success based on Field Position


# Requirement

Script written in R. Packages used: `tidyverse` `ggplot2` `dplyr` `corrplot` `caTools` `caret` `ROCR` `MASS` `randomForest` `neuralnet`
`e1071`


# Summary

The goal of this analysis is to determine which play type would be selected based on location on the field of play. Five ML algorithms were used to train and test our data to determine which algorithm provided the best accuracy and how play type selection could be statistical proven


# Data 
The set is over 400K rown and 255 columns. After subsetting to meet the analysis parameters I was left with 318K rows and 35 columns.
the subsets included seperating rows by the Down of the play and the Play type. Below is a visualization of all play types inculded in an NFL game. Based on this I decided to subset for the two most used playtypes. Below is a link to the original data set. 

https://www.kaggle.com/maxhorowitz/nflplaybyplay2009to2016

<a href="https://ibb.co/QrF5fFd"><img src="https://i.ibb.co/FgbPKbV/Capture4.png" alt="Capture4" border="0"></a>


# Results

The results of the analysis are very interesting. Many question can be answered about why team call the plays they do. I discovered that if a team is on their side of the field between their goal line and the 50 yard line the pass play was predicted play of choice. Pass plays which are complete usually net teams more yardage than run plays. 
Conversely, when team were on the oppsing teams side of the field the predicted play of choice was the run play. When a teams passes the 50 yard line they are now thinking they have a realistic chance of scoreing point on that drive. Their play selection becomes more balanced between run and pass.
5 ML algorithms are used to train and test our data. SVM, Random Forest, Linear Regression, Neural Network and Logistic Regression. SVM, RF, NN were used as the primary ML algorithms in training and testing the data to predict play type based on field position. LM model was used to determine what teams should do on 4th down and short with < 3 yards to go to reach a 1st down and being at least at the teams own 40 yard line. I found that on average the LM model preidcted that a team would reach the yards to gain for a 1st down. 
GLM was used to determine what play type a team should used on 3rd down and long > 5 yard and the team being at at least their own 40 yard line. The most used play was a pass play. Below is a visual of the comparison betweeen the 3 models up for the 2nd down play type prediction. The Random Forest model provided the best accuracy between the 3 ML alogrithms 

<a href="https://ibb.co/Hr3SKzq"><img src="https://i.ibb.co/FBCrhwz/Capture.png" alt="Capture" border="0"></a>








