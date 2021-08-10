# Credit_Risk_Analysis

### Overview and Purpose
In order to create a model to accurately predict credit risk machine learning models will be applied to solve the data set from LendingClub, a peer-to-peer lending services company.In the analysis imbalanced-learn and scikit-learn libraries will be used to build and evaluate models using resampling.
The following model will be used and related objectives:
1. RandomOverSampler 
2. SMOTE algorithms to oversample 
3. ClusterCentroids algorithm (CC) to undersample 
4. SMOTEENN algorithm, a combinatorial approach of over- and undersampling;
5. BalancedRandomForestClassifier 
 6. EasyEnsembleClassifier
The balance accuracy score improved to 93%, which is the highest thus far. According to the confusion matrix the false negative increased even more to 16160. There is a slight increase in terms of classification outcomes. The CC model perfectly predicted all true negatives (low risk) with a 99% precision rate. Low risk credit cards were identified retrieved, with a score of 1, all relevant low risk credit card and high risk were below 0.09. However, the CC model has the highest recall score percentage with 92% and 94% for high risk and low risk respectively compared to the other models. 

### Resutls

##### 1. RandomOverSampler 
The Random over sampler balance accuracy is 66% in accuratly predicting positive low risk credit card.  According to the confusion matrix there were 70 true positives and 31 false pasitives, and 7561 false negatives and 9543 true negatives. The Random Oversampling model perfectly predicted all true negatives (low risk) with a 99% precision rate. Low risk credit cards were identified retrieved, with a score of 1, all relevant low risk credit card and high risk were below 0.01. The model predicted risk from the data with a recall score of 69% & 56% for both high risk and low risk credit card respectively.

##### 2. SMOTE algorithms to oversample 
The Random over sampler balance accuracy is higher in accuratly predicting positive low risk credit card, but not as accurate in predeicting high risk credit card (66%). According to the confusion matrix the combined classes avarage values show slight improvement. The model failed to accurately predict 5291 wich is an imporovemnt over RO. The RO and SMOTE model perfectly predicted all true negatives (low risk) with a 99% precision rate. Low risk credit cards were identified retrieved, with a score of 1, all relevant low risk credit card and high risk were below 0.01. The predicted riskfrom the data with a recall score of 59% & 72% for both high risk and low risk credit card respectively, a slight increase in low risk prediction.

##### 3. ClusterCentroids algorithm (CC) to undersample 
The balance accuracy is the same for the Cluster Centroid algorithm as it is for the SMOTE model at 66%.The confusion matrix for the CC model showed that this model has increased false negatives(10324) compared to the NRO and SMOTE models. There is no real difference with the RO model in terms of classification outcomes. The CC model perfectly predicted all true negatives (low risk) with a 99% precision rate. Low risk credit cards were identified retrieved, with a score of 1, all relevant low risk credit card and high risk were below 0.01. However, the CC model has the highest recall score percentage with 68% of total data retrieved compared to three models above.

##### 4. SMOTEENN algorithm, a combinatorial approach of over- and undersampling;
The balance accuracy decreased to 54%,which is lower than the RO and the SMOTE models.Accoridng to the confusion matrix,there are no real difference between the three models.The major difference is on the retrieval of classes with a recal score of 69% for high risk, which is the highest of the three models. Predicting the high risk credit card is better with the SMOTEEN model. However, the low risk recall dropped to the lowest at 40%. 

##### 5. BalancedRandomForestClassifier 
The balance accuracy score improved to 80%, which is the highest thus far. According to the confusion matrix the false negative increased even more to 15018. There is no real difference in terms of classification outcomes. The CC model perfectly predicted all true negatives (low risk) with a 99% precision rate. Low risk credit cards were identified retrieved, with a score of 1, all relevant low risk credit card and high risk were below 0.03.However, the CC model has the highest recall score percentage with 71% and 88% for high risk and low risk respectively compared to the other models.The low risk percentage more than doubled from the SMOTEEN model. None of the features are partucularly usefl in this model. 

##### 6. EasyEnsembleClassifier
The balance accuracy score improved to 93%, which is the highest thus far. According to the confusion matrix the false negative increased even more to 16160. There is a slight increase in terms of classification outcomes. The CC model perfectly predicted all true negatives (low risk) with a 99% precision rate. Low risk credit cards were identified retrieved, with a score of 1, all relevant low risk credit card and high risk were below 0.09. However, the CC model has the highest recall score percentage with 92% and 94% for high risk and low risk respectively compared to the other models. 

### Summary
In an intial evaluation of the variables there is a weak correltation anomg the independent variaables and the dependent variable. IT is not suprising that all the models used in the credit risk analysis show weak precision in determining if a credit risk is high. The Ensemble models seemed to perform better than the other models specially for sensitivity of high risk credits. The Easy Ensemble Classifier model had a recall of 92% so it detects the majority of high risk credit. However, the low precision and the increas in false negative low risk credits there is still a high rate of false detection of high risk, thus decrease loan opportunities and revenue. A review of the features ranked by importance also showed that the foundtation of these models are flawed and would not recommend the bank to use any of these models to predict credit risk.

### Resources
https://python.hotexamples.com/examples/imblearn.combine/SMOTEENN/-/python-smoteenn-class-examples.html
https://github.com/Ekanpat/Credit_Risk_Analysis
https://www.geeksforgeeks.org/ensemble-methods-in-python/
https://github.com/cedoula/Credit_Risk_Analysis

https://stackoverflow.com/questions/40565444/balanced-random-forest-in-scikit-learn-python
