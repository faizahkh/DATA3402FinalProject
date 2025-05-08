## Mushroom Classification using decision tree classifier
# Overview
* This repository holds an attempt to use decision tree classifiers and method to the features of mushrooms given in a dataset, in the Mushroom Classification Kaggle Dataset: https://www.kaggle.com/datasets/uciml/mushroom-classification/data
* The approach in this repository formula was to take the idea of classification and use it on varous species of mushrooms to see predict mushroom's 'edibility'.
* Summary: The decision tree classifier method predicted the edible state with 1.0 (100%) accuracy within the model, given that it was a dataset with minimal missing values. The factors 
## DATA
* Data type: categorical; tabular data (CSV file)
* Size: 8124 rows, 23 columns/features
* Instances (Training: 4863, Validation: 1621, Testing: 1622)
# Cleaning up data/pre-processing
* The data was fairly clean with very minimal missing values. In this case, I had the feature called "stalk-root", which had a '?' in place of a characteristic in it so I were able to change those unknown values to create and replace with class value/mode (written in code)
* ![stalk picture](stalk.png)
* ![after stalk](afterstalk.png)
* Additional features, such as gill-attach and veil-type were removed because they had very little significance to the overall dataset and would cause a shift in training the model.
# Data Visualization
* I decided to go ahead and use a code that would be able to showcase all the graphs with their respective categories and features, and the letters that correspond to the variables. There is a distinct measure of multiple types of features and frequencies of each characteristic of the mushrooms and how to use it for training dataset.
* ![frequency](color.png)
* ![class](classdist.png)
# Problem
* The inputs were: mushroom characteristics and features
* Output was: prediction of being edible as a mushroom
* Model: Basic decision tree classification since it made value simpler to understand and code with through cleaned up data.
* Trained with normal parameters, no hyper tuning parameters used.
# Conclusions:
* Got an accuracy of 1.00 which was attainable given simpler data and less processing. The model should predict edible mushrooms 100% of time using the model and accuracy results.
* ![accuracy](precision.png)
# Reproducing Results: 
* Seperate features and perform one-hot encoding of categorical variables, create a new clean dataset.
* Use the decision tree classifications.
* Convert unknown variables in stalk-root feature.
* Use 'sklearn' and get rid of columns that might affect the fitting; pre-process and visualize all the categories beforehand.
# Repository files:
* README file
* MushroomKaggleChallenge.ipynb file
# Software:
* pandas as pd
* numpy as np
