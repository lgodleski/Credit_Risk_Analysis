# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to use machine learning models to predict credit risk.


## Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
   - Naive Random Oversampling
     - ![](Resources/naive_random_accuracy.png)
     - When using the Naive Random Oversampling algorithm, we had a balanced accuracy score of .6547 or 65.47%. 
     - ![](Resources/naive_random_classification.png)
     - The overall precision score for this algorithm is very high at 99% and the recall is lower at 59% which tells us that the predicted positives are likely true positives but a number of other true positives may not have been predicted using this algorithm. 
   - SMOTE Oversampling
     - ![](Resources/smote_accuracy.png)
     - When using the SMOTE Oversampling algorithm, we get a balanced accuracy score of 66.2%.
     - ![](Resources/smote_classification.png)
     - Again we see a very high precision score of 99% and a recall score of 69%. The predicted positives are likely true positives but there may be a number of true positives that were not predicted using this algorithm. 
   - Undersampling
     - ![](Resources/undersampling_accuracy.png)
     - When using the Undersampling algorithm, we get a balanced accuracy score of 54.4%. 
     - ![](Resources/undersampling_classification.png)
     - The precision score for this algorithm is very high 99% and the recall score is low at 40%. The predicted positives are likely true positives but there may be a number of true positives that were not predicted using this algorithm. 
   - Combination Sampling (SMOTEENN)
   - 
   - Balanced Random Forest Classifier
   - Easy Ensemble AdaBoost Classifier

## Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
