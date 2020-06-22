# Credit_Risk

Credit risk is an unbalanced classification problem, as the number of good loans easily outnumber the number of risky loans.  Use imbalanced-learn and scikit-learn libraries to build and evaluate machine learning models using resampling.  

## Objective 1
- Compare two oversampling algorithms (Naïve Random Oversampling and SMOTE) to determine which algorithm results in the best performance.
- Compare undersampling algorithms (Cluster Centroids algorithm) to determine how they compare to the oversampling methods.
- Test a combination of over- and under-sampling algorithm to compare the algorithm results to the previous sampling algorithms.

### Naïve Random Oversampling

With the “Random Oversampling” method, the accuracy score is 0.65.  For high risk applications, precision is 0.01, recall is 0.69, and  f1 score is 0.02.  For low risks, precision is 1.00, recall is 0.61, and f1 score is 0.76.

### SMOTE

With the “SMOTE” method, the accuracy score is 0.66.  For high risk applications, precision is 0.01, recall is 0.66, and f1 score is 0.02.  For low risks, precision is 1.00, recall is 0.69, and f1 score is 0.82.


### Cluster Centroid 
With the “Cluster Centroid” method, the accuracy is 0.55.  For high risk applications, precision is 0.01, recall is 0.68, and f1 score is 0.01.  For low risks, precision is 1.00, recall is 0.41, and f1 score is 0.58.

### Combination (Over and Under) 
With the “Combination (Over and Under)” method, specifically the SMOTEENN, the accuracy is 0.55.  For high risk applications, precision is 0.01, recall is 0.71, and f1 score is 0.02.  For low risks, precision is 1.00, recall is 0.58, and f1 score is 0.73.

### Summary and Analysis
The accuracy score for models used were all in the 55-66%.  The precision for high risk from all models were very low (1%) whereas the precision for low risk from all model were 100%.  I do not recommend any models to predict high risks as accuracy and precisions are very low.


## Objective 2
Train and compare two different ensemble classifiers to predict loan risk and evaluate each model.

### Balanced Random Forest
With the “Balanced Random Forest” method, the accuracy is 0.79.  For high risk applications, precision is 0.04, recall is 0.67, and f1 score is 0.07.  For low risks, precision is 1.00, recall is 0.90, and f1 score is 0.95.

### Easy Ensemble Classifier
With the “Easy Ensemble Classifier” method, the accuracy is 0.93.  For high risk applications, precision is 0.09, recall is 0.92, and f1 score is 0.16.  For low risks, precision is 1.00, recall is 0.94, and f1 score is 0.97.

### Summary and Analysis
The Easy Ensemble Classifier has highest accuracy from all models, with 0.93.  The precision for this model is low with 0.09 vs 0.04 for “Balanced Random Forest.”  With that said, I would recommend to use the Easy Ensemble Classifier model.






