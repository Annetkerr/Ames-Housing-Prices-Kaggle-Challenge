## Project 2 - Ames Housing Data and Kaggle Challenge

General Assembly DSI CC7 Project 2
Anne Kerr - SF

## Problem Statement
As a cohort, we have been given a challenge! Using the provided Ames Housing Data we were asked to build a model that predicts home prices. In addition to performing all the steps of a completed data science project, we were also invited to participate in a Kaggle competition. Our goal was to build the best model we could to predict home prices. We were given a training data set with target prices with which we were to build our model. We were also given a test dataset with no target prices. The goal was to iteratively build (hopefully better and better) models to increase our predictive performance. We were invited to submit up to 10 prediction sets to Kaggle per day. Kaggle kept a leader board with the running Tally's. 

## Approach
My approach was  to first build a simple linear regression model using the numeric columns in the dataset, and upload an initial prediction. That was my baseline score that I attempted to beat. Using the techniques we have learned in class to date, I  selected features to include or exclude, analyzed the scores of each model, and made revisions to to see if I could improve. I didn't win, but I held my own. This project details the steps in the process, and is summarized with a final report that provides details about which features are most important in predicting home prices.

## Overview of the Data
Data set contains information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010.

SOURCES:  Ames, Iowa Assessor’s Office
NAME: AmesHousing.txt
TYPE: Population
SIZE: 2930 observations, 82 variables
A complete overview of the data can be found here: Ames Housing Data Dictionary

### This project contains the following:
```
\code - Two jupyter notebooks
 
1. Cleaning_and__model_prep 
This is where I explore and clean the data, and create baseline linear regression models. 

2. Modeling_and_results.ipynb 
This is where I use LassoCV and RidgeCV to build a better model by reducing (Ridge) or eliminating(Lasso) features that aren't contributing to the model. 

\data - interim cleaned datafiles  

\datasets - the original data provided

\models - saved models for future use
```

### Summary of conclusion and next steps
The model did tell us which features it determined were most predictive, which begin to answer the question of what features are most important for predicting home prices. It suggests that ***while location is important, size and quality are the most important.***

More could be done, however, to improve the model. I would like to do a deeper exploration the data by category, transform ranking variables differently than continous numeric variables, run polynomialfeatures to create and evaluate interaction terms, and create interaction terms manually. I would also like to build a series of pipelines to make it easy to build and test these models in batch. 