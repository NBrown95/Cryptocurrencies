# Cryptocurrency Analysis

## Overview of Project

For this project, we are creating a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for a new cryptocurrency investment portfolio. There is no known output for what we are looking for, so we are using unsupervised machine learning algorithms to group the cryptocurrencies. Then, we visualized the findings with scatterplots.

## Preprocessing

First, we preprocessed the dataset. We kept all they cryptocurrencies that are being traded and dropped null rows and the column that indicates if the cryptocurrency is being traded. We also removed the coin name column to ease the clustering process. We used get_dummies() to get binary numbers instead of text features. We scaled this data using StandardScaler to standardize the features. 

## PCA

Then, we applied PCA to reduce the dimensions to three principal components. We then created a new dataframe that showed the three principal components.

## K-means

We then created an elbow curve to find the best value for K. It was clear that K should be equal to 4 and we used the K-means algorithm to make predictions of the K clusters for the data. We then created a new dataframe that combined the clustered dataframe with the pca one. 

## Visualization

We created a 3D scatter plot to plot the three clusters from the PCA dataframe. We then created a sortable table with the tradable cryptocurrencies. Finally, we created a scatter plot to show the total coin supply and total coins mined by their class.
 
