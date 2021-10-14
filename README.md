# Data

# 3. Data Analysis

Once we obtain the correlation matrix with the prepared data set, we are able to determine which features are relevant (and useful) to perform the regression models fitting. The theoretical and computational procedure we implement consists in two steps: first choose a set of features that have a correlation with the sale price greater than certain amount $n_{SP}\in(0,1),$ secondly check each feature couple from this set and compute their correlation, if it is greater that certain amount $n_{corr}\in(0,1)$ then remove the feature that has less correlation with the sale price. This procedure is mean to reduce milticollinearity and improve the linear regression methods.
