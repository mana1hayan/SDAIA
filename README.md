# Women's Fashion Ratings and Reviews
Manal Abdulaziz Alhayan


## Abstract 
Online ratings and reviews play a main role for business revenues since customers usually write about their experiences whether positive or negative when purchasing a product through online services. This means the more complimentary reviews the better income for businesses, but some buyers are dissatisfied with the quality of products, causing adverse consequences for the business since online shoppers can be persuaded through those negative reviews for not buying unrecommended clothes. Thus, the main objective of this project is to enhance products based on customers reviews using one category of machine learning methods which is supervised. The used data is available in Kaggle, labeled using Sentiment analysis model, and evaluated by Naive Bayes classifier. The overall accuracy is 93%, but since we have imbalanced dataset, the official metric is F-score, achieving 96% with positive or satisfying reviews. 

## Design 
To address the above issue, adverse and helpful reviews should be determined in order to meet customers satisfaction and maintain a good business by machine learning methods (ML). To illustrate, we will classify text reviews based on sentiment Analysis method (SA) by using one of ML methods which is supervised, so that satisfying and dissatisfying reviews can be distinguished.


## Data
The Women's Fashion Reviews dataset has been acquired from kaggle as a .csv file, containing 23486 rows and 10 features. To address the issue, we select the two top relevant features, which are the Review Text, and Rating columns. In the Review text feature, consumers have been written about their experience with the quality of clothes, and the other feature is determined customers' rating scale from 1 till 5, which is used in our project to label data for Sentiment Analysis tools. In addition, other features have been used for a business insight to determine the most and least selling items and the distribution of age group such as Age,Recommended IND, and Department_Name.


## Algorithms 

###### Feature Engineering: 
- The Text Review feature have been cleaned by removing all punctuations, numbers, a word that has length <= 2 , stopwords and lowering the word.
- Labeled data have been gotten by using the Rating feature, where one and two star ratings indicate dissatisfying reviews, 3 means moderate, and when assigning 4 and 5 ratings, it means satisfying reviews. Moderate reviews have been dropped due to sentiment analysis, so that so that 0 is dissatisfying reviews and 1 is satisfying reviews.
- The most common words in dissatisfying reviews have been counted using a bag of word, implying for several things. For instance, size, small, and wear were most frequent words and this might imply for complaining about sizes, as a result US and UK size charts should be included in the website. In addition, Frequent Fabric, and Material words might indicate that customers were dissatisfied with the quality of products, consequently types of fabric should be included in detail. Moreover, looked, look, like , love words showed high frequency, which might imply that the Item not the same as in pictures, this High resolution image should be posted.

###### Model Selection and Evaluation:
- Naive Bayes model have been used to classify the text reviews. The precision, recall, and F1 score were selected to evaluate our model due to imbalanced dataset as shown in the below picture:  
 ![Picture1](https://user-images.githubusercontent.com/93191265/141857467-52cc1496-e02d-4ba6-b98c-57e20b82f639.png)

## Tools
- Pandas for loading data and applying functions.
- Scikit-learn for modelling.
- NLTK for natural language processing.
- re, string for for data cleansing. 
- Matplotlib, Seaborn for visualizing data.

## Communication
Presentation: [Click](https://github.com/mana1hayan/SDAIA/blob/main/Presentation/Online%20clothes'%20reviews.pdf)
