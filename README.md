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

![naive_cm](https://github.com/rainmannyc/Credit_Risk_Analysis/blob/e5b603f2bd932ef489f6984fe98cd9a342ec9abf/Resources/naive_cm.png)


For our second model we examined a SMOTE Oversampling model, another logistic regression model which yielded us the following results:

* Balance Accuracy Score: 0.625
* Precision Score: 0.99
* Recall score: 0.67
* F1 score: 0.80

SMOTE Oversampling Confusion Matrix:

![smote_cm](https://github.com/rainmannyc/Credit_Risk_Analysis/blob/e5b603f2bd932ef489f6984fe98cd9a342ec9abf/Resources/smote_cm.png)

On our third model, we explored an Undersampling model with undersampling algorithms. We used the Clustering Centroids algorithm to yield the following results:

* Balance Accuracy Score: 0.514
* Precision Score: 0.99
* Recall score: 0.45
* F1 score: 0.58

Undersampling Confusion Matrix:

![undersampling_cm](https://github.com/rainmannyc/Credit_Risk_Analysis/blob/e5b603f2bd932ef489f6984fe98cd9a342ec9abf/Resources/undersampling_cm.png)


Our fourth model was carried out using a combination of Oversampling and Undersampling algorithms. We used a SMOTEENN algorithm to yield the following results:

* Balance Accuracy Score: .604
* Precision Score: 0.99
* Recall score: 0.56
* F1 score: 0.65

SMOTEENN Confusion Matrix:

![smoteenn](https://github.com/rainmannyc/Credit_Risk_Analysis/blob/e5b603f2bd932ef489f6984fe98cd9a342ec9abf/Resources/combo_cm.png)

## Ensemble Learners: Balanced Random Forest Classifier & Easy Ensemble AdaBooster Classifier

For our first Ensemble learning model, we ran a Balanced Random Forest Classifier with the following results below:

* Balance Accuracy Score: 0.996
* Precision Score: 0.88
* Recall score: 0.70
* F1 score: 0.76

Balanced Random Forest Classifier Confusion Matrix:

![r_forest_cm](https://github.com/rainmannyc/Credit_Risk_Analysis/blob/e5b603f2bd932ef489f6984fe98cd9a342ec9abf/Resources/r_forest_cm.png)

Our second Ensemble model and our final model is the Easy Ensemble AdaBooster Classifier:

* Balance Accuracy Score: 0.920
* Precision Score: 0.99
* Recall score: 0.95
* F1 score: 0.97

Easy Ensemble AdaBooster Classifier Confusion Matrix:

![easy_e_cm](https://github.com/rainmannyc/Credit_Risk_Analysis/blob/e5b603f2bd932ef489f6984fe98cd9a342ec9abf/Resources/easy_e_cm.png)

# Conclusion

All in all, all models performed above 60% accuracy apart from our Undersampling model which had the lowest accuracy score and underperformed at 51% and an F1 score of only .58. This would be a model I would not recommend.

For a model I would recommend, would be either one of our Ensemble Learners, with more favor leaning towards the Easy Ensemble AdaBooster Classifier model which yielded excellent results! However, the Random Forest model did also perform very well with a higher balanced accuracy score of 0.996, almost perfect! 