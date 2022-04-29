# Spotify_Analysis

In this project I am using the "Top 200 Weekly Global Charts On Spotify" from Kaggle which can be found here: https://www.kaggle.com/datasets/sashankpillai/spotify-top-200-charts-20202021/code. 
This particular dataset contains the top 200 songs that have been played most frequently based on several attributes. However, for this particular 
exploratory analysis I will only be analying the top 10. In order to explore this data I had to clean the data utilizing functions to drop columns, 
remove unique values, correct data types, as well as dropping null values. Afterwards, I assess the data using graphs to find correlations as well as 
the significance certain attribute may have as contributing factors for a song being considered a top 10 streaming song. All of which aided in discovering 
which attribites compose opitmal results in streams. The findings were that the some characteristics impacted the number of times streamed. It was discovered that streams are primarily dependent on its sound characteristics and energy levels. Followers seemed to have the least impact in regards to streams.

Model development: Based on using different features and my target "Streams" I have created a variation of models including KMeans, Logistic Regression, KNN, Logistic Regression, Random Forrest, all of which have been tuned with and without PCA(s). Upon reviewing all of these models it appears that the Random Forrest model without a PCA had the best performance and production as it was the closest to the original streams.

Below is an overview of my findings:

Findings and choice of production model:
KMeans model with 2 clusters performance: 0.18363826197079378

Logistic Regression with PCA: 0.9490500863557858

Logistic Regression without PCA: 0.9879101899827288

KNN Model with PCA: 0.18393782383419688

KNN Model without PCA: 0.18998272884283246

LinearRegression with PCA:

Training: 0.16592114659779855 Test: 0.11571676362065952

LinearRegression without PCA:
Training: 0.1666819894170397 Testing: 0.11021787508223613

Random Forrest with PCA:
Train: 0.9048820668318618 Test: 0.29045111948431046

Random Forrest without PCA:
Train: 0.9763793466688971 Test: 0.8331243767892835

The KMeans, KNN, Linnear regression models would not be useful models as they scored below 60% in the teen number ranges. Their performance was dissatisfactory.

The Logistic regression without PCA performed well with a 0.98%
