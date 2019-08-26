This repository is a model to predict the housing prices in the King County region.
I used markdown headers and sub-headers to organize my code.
I will put a "directory" style in this readme file for reference of where to find parts of my code.

// A red and black arrow indicates one of my three EDA questions, The answers to each will be at the bottom in my conclusion //

__Section 1 - Aliasing the software__
 This is just the basic imports and loading all the frameworks I needed for my model.

__Section 2 - Dealing with NANs and Missing Data__ 
 Here I checked for nans in the df and any other outliers that need to be dealt with. Below that is the code for each column that was affected by NaNs and how I executed each column to fit into the final model.

__Section 3 - Categorical Variables__
 Here, I seperated the columns that were continuous or categorical. Then, I visualized several variables to check the trends in the dataset, and I also dropped columns that seemed unlikely to help me in my regression based on EDA.

__Section 4 - Dealing With Categoricals__
 After identifying what columns were categorical, I took a different approach based off each column. Mostly dummy but a few one-hot encoding as well.

__Section 5 - Visualization__
 Ran each of the continous variables through a scatter plot vs price, a couple box plots to see what else needed to be transformed and a quick "price intensity" map to look at the price based off of the location in King County.

__Section 6 - Correlation and Collinearity__
 Here I checked the correlation with the existing price column and how much weight each column had to get an idea of what significant variables to use in my final model. I also made a heat map of those correlations to use in my presentation so it could be easily understood why I used those variables.

__Section 7 - Min Max and Log Transformations__
 Made a histogram for the continuous data so I could see what columns needed to be logged and scaled. Then, I scaled each columns I would be using in my model.

__Section 8 - OLS Regression Results__
 Checking for R-Squared and p-values of newly edited dataframe. This is where I started having trouble with my code, (maybe a problem with my cleaning methods?).


__Section 9 - Train-Test Split__
 Trained the model and got my Mean Squared Error here. I then evaluated more with a Train Test Scatter plot and utalized a stepwise selection function to verify what variables to use.

__Section 10 - Cross Validation and Prediction__
 Ran a cv_10 of the model to get my neg-MSE and prediction for the dataset.

__Section 11 - Concluding Paragraph__
 In this last section, I answered the questions I came up with while performing my EDA and a general summary of why I chose to do the model in this way.