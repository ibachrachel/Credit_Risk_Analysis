# Credit_Risk_Analysis

Module 17: Credit Risk Analysis


# Credit Risk Analysis

## Overview

*Background* 

In 2019, more than 19 million Americans had at least one unsecured personal loan. That's a record-breaking number! Personal lending is growing faster than credit card, auto, mortgage, and even student debt. With such incredible growth, FinTech firms are storming ahead of traditional loan processes. By using the latest machine learning techniques, these FinTech firms can continuously analyze large amounts of data and predict trends to optimize lending.

Fast lending, a peer-to-peer lending services company
ML is being used to assess credit risk
Quick and reliable loan experience
ML will be more accurate identification for good candidates for loans: lower default rates
Assist lead data scientist is implementing this plan:
Build and evaluate many ML models to see which works best for the data
→ evaluate their performance and see how well the model predicts data
 
The lead data scientist, Jill, has asked you to create the same development environment that she is using. This step will help you run the code smoothly without conflicts.


*Purpose*

Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.



-----------------------------------
## Results

Below are descriptions of the balanced accurary scores and the precision and recall scores of all six machine learning models. 


*1. Random Over Sampler*

#### Balanced Accuracy Score

![Balanced Accuracy Score](https://user-images.githubusercontent.com/102566199/183555422-e2b1fba6-0cd7-4e40-84ef-81a65b2dfb10.png)


#### Confusion Matrix

![Confusion Matrix](https://user-images.githubusercontent.com/102566199/183555548-992c7ef8-d2ca-417b-8041-4c8de2b4ea88.png)

#### Imbalanced Classification Report

![Imbalanced Classification Report](https://user-images.githubusercontent.com/102566199/183555649-3dd658b5-c485-4939-9c06-8a6366367c76.png)



*2. SMOTE*


#### Balanced Accuracy Score
![BAS_Smote](https://user-images.githubusercontent.com/102566199/183555794-97243d33-5a1d-47b7-b6af-9ba0c8975c2f.png)

#### Confusion Matrix

![CM_Smote](https://user-images.githubusercontent.com/102566199/183555901-606e7961-bd1a-4e50-ae71-d40edb8e8012.png)

#### Imbalanced Classification Report

![ICR_smote](https://user-images.githubusercontent.com/102566199/183555978-997e921d-374f-4700-9ed9-8d36e603336b.png)


 *3. Cluster Centroids*

#### Balanced Accuracy Score

![BAS_CC](https://user-images.githubusercontent.com/102566199/183556212-af20c030-8aef-4bc4-a139-6a88c82e7a7f.png)


#### Confusion Matrix

![CM_CC](https://user-images.githubusercontent.com/102566199/183556241-991221bc-1b9c-43df-8b3a-275e96e6827d.png)


#### Imbalanced Classification Report

![ICR_CC](https://user-images.githubusercontent.com/102566199/183556281-45d48d9d-220c-4891-b875-c285e792acfe.png)


 *4. SMOTEENN*
 
#### Balanced Accuracy Score

![BAS_S](https://user-images.githubusercontent.com/102566199/183556340-02ca32ff-8f72-4342-a5dd-e2ff30d48e94.png)


#### Confusion Matrix

![CM_S](https://user-images.githubusercontent.com/102566199/183556359-0b889fc1-9d7f-4f44-91a0-5514db14a96c.png)


#### Imbalanced Classification Report

![ICR_S](https://user-images.githubusercontent.com/102566199/183556392-612ed405-0431-4695-9d7e-fcd66d17da9e.png)

 *5. Balanced Random Forest Classifier*
 
#### Balanced Accuracy Score


#### Confusion Matrix



#### Imbalanced Classification Report

 *6. Easy Ensemble Classifier*
 
 #### Balanced Accuracy Score


#### Confusion Matrix



#### Imbalanced Classification Report

-------------------

## Summary

*Summary of results*

Results of the machine learning models summarized

*Recommendations*

Recommendation on the model to use, if any: if no recommendation is possible explain why and give a justification 
