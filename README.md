# Spotify_Analysis

In this project I am using the "Top 200 Weekly Global Charts On Spotify" from Kaggle which can be found here: https://www.kaggle.com/datasets/sashankpillai/spotify-top-200-charts-20202021/code. 
This particular dataset contains the top 200 songs that have been played most frequently based on several attributes. However, for this particular 
exploratory analysis I will only be analying the top 10. In order to explore this data I had to clean the data utilizing functions to drop columns, 
remove unique values, correct data types, as well as dropping null values. Afterwards, I assess the data using graphs to find correlations as well as 
the significance certain attribute may have as contributing factors for a song being considered a top 10 streaming song. All of which aided in discovering 
which attribites compose opitmal results in streams. The findings were that the some characteristics impacted the number of times streamed. It was discovered that streams are primarily dependent on its sound characteristics and energy levels. Followers seemed to have the least impact in regards to streams.

Model development: Based on using different features and my target "Streams" I have created 2 versions of models using RandomForestRegression, and LinearRegression. It appears that the hypertuned version of the RandomForestRegression would be best since it received the best score for Streams.

Below is an overview of my findings:

The original score for RandomForestRegression:

Training accuracy: 0.965853733901256
Testing accuracy: 0.8745045406666199

With Hypertuning the score slightly increased to:

Training accuracy: 0.9684868278552011
Testing accuracy: 0.873736178764275

The original score for LinearRegression:

Training accuracy: 0.1561831274632005
Testing accuracy: 0.17056333091707043

Linear Regression with Hypertuning, it improved slightly. However, still maintains a low score:

Training accuracy: 0.15999720440086207
Testing accuracy: 0.16587903261320358
