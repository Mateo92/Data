# Overview

For this project we have two data sets(the data sets may be downloaded from https://www.kaggle.com/c/house-prices-advanced-regression-techniques), each containing information on 1,459 houses in a single city (Ames, Iowa), including 79 variables for each house. The first data set is intended for training our models, while the second is for testing them out. Our goal is to find the best regression model to predict the price of each home. Before modelling the data, we must:

1-Frame the problem and look at the big picture.

2-Prepare the data, checking for faulty entries (empty cells or cells with "nan"s or other values that do not make sense in the context of the problem) and dealing with them.

3-Explore the data with visual tools to gain some insight and intuition.

# 3. Data Analysis

Once we obtain the correlation matrix with the prepared data set, we are able to determine which features are relevant (and useful) to perform the regression models fitting. The theoretical and computational procedure we implement consists in two steps: first choose a set of features that have a correlation with the sale price greater than certain amount $n_{SP}\in(0,1),$ secondly check each feature couple from this set and compute their correlation, if it is greater that certain amount $n_{corr}\in(0,1)$ then remove the feature that has less correlation with the sale price. This procedure is mean to reduce milticollinearity and improve the linear regression methods.
