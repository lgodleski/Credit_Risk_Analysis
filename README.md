# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to use machine learning models to predict credit risk.


## Results
   - Naive Random Oversampling
     - ![](Resources/naive_random_accuracy.png)
     - When using the Naive Random Oversampling algorithm, we had a balanced accuracy score of .6547 or 65.5%. 
     - ![](Resources/naive_random_classification.png)
     - The overall precision score for this algorithm is very high at 99% but when looking at the precision for predicting high-risk loans specifically, the precision is only 1% vs. 100% for predicting low-risk. The overall recall is lower at 59%, with a 72% recall score for high-risk loans and a 59% recall score for low-risk.
   - SMOTE Oversampling
     - ![](Resources/smote_accuracy.png)
     - When using the SMOTE Oversampling algorithm, we get a balanced accuracy score of 66.2%.
     - ![](Resources/smote_classification.png)
     - Again we see a very high precision score of 99% but only 1% for high-risk and 100% for low-risk loans. The overall recall score of the algorithm is 69%, with a 63% recall score for high-risk and a 69% recall score for low-risk.
   - Undersampling (Cluster Centroids)
     - ![](Resources/undersampling_accuracy.png)
     - When using the Cluster Centroids algorithm, we get a balanced accuracy score of 54.4%. 
     - ![](Resources/undersampling_classification.png)
     - The overall precision score for this algorithm is very high 99% but 1% for high-risk and 100% for low-risk loans. The overall recall score is low at 40%, with a 69% recall score for high-risk loans and 40% for low-risk.
   - Combination Sampling (SMOTEENN)
     - ![](Resources/smoteenn_accuracy.png)
     - When using the SMOTEENN algorithm, we had a balanced accuracy score of 66.6%
     - ![](Resources/smoteenn_classification.png)
     - The overall precision score is very high at 99%, with 1% precision score for high-risk and 100% for low-risk loans. The overall recall score is 61%, with 72% recall score for high-risk and 61% for low-risk. 
   - Balanced Random Forest Classifier
     - ![](Resources/balanced_forest_accuracy.png)
     - When using the Balanced Random Forest Classifier we had a balanced accuracy score of 78.9%. 
     - ![](Resources/balanced_forest_classification.png)
     - The overall precision score for this algorithm is very high at 99%, with 3% precision score for high-risk loans and 100% for low-risk. The overall recall score is also high at 87%, with a 70% recall score for high-risk and 87% for low-risk. 
   - Easy Ensemble AdaBoost Classifier
     - ![](Resources/easy_ensemble_accuracy.png)
     - When using the Easy Ensemble AdaBoost Classifier we had a balanced accuracy score of 93.2%
     - ![](Resources/easy_ensemble_classification.png)
     - The overall precision score for this algorithm is very high at 99%, with 9% precision score for high-risk loans and 100% for low-risk. The overall recall score is also very high at 94%, with a 92% recall score for high-risk and 94% for low-risk. 

## Summary

When predicting credit risk, we are looking for a machine learning model that has a high recall score because these algorithms detect the intended target but risk resulting in false positives. Looking at the results of each model, we can see that by using Naive Random Oversampling, SMOTE Oversampling, Undersampling, and SMOTEENN we get very high precision scores, with a big disparity between low-risk and high-risk, and generally low recall scores. This tells us that the algorithm is predicting almost all loans as low-risk so the predicted positives are likely true positives but a number of other true positives are not being predicted. The Balanced Random Forest Classifier algorithm follows a similar pattern but the recall score is significantly higher. The Easy Ensemble Classifier has the highest accuracy score, a high precision score, and the highest overall recall score of 94%. For these reasons, I recommend using the Easy Ensemble AdaBoost Classififer algorithm. 

