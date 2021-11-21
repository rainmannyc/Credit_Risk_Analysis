# LOAN PREDICTION ANALYSIS 

# Overview of the analysis: Explain the purpose of this analysis.

The purpose of the analysis was to classify credit risks from the Lending Club dataset to more accurately determine risky and non-risky loans. We ran our analysis through six machine learning models and have summarized our results below.

# The Machine Learning Models

In our first model, we explored a Naive Random Oversampling model, a logistic regression model which yielded the following results:

* Balance Accuracy Score: 0.628
* Precision Score: 0.99
* Recall score: 0.64
* F1 score: 0.78

Naive Random Oversampling Confusion Matrix:

<img>

For our second model we examined a SMOTE Oversampling model, another logistic regression model which yielded us the following results:

* Balance Accuracy Score: 0.625
* Precision Score: 0.99
* Recall score: 0.67
* F1 score: 0.80

SMOTE Oversampling Confusion Matrix:

<img>

On our third model, we explored an Undersampling model with undersampling algorithms. We used the Clustering Centroids algorithm to yield the following results:

* Balance Accuracy Score: 0.514
* Precision Score: 0.99
* Recall score: 0.45
* F1 score: 0.58

Undersampling Confusion Matrix:

<img>


Our fourth model was carried out using a combination of Oversampling and Undersampling algorithms. We used a SMOTEENN algorithm to yield the following results:

* Balance Accuracy Score: .604
* Precision Score: 0.99
* Recall score: 0.56
* F1 score: 0.65

SMOTEENN Confusion Matrix:

<img>

## Ensemble Learners: Balanced Random Forest Classifier & Easy Ensemble AdaBooster Classifier

For our first Ensemble learning model, we ran a Balanced Random Forest Classifier with the following results below:

* Balance Accuracy Score: 0.996
* Precision Score: 0.88
* Recall score: 0.70
* F1 score: 0.76

Balanced Random Forest Classifier Confusion Matrix:

<img>

Our second Ensemble model and our final model is the Easy Ensemble AdaBooster Classifier:

* Balance Accuracy Score: 0.920
* Precision Score: 0.99
* Recall score: 0.95
* F1 score: 0.97

Easy Ensemble AdaBooster Classifier Confusion Matrix:

<img>

# Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

All in all, all models performed above 60% accuracy apart from our Undersampling model which had the lowest accuracy score and underperformed at 51% and an F1 score of only .58. This would be a model I would not recommend.

For a model I would recommend, would be either one of our Ensemble Learners, with more favor leaning towards the Easy Ensemble AdaBooster Classifier model which yielded excellent results! However, the Random Forest model did also perform very well with a higher balanced accuracy score of 0.996, almost perfect! 