# Credit_Risk_Analysis

Module 17: Credit Risk Analysis


# Credit Risk Analysis

## Overview

*Background* 

In 2019, more than 19 million Americans had at least one unsecured personal loan. That's a record-breaking number! Personal lending is growing faster than credit card, auto, mortgage, and even student debt. With such incredible growth, FinTech firms are storming ahead of traditional loan processes. By using the latest machine learning techniques, these FinTech firms can continuously analyze large amounts of data and predict trends to optimize lending.

A peer-to-peer lending services company, Fast Lending, is looking to use machine learning to assess credit risk. By using machine learning (ML), they hope to create a quicker and more reliable loan experience. ML will have a high accuracy identification rate for good candidates for loans, which in turn could allow for lower default rates and other positive results. The lead scientist, Jill will need help to implent this plan by building and evaluating many ML models to see which works best for the data. It's important to evaluate the model's performance to see how well it could predict data. 

*Purpose*

Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

-----------------------------------

## Results

Below are descriptions of the balanced accurary scores and the precision and recall scores of all six machine learning models. 

*1. Random Over Sampler*

#### Balanced Accuracy Score

- Balanced Accuracy Score: 66.1%
- Precision of High-Risk Classification was 0.01, while the precision of the Low-Risk Classification was 1.00. These values help to explain that the Low-Risk Classifications are very reliable, but the High-Risk classications are not reliable at all. 
- Recall of High-Risk Classification was 0.72 and the recall of the low-risk classification was 0.60. These values demonstrate that High-Risk classification has a higher sensitivity than the Low-Risk Classication, which means that the model was able to correctly identify 72% of the High-Risk classified loans. 

![Balanced Accuracy Score](https://user-images.githubusercontent.com/102566199/183555422-e2b1fba6-0cd7-4e40-84ef-81a65b2dfb10.png)


#### Confusion Matrix

![Confusion Matrix](https://user-images.githubusercontent.com/102566199/183555548-992c7ef8-d2ca-417b-8041-4c8de2b4ea88.png)

#### Imbalanced Classification Report

![Imbalanced Classification Report](https://user-images.githubusercontent.com/102566199/183555649-3dd658b5-c485-4939-9c06-8a6366367c76.png)



*2. SMOTE*

- Balanced Accuracy Score: 65.8%
- Precision of High-Risk Classification was 0.01, while the precision of the Low-Risk Classification was 1.00. These values help to explain that the Low-Risk Classifications are very reliable, but the High-Risk classications are not reliable at all. 
- Recall of High-Risk Classification was 0.63 and the recall of the low-risk classification was 0.68. These numbers are fairly similar and both sit lower than the previous model with only 63% of the High-Risk loans being identified. 

#### Balanced Accuracy Score
![BAS_Smote](https://user-images.githubusercontent.com/102566199/183555794-97243d33-5a1d-47b7-b6af-9ba0c8975c2f.png)

#### Confusion Matrix

![CM_Smote](https://user-images.githubusercontent.com/102566199/183555901-606e7961-bd1a-4e50-ae71-d40edb8e8012.png)

#### Imbalanced Classification Report

![ICR_smote](https://user-images.githubusercontent.com/102566199/183555978-997e921d-374f-4700-9ed9-8d36e603336b.png)


 *3. Cluster Centroids*

- Balanced Accuracy Score: 54.4% (Lowest value of all models)
- Precision of High-Risk Classification was 0.01, while the precision of the Low-Risk Classification was 1.00. These values help to explain that the Low-Risk Classifications are very reliable, but the High-Risk classications are not reliable at all. 
- Recall of High-Risk Classification was 0.69 and the recall of the low-risk classification was 0.40. These values demonstrate that High-Risk classification has a higher sensitivity than the Low-Risk Classication, which means that the model was able to correctly identify 69% of the High-Risk classified loans. 


#### Balanced Accuracy Score

![BAS_CC](https://user-images.githubusercontent.com/102566199/183556212-af20c030-8aef-4bc4-a139-6a88c82e7a7f.png)


#### Confusion Matrix

![CM_CC](https://user-images.githubusercontent.com/102566199/183556241-991221bc-1b9c-43df-8b3a-275e96e6827d.png)


#### Imbalanced Classification Report

![ICR_CC](https://user-images.githubusercontent.com/102566199/183556281-45d48d9d-220c-4891-b875-c285e792acfe.png)


 *4. SMOTEENN*
 
- Balanced Accuracy Score: 64.8%
- Precision of High-Risk Classification was 0.01, while the precision of the Low-Risk Classification was 1.00. These values help to explain that the Low-Risk Classifications are very reliable, but the High-Risk classications are not reliable at all. 
- Recall of High-Risk Classification was 0.72 and the recall of the low-risk classification was 0.57. These values demonstrate that High-Risk classification has a higher sensitivity than the Low-Risk Classication, which means that the model was able to correctly identify 72% of the High-Risk classified loans. 
 
#### Balanced Accuracy Score

![BAS_S](https://user-images.githubusercontent.com/102566199/183556340-02ca32ff-8f72-4342-a5dd-e2ff30d48e94.png)


#### Confusion Matrix

![CM_S](https://user-images.githubusercontent.com/102566199/183556359-0b889fc1-9d7f-4f44-91a0-5514db14a96c.png)


#### Imbalanced Classification Report

![ICR_S](https://user-images.githubusercontent.com/102566199/183556392-612ed405-0431-4695-9d7e-fcd66d17da9e.png)

 *5. Balanced Random Forest Classifier*
 
- Balanced Accuracy Score: 78.8%
- Precision of High-Risk Classification was 0.03, while the precision of the Low-Risk Classification was 1.00. These values help to explain that the Low-Risk Classifications are very reliable, but the High-Risk classications are not reliable at all. 
- Recall of High-Risk Classification was 0.70 and the recall of the low-risk classification was 0.87. These values demonstrate that High-Risk classification has a lower sensitivity than the Low-Risk Classication, which means that the model was able to correctly identify 70% of the High-Risk classified loans.  
 
#### Balanced Accuracy Score

![BAS_RF](https://user-images.githubusercontent.com/102566199/183558179-a3d4a6e6-ca89-48bc-817b-1c12bbe87eab.png)


#### Confusion Matrix

![CM_RF](https://user-images.githubusercontent.com/102566199/183558224-9eb79a9a-365f-4146-af94-23cc9326ed5d.png)


#### Imbalanced Classification Report

![ICR_RF](https://user-images.githubusercontent.com/102566199/183558251-b85bb131-8b44-4c1f-9fa3-2ed1ae37d264.png)


 *6. Easy Ensemble Classifier*
 
- Balanced Accuracy Score: 93.2% (Highest value of all models)
- Precision of High-Risk Classification was 0.09, while the precision of the Low-Risk Classification was 1.00. These values help to explain that the Low-Risk Classifications are very reliable, but the High-Risk classications are not reliable at all. 
- Recall of High-Risk Classification was 0.92 and the recall of the low-risk classification was 0.94. Both have extremely values, which is impressive because the model was able to correctly identify 92% of the High-Risk classified loans. 
 
 #### Balanced Accuracy Score

![BAS_EE](https://user-images.githubusercontent.com/102566199/183558313-712c7f7e-04c1-47f2-976d-5aa138d23320.png)


#### Confusion Matrix

![CM_EE](https://user-images.githubusercontent.com/102566199/183558337-7738f09b-f9a2-4bdc-b19c-5fdfc605d930.png)


#### Imbalanced Classification Report

![ICR_EE](https://user-images.githubusercontent.com/102566199/183558377-919f4174-e467-4d6c-94c0-cf0d16b467cf.png)


-------------------

## Summary

*Summary of results*

Results of the machine learning models summarized

*Recommendations*

Recommendation on the model to use, if any: if no recommendation is possible explain why and give a justification 
