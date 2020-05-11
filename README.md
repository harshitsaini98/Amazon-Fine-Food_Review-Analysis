# Amazon-Fine-Food_Review-Analysis
The Amazon Fine Food Reviews dataset consists of 568,454 food reviews Amazon users left up to October 2012.

The purpose of this analysis is to make up a prediction model where we will be able to predict whether a recommendation is positive or negative. In this analysis, we will not focus on the Score, but only the positive/negative sentiment of the recommendation

# Problem Statement
Given a review, determine whether the review is positive (Rating of 4 or 5) or negative (rating of 1 or 2).

# Source
* https://www.kaggle.com/snap/amazon-fine-food-reviews
* Number of reviews: 568,454
* Number of users: 256,059
* Number of products: 74,258
* Timespan: Oct 1999 - Oct 2012
* Number of Attributes/Columns in data: 10

# Attribute Information
* Id
* ProductId - unique identifier for the product
* UserId - unqiue identifier for the user
* ProfileName
* HelpfulnessNumerator - number of users who found the review helpful
* HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
* Score - rating between 1 and 5
* Time - timestamp for the review
* Summary - brief summary of the review
* Text - text of the review

# Data Preprocessing
* Remove Special characters
* Remove stop words
* Remove HTML Tags
* Removing null coloumn

# Splitting Data
## Time based Splitting into train,cv and test
* Train-60
* cv-20
* test-20

# Applying various Machine Learning models
# Naive Bayes 
* Featurize the text data using the previous technique.
* Tuned hyperparameter to get best alpha and plotted the graph at each iteration.
* Obtained top 10 +Ve and -Ve features


![myimage-alt-tag](https://camo.githubusercontent.com/4c76daea0720266c597328122e923c04683c99c9/68747470733a2f2f692e696d6775722e636f6d2f4954796d4237552e706e67)

## conclusion
* Naive bayes are good at text classification task like spam filtering, sentimental analysis, RS etc.
* As we know when a model performs good on training data but poor performence on unseen data(test data)i.e. its dependent on training     data only, tends to overfits and when a model perform poor performence on training data and good performence on test data i.e. it       fails to learn relationship in training data tends to underfit. We need to balance between both i.e. reduce training error and balance   error between both training and testing which is balanced in this case.
* Another concept bias vs variance is also related with underfitting and overfitting. when a model has high bias and low variance tend     to underfitting and its reverse- high variance and low bias called overfitting and we balanced using cross-validataion. As it is shown   in below table where both models have low trainig error and test error.



