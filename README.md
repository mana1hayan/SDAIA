# Women's Fashion Ratings and Reviews
Manal Abdulaziz Alhayan


## Abstract 
Online ratings and reviews play a main role for business revenues since customers usually write about their experiences whether positive or negative when purchasing a product through online services. This means the more complimentary reviews the better income for businesses, but some buyers are dissatisfied with the quality of products, causing adverse consequences for the business since online shoppers can be persuaded through those negative reviews for not buying unrecommended clothes. Thus, the main objective of this project is to enhance products based on customers reviews using one category of machine learning methods which is supervised. The used data is available in Kaggle, labeled using Sentiment analysis model, and evaluated by Logistic Regression classifier.

## Design 
The goal of improving products based on customers' reviews in this project has been achieved using the Kaggle dataset. The sentiment analysis method was applied to distinguish between negative and positive reviews. The best and most selling products were determined using positive reviews and the reasons of products dissatisfaction were determined by most common words in negative reviews, implying several issues like quality and sizes. Those steps were applied in detail using [Jupyter Notebook](https://github.com/mana1hayan/SDAIA/blob/main/Final_Project.ipynb) with visualizations.


## Data
The Women's Fashion Reviews dataset has been acquired from kaggle as a .csv file, containing 23486 rows and 10 features. To address the issue, we select the two top relevant features, which are the Review Text, and Rating columns. In the Review text feature, consumers have been written about their experience with the quality of clothes, and the other feature is determined customers' rating scale from 1 till 5, which is used in our project to label data for Sentiment Analysis method. In addition, other features have been used for a business insight to determine the most and least selling items and the distribution of age group such as Age,Recommended IND, and Department_Name.


## Algorithms 

###### Feature Engineering: 
- Cleansing the Text Review feature by removing all punctuations, numbers, a word that has length <= 2 , stopwords and lowering the word, and presenting the length of each text review for cleaning purposes.
- Labeling data using the Rating feature. To ilustrate, one and two star ratings indicate dissatisfying reviews, 3 means moderate, and when assigning 4 and 5 ratings, it means satisfying reviews. Moderate reviews have been dropped due to applying sentiment analysis method.
- Counting the most common words in dissatisfying reviews using a bag of word by SciKit Learn's CountVectorizer, implying for several things. For instance, size, small, and wear were most frequent words and this might imply for complaining about sizes, as a result US and UK size charts should be included in the website. In addition, Frequent Fabric, and Material words might indicate that customers were dissatisfied with the quality of products, consequently types of fabric should be included in detail. Moreover, looked, look, like , love words showed high frequency, which might imply that the Item not the same as in pictures, this High resolution image should be posted.

###### Model Selection and Evaluation:
- Logistic Regression model have been used to classify the text reviews. The model was trained on a 20 test and 80 train. The F1 score was selected to evaluate our model due to imbalanced dataset as shown in the below picture:  
 ![LR](https://user-images.githubusercontent.com/93191265/142176998-675f425e-1167-4a95-a96f-608a93b1b362.png)

## Tools
- Pandas for loading data and applying functions.
- Scikit-learn for modelling.
- NLTK for natural language processing.
- re, string for for data cleansing. 
- Matplotlib, Seaborn for visualizing data.

## Communication
- Presentation: [Click](https://github.com/mana1hayan/SDAIA/blob/main/Presentation/Online%20clothes'%20reviews.pdf)
- Description: [Click](https://github.com/mana1hayan/SDAIA/blob/main/README.md)
