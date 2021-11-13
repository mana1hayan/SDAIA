# Project Proposal Template


## How to improve an online business based on customers’ reviews?
 The main objective of this project is to know what the level of customer satisfaction with the quality of clothes is by applying sentiment analysis. In another words, we can determine if customers are satisfied or dissatisfied with their purchased. We want also to find out what is the most and least selling items, and which age groups favor to buy specific type of clothes as well. 

## Data Description:
 In order to analyze data and obtain our objectives, we use Women's Fashion Reviews, which is available in Kaggle https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews . as the .csv file, and contains 23486 rows and 10 columns. 
The bellow image illustrates a sample of used data: 

 We are going to use two features which are Review Text as a target, and Rating feature to determine customers’ satisfaction, so that when ratting reviews are assigned as 1 or 2, it indicates dissatisfaction, while when reviewers have rated clothes greater than 3, we can infer that customer like items. Since we are going to apply sentiment analysis, we do not need moderate ratings, therefore rating reviews that is equal to 3 will be dropped

## Tools:
Several tools will be applied in this project to help enhancing the business. For instance, pandas’ tool can be used to get the data and apply useful functions. In addition, we can use seaborn to visualize the data, and NLTK for preprocessing data as well. 
Before applying supervised learning, we need to label data as satisfied or dissatisfied for sentiment classification, so Rating feature will be used for labeling data and then we will select appropriate model for obtaining best result.

## TO DO:
- EDA phases including preprocessing data will be used, and then an appropriate model will be selected to fit the data.
- NOTE: Rating feature might be changed to Recommended IND, which have been already labeled in the data, indicating that 0 is unrecommended and 1 is recommended. 




