# Women's Fashion Ratings and Reviews



## Problem Statement 
Online ratings and reviews play a main role for business revenues since customers usually write about their experiences whether positive or negative when purchasing a product through online services.This means the more complimentary reviews the better income for businesses, but when some buyers are dissatisfied with the quality of products, this might cause adverse consequences not only for them but also for other customers because online shoppers can be persuaded through those negative reviews for not buying unrecommended clothes. Additionally, businesses often produce new products to meet customer tastes, but successful products might be unintentionally changed, causing a decrease in profits. 


## Design 
To address the above issue, adverse and helpful reviews should be determined in order to meet customers satisfaction and maintain a good business by machine learning methods (ML). To illustrate, we will classify text reviews based on sentiment Analysis method (SA) by using one of ML methods which is supervised, so that satisfying and dissatisfying reviews can be distinguished.


## Data
The Women's Fashion Reviews dataset has been acquired from kaggle as a .csv file, containing 23486 rows and 10 features. To address the issue, we select the two top relevant features, which are the Review Text, and Rating columns. In the Review text feature, consumers have been written about their experience with the quality of clothes, and the other feature is determined customers' rating scale from 1 till 5, which is used in our project to label data for Sentiment Analysis tools. In addition, other features have been used for a business insight to determine the most and least selling items and the distribution of age group such as Age,Recommended IND, and Department_Name.


## Algorithms 
###### Feature Extraction Methods: 
- The Text Review feature have been cleaned by removing all punctuation, numbers, a word that has length <= 2 , stopwords and lowering the word.
- labeled data have been gotten by using the Rating feature, where one and two star ratings indicate dissatisfying reviews, 3 means moderate, and when assigning 4 and 5 ratings, it means satisfying reviews. Moderate reviews have been dropped due to sentiment analysis, so that so that 0 is dissatisfying reviews and 1 is satisfying reviews.


