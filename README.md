# California Price Prediction

## Objective

#### Build
Build a model framework to predict median house values in California using the provided dataset.

#### Train
Train the model to learn from the data to predict the median housing price in any district, given all the other metrics.


#### Predict
Predict housing prices based on median income and plot the regression chart for it.


## Data Description

There are 20,640 districts in the project dataset. Districts or block groups are the smallest geographical units for which the US Census Bureau publishes sample data. Note that a block group typically has a population of 600 to 3,000 people. 

Dataset Description & Info
![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/e4efa0c1-2765-4c9e-9fe6-7c71eeb69715) ![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/d222d250-10ce-405a-a856-54377c46dedf)


## Method for Cleaning & Wrangling
- Missing values were treated with the  mean of the respective feature. Categorical columns in the dataset were converted to numerical data. 

- The data was split into 80% training dataset and 20% test dataset. The data was standardized into training and test datasets and linear regression was performed. 

## Data Cleaning:
The chart below reveals the first few rows of the dataset and shows all the features of the dataset. The median house value will be used as the response once the data is split into features and response. Note that ocean proximity is categorial.

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/dc9d0053-e61c-4f38-abff-7e9662a1428f)

#### This heatmap was used visualize if there were any missing data in the dataset. We can see that the total bedrooms feature is missing some data.

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/2945a73d-91a3-4c05-849d-ead42997b7ec)

#### The missing data was filled in with the mean and with this treatment of missing values we see that the heatmap shows no missing values.

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/a4012592-7453-4004-a3e7-582083611a8e)

#### From the head() function in slide six we can see that ocean proximity does not have numerical observations, thus the get_dummies function was used to generate dummy values in order to use the feature to produce an accurate and inclusive model . The view below shows the ocean proximity values numerically.
![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/5b081463-5a0a-42c3-9871-05f49e9bf844)


## Data Wrangling:

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/763262fe-9769-47eb-b70f-23bd5523ec16)


## Correlation Plot

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/953a5477-9b72-4a08-ae25-de63855cf0e8)

## Multiple Linear Regression Analysis

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/8ad0d52b-7e63-4e6e-aff1-2088aa96bd2f)

- The model generated use the coefficients shown in the table. Each feature was used to develop the model as a contributing factor to the median house value.
- Median House Value= 206605.10895107 -53832.019953 β1 -55144.206003 β2 +13375.841699 β3 -8008.168495 β4 + 30659.086456 β5-50543.036221 β6 +32789.588389 β7+73061.679934 β8-18341.261361 β9 +2646.295627 β10 -989.350756 β11+1537.608747 β12 


![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/98e1d463-aec6-4f2a-a9e6-4576c6e70c6a)


## Prediction
The model was used to predict median house values as shown in the scatter plot . 

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/bef25db2-142e-4ec8-8976-57ff213d5584)

## Error Analysis
![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/01eccb3e-80e4-42b5-8cf0-ce461ff6a335)

The root mean squared error indicates the measure of how concentrated the data is around the regression line which is the best line of fit. The RMSE was found to be 72439.86634739453.

### Median Income feature was used to predict median house value and the plots show a visual on how role of median income influence median house value.

![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/55f15c67-bef6-4732-9cfb-d2694b05747d)
![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/3222f31a-52a7-4099-909c-e06f7882308f)
![image](https://github.com/caand4/California-Price-Prediction/assets/80293132/d56cc0f2-a1cb-4108-bc57-0fd734ae752a)

# Conclusion

In this project, a model was built to predict median house values in California using the provided dataset. This model learned from the data in order to predict the median housing price in any district, given all the other metrics.
The model shows how all the features provided in the dataset influence median house values.





























