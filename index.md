## Abstract

We propose to study the power of random forest in predicting rare events in another field. We will use a dataset recording direct marketing campaigns (bank term deposit) of a Portuguese banking institution. The subscriptions of the bank term deposit are based on phone calls, so this is a rare event. We plan to apply random forest and logistic regression method to predict if a client will subscribe a term deposit in the bank, and compare their predictive accuracies. Then, we will analyze the causal effects in the subscription of a term deposit from a bank. Finally, we could indicate which clients are more likely to subscribe for term deposits.

## Research questions
1. What is the accuracy of random forests in predicting the rare event in a new filed?

2. Can random forests predict the subscriptions of the bank term deposit efficiently and generally?

3. To what extent does random forest outperform logistic regression method in predicting the rare events, subscription of the bank term deposit?

4. Is there a causal effect of a client subscribing a bank term deposit?

5. What is the most important factor affecting a client subscribe a term deposit? Which clients are more likely to subscribe a term deposit?

## datasets
-	bank-additional-full.csv from “Bank Marketing Data Set” UCI machine learning repository. There are 41188 observations each with 20 features such as a client’s age, sex and job. The observations are ordered by date (from May 2008 to November 2010). The dependent variable is ‘y’ indicating whether a client subscribe the bank term deposit. 
The dataset is highly imbalanced because few people subscribe the bank term deposit. The ratio of subscribed (‘Yes’) bank term deposit and not ('no') subscribed in the data is roughly 1:8. In addition, there are missing or unknown values such as ‘education’, ‘housing’ and ‘loan’ in the dataset because some people would not like to tell their private information to the banking representative. We will discard the rows containing missing values. 

## Methods
Data collection: (a) Collect the dataset from UCI Machine learning Repository (b) Discard the rows containing missing values in the dataset (c) Determining the categorical features and numerical features (d) Visualize the relationship between features and dependent variable y (e) Get the proper features

Building the logistic regression model: After getting the proper dataset and features, we will use these data to build three logistic regression models with no regularization, L1 norm and L2 norm regularization, respectively. Then we use ten-fold cross validation to plot the ROC curve, and calculate the AUC score and F1 score of each model. Finally, we will get the best model.

Building the random forest model: After selecting proper features, we will build a random forest model with different hyperparameters. We will test different hyperparameters, and use ten-fold cross validation to calculate the average accuracy with 95% confidence intervals. Then, we select the best hyperparameters. 

Compare logistic regression model and random forest model: We use ten-fold cross validation to plot the ROC curve, and calculate the AUC score and F1 score of the best logistic regression model and the best random forest model respectively. Then, we compare the results.

Data analysis: We will visualize the variable importance by mean decrease in Gini Score of random forest model. Second, we analyze the importance of the features. Third, we will draw the partial dependence plots. We will analyze how the percentage of total votes for subscribing the bank term deposit changes over the range of each predictor. Finally, we summarize the causes of subscribing bank term deposits. Also, we indicate which clients are more likely to subscribe the bank term deposit.

## Data preprocessing

### 1.0 Data Visualization
### 2.0 Data Nummerize and Standardization
### 3.0 unknown filling

## Model and implementation
### Logistic Regression
### Random Forest
### Data Analysis and Visulization
#### 1.0 ROC Curve
#### 2.0 Importance of variables
#### 3.0 Result Compare



[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/LIUQyou/ADA_P4/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
