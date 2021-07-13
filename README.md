# Credit_Risk_Analysis

## Overview:
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

### Resources: 
  - Jupyter Lab (MLENV kernel), Python3.7, Pandas, Scikit-Learn libraries 
  - Resource files and module 17 starter code supplied
  
### Objective:
#### Deliverable 1: Use Resampling Models to Predict Credit Risk
#### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
#### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk


## Results from all Deliverables:
### Naive Random Oversampling results:
   - Our balanced accuracy test is 66%, the precision for the high_risk has a very low positivity at 0.01% and the recall is 58% 
   ![image](https://github.com/antxamp/Credit_Risk_Analysis/blob/main/Image_Resources/naive_random.PNG)
    
### SMOTE Oversampling results:    
   - The accuracy score is 65.3%, the precision for the high_risk loans has a low positvity again at 0.01% and recall is 68% overall
   ![image](https://github.com/antxamp/Credit_Risk_Analysis/blob/main/Image_Resources/smote_oversampling1.PNG)
   
### ClusterCentroids Undersampling results:
  - Balanced accuracy score is 65.3% overall, the precision avg/total is at 99% and the recall is 40%
   ![image](https://github.com/antxamp/Credit_Risk_Analysis/blob/main/Image_Resources/clustercentroids1.PNG)
   
### SMOTEENN results:    
   - Balanced accuracy score is 54.4% the precision is 99% and the recall is 57% overall   
   ![image](https://github.com/antxamp/Credit_Risk_Analysis/blob/main/Image_Resources/smoteenn2.PNG)
    
### Balanced Random Forest Classifier results:    
   - The accuracy score is 73.6% the precision is 99% and the recall is 86%   
   ![image](https://github.com/antxamp/Credit_Risk_Analysis/blob/main/Image_Resources/balanced_random_forest3.PNG)
   
### Easy Ensemble Classifier results:    
   - The accuracy score is 91.7% the precision is 99% and the recall is 94%  
   ![image](https://github.com/antxamp/Credit_Risk_Analysis/blob/main/Image_Resources/easy_ensemble3.PNG)
 
### Summary:
  - The first four models we undersampled, oversampled and a combination of both to try and determine which model is best at predicting which loans are high risk. I resampled the following data using ensemble classifiers to try and predict which loans are high or low risk. The accuracy score in the first four models are not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores overall. Typically in the models we want a good balance of recall and precision which is why I recommend using the Easy Ensemble classifiers over the first four methods.
