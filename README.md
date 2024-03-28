## Problem Statement:

We are one of the fastest growing startups in the logistics and delivery domain. We work with several partners and make on-demand delivery to our customers. During the COVID-19 pandemic, we are facing several different challenges and everyday we are trying to address these challenges.

We thrive on making our customers happy. As a growing startup, with a global expansion strategy we know that we need to make our customers happy and the only way to do that is to measure how happy each customer is. If we can predict what makes our customers happy or unhappy, we can then take necessary actions.

Getting feedback from customers is not easy either, but we do our best to get constant feedback from our customers. This is a crucial function to improve our operations across all levels.

We recently did a survey to a select customer cohort. You are presented with a subset of this data. We will be using the remaining data as a private test set.

#### Data Description:

Y = target attribute (Y) with values indicating 0 (unhappy) and 1 (happy) customers
X1 = my order was delivered on time
X2 = contents of my order was as I expected
X3 = I ordered everything I wanted to order
X4 = I paid a good price for my order
X5 = I am satisfied with my courier
X6 = the app makes ordering easy for me

Attributes X1 to X6 indicate the responses for each question and have values from 1 to 5 where the smaller number indicates less and the higher number indicates more towards the answer.

#### Goal(s):

- Predicting if a customer is happy or not based on the answers they give to questions asked.

#### Bonus:

- We are very interested in finding which questions/features are more important when predicting a customer’s happiness. Using a feature selection approach show us understand what is the minimal set of attributes/features that would preserve the most information about the problem while increasing predictability of the data we have.
  
#### Solution employed with metrics:

- **EDA**
  - I first explored the data to gain insights. This included assessing the balance of the data and how many entries we have and how many features. This exploration showed there was no missing data. I then looked at histograms of the distribution of each of the features to better understand the dataset, as well as analyzed the feature importance for each 6 features.

- **Model building**
  - I then built several models: Logistic regression, KNN, Decision tree, Random forest, Gradient boosting, and XGboost. I trained these models using using training data (randomly selected from the whole dataset) at both a 80% and 75% split. I also trained these models using scaled and unscaled data. Finally I tried dropping one or two feature(s) to see if it improved the results of the model 

- **Metrics and results** - 
  - Reached more than 73% accuracy score even with small dataset. Here what we see is that the classical ML model works better than the Neural Network model because of size of data set which is small and neural networks perform better for larger amount of data. And Random forest performs the best as it is based on a series of decision trees reducing overfitting and not massively increasing error due to bias.

  - Also found which features are more important when predicting a customer’s happiness. Using a feature selection approach, it was shown what the minimal set of attributes/features that would preserve the most information about the problem while increasing predictability of the data we have.
