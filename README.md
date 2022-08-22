# Credit_Risk_Analysis

## Project Overview
The purpose of this project was to apply machine learning to credit card risk. Credit risk is inherently unbalanced as good loans outnumber risky loans. Various machine learning models were used to determine which model is best at predicting a customer's credit risk for loan approvals. The six models that were used for this project are RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalanceRandomForestClassifier, and EasyEnsembleClassifier. 

## Resources
Data: LoanStats_2019Q1.csv
Machine Learning Models: RandomOverSampler; SMOTE; ClusterCentroids; SMOTEENN; BalanceRandomForestClassifer; EasyEnsembleClassifier

## Deliverable 1: Use Resampling Models to Predict Credit Risk

### RandomOverSampler

Balanced Accuracy Score
<img width="1119" alt="Screen Shot 2022-08-21 at 6 51 27 PM" src="https://user-images.githubusercontent.com/103774401/185818069-ae9dfe25-a9b6-40b9-be90-b17d385c78b7.png">

RandomOverSampler Imbalanced Classification Report
<img width="1138" alt="Screen Shot 2022-08-21 at 6 51 53 PM" src="https://user-images.githubusercontent.com/103774401/185818077-72005281-a766-4642-a34a-b6fbea392075.png">

- Balanced Accuracy Score: 0.64
- Precision Scores: 
  - Low Risk: 1.00
  - High Risk: 0.01
 - Recall Scores: 
  - Low Risk: 0.62
  - High Risk: 0.66
  
### SMOTE

Balanced Accuracy Score
<img width="1097" alt="Screen Shot 2022-08-21 at 6 56 47 PM" src="https://user-images.githubusercontent.com/103774401/185818096-cf4d27f5-9884-4da7-8699-158930f84364.png">

SMOTE Imbalanced Classification Report
<img width="923" alt="Screen Shot 2022-08-21 at 6 57 03 PM" src="https://user-images.githubusercontent.com/103774401/185818101-fcf675b5-65bc-4fba-bd17-9bb89799b655.png">

- Balanced Accuracy Score: 0.65
- Precision Scores: 
  - Low Risk: 1.00
  - High Risk: 0.01
 - Recall Scores: 
  - Low Risk: 0.69
  - High Risk: 0.61
  
### ClusterCentroids

Balanced Accuracy Score
<img width="1076" alt="Screen Shot 2022-08-21 at 6 59 54 PM" src="https://user-images.githubusercontent.com/103774401/185818490-b28539f9-561d-41c7-a4c2-104bcbba9dbb.png">

ClusterCentroids Imbalanced Classification Report
<img width="907" alt="Screen Shot 2022-08-21 at 7 00 24 PM" src="https://user-images.githubusercontent.com/103774401/185818521-65277f0b-0f32-4877-9dc0-505e09dcf6e7.png">

- Balanced Accuracy Score: 0.65
- Precision Scores: 
  - Low Risk: 1.00
  - High Risk: 0.01
 - Recall Scores: 
  - Low Risk: 0.40
  - High Risk: 0.69
  
## Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk

### SMOTEENN

Balanced Accuracy Score
<img width="1052" alt="Screen Shot 2022-08-21 at 7 01 38 PM" src="https://user-images.githubusercontent.com/103774401/185818636-08600ebb-8b0a-4bf9-b28d-7e37ebfbe4b0.png">

SMOTEENN Imbalanced Classification Report
<img width="1115" alt="Screen Shot 2022-08-21 at 7 01 55 PM" src="https://user-images.githubusercontent.com/103774401/185818670-1a8b7734-b6d4-4db5-b665-a2b38435d57b.png">

- Balanced Accuracy Score: 0.54
- Precision Scores: 
  - Low Risk: 1.00
  - High Risk: 0.01
 - Recall Scores: 
  - Low Risk: 0.56
  - High Risk: 0.75
  
## Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

### BalancedRandomForestClassifier

Balanced Accuracy Score
<img width="1092" alt="Screen Shot 2022-08-21 at 7 04 03 PM" src="https://user-images.githubusercontent.com/103774401/185818710-bfc20030-e547-4bef-b135-f8689c7c8469.png">

BalancedRandomForestClassifier Imbalanced Classification Report
<img width="1037" alt="Screen Shot 2022-08-21 at 7 04 19 PM" src="https://user-images.githubusercontent.com/103774401/185818723-4c9a8d71-41ba-4004-9b7a-c1077e3c5ca6.png">

- Balanced Accuracy Score: 0.79
- Precision Scores: 
  - Low Risk: 1.00
  - High Risk: 0.03
 - Recall Scores: 
  - Low Risk: 0.87
  - High Risk: 0.70
  
### EasyEnsembleClassifier

Balanced Accuracy Score
 <img width="1113" alt="Screen Shot 2022-08-21 at 7 04 55 PM" src="https://user-images.githubusercontent.com/103774401/185818742-7ea184fe-707b-4f0f-89cc-cc809159d638.png">

EasyEnsembleClassifier Imbalanced Classification Report
<img width="1120" alt="Screen Shot 2022-08-21 at 7 05 14 PM" src="https://user-images.githubusercontent.com/103774401/185818761-1621dcb7-e693-48f7-ac8d-815469367c79.png">

- Balanced Accuracy Score: 0.93
- Precision Scores:
  - Low Risk: 1.00
  - High RisK: 0.09
 - Recall Scores: 
  - Low Risk: 0.94
  - High Risk: 0.92
  
## Summary
The four resampling models (RandomOver Sampler, SMOTE, ClusterCentroids, and SMOTEENN) all have fairly similar balance accuracy scores. SMOTEENN has the lowest balanced accuracy score of the resampling techniques with a score of 0.54. Overall, the resampling models are not the greatest models to predict credit risk. 

The two ensemble models predict credit risk far better than the resampling models. The BalancedRandomForestClassifier model has a balance accuracy score of 0.79. The EasyEnsembleClassifier model had a balanced accuracy score of 0.93 which is by far the highest balanced accuracy score. Therefore, ensemble models are much better at predicting a customer's credit risk than resampling models. Further, the EasyEnsembleClassifier model is the highest performing model and should be used to predict a customer's credit risk as it has a 93% accuracy rate. However, it may be risky to solely use the EasyEnsembleClassifier model as it is only 93% accurate and not 100% accurate. Therefore, it may be beneficial to introduce an additional method of assessing credit risk after risk is assessed using the EasyEnsembleClassifier model.
