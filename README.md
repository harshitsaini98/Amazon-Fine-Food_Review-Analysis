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
