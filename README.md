# Prediting a salary (focusing on pre-modeling)

According to [[1]](https://www.infoworld.com/article/3228245/the-80-20-data-science-dilemma.html),80 percent of a data scientist’s valuable time is spent simply finding, cleaning and reorganizing huge amounts of data. Moreover, the quality of pre-modeling data such as: data preprocessing, feature exploration, feature engineering dirrectly affect to the performance of machine learning model. Therefore, in this project, I want to pay attention to `pre-modeling steps`. 

The data used in this project was extracted from the census [bureau database](http://www.census.gov). The original database came from the [Adult Data Set](https://archive.ics.uci.edu/ml/datasets/Adult) from UCI Machine Learning Repository.

The bussiness problem of this project is to clasify a salary of person. This is binary classification problem if an income of a person greater or smaller than a threshold value (50k USD). This problem could be applied to a recommendation system of some online e-commerce sites such as Amazon or Rakuten. If a person's income is below a certain threshold salary, the product suggestion system will adjust suggested products according to her/him salary in the way that he/she are more likely to purchase the product. Another business case of this problem is understanding and segmenting a customer to pay more attention to some specific group of customers in promotional campaigns or introdution of new products.

**In this project, I will analyze the data carefully to find correlations between an income with other factors, then pre-process the data and build a machine learning model. This is end-to-end binary classification problem.**


### Outline of this project
[**1.Introduction - Problem Definition**](#part1)

[**2. Pre-Modeling**](#part2)
   - [2.1. Data exploration (Exploratory data analysis or EDA)](#2.1)
       - [A. General statistic of our dataset](#2.1a)
       - [B. Explore details of each feature and correct the missing information](#2.1b)
       - [C. Analysze by visualizing relation of combined features](#2.1c)
   - [2.2. Data cleaning](#2.2)
       - [A. Handling data type](#2.2a)
       - [B. Outlier detection](#2.2b)
       - [C. Missing values](#2.2c)
    
[**3. Model building**](#part3)
   - [3.1. Selecting models](#3.1)
   - [3.2. Hyperparameter tuning](#3.2)
   - [3.3. Evaluate results and choose the best model](#3.3)
      
[**4. Conlusion**](#part4)

[**References**](#ref)