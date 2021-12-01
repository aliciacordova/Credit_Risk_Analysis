# Credit_Risk_Analysis

## Overview

We have been asked to help Jill with an analysys to evaluate the performance of differents models and make a recommendation on whether they should be used to predict credit risk. Some of them are: 
- Oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

And finally we will recommend what should be used to predict credit risk.

## Results

## DELIVERABLE #1:

### RandomOverSampler model

![M17 RamdomOverSample1](https://user-images.githubusercontent.com/87447639/143935076-5840cff5-5d5b-4ac6-9254-c515fce7e5e0.PNG)


![M17 RamdomOverSample2](https://user-images.githubusercontent.com/87447639/143935074-8c0b8c4e-0479-48c1-b16e-231d92df37e3.PNG)


- The balanced accuracy score is 64%.
- The high_risk precision is about 1% only with 60% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### SMOTE model

![M17 Smotemodel1](https://user-images.githubusercontent.com/87447639/143935073-dd0f7275-9c4c-4d35-91b6-2d1232f917e4.PNG)


![M17 Smotemodel2](https://user-images.githubusercontent.com/87447639/143935072-d0001a6f-fad2-41a7-afb1-3bba7f6dc18a.PNG)

- The balanced accuracy score is 64%.
- The high_risk precision is about 1% only with 60% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### ClusterCentroids model

![M17 ClusterCentroids1](https://user-images.githubusercontent.com/87447639/143935071-e2aa7557-2466-479f-a38a-c9a864c0d942.PNG)

![M17 ClusterCentroids2](https://user-images.githubusercontent.com/87447639/143935067-d4452feb-4ccb-431a-8ebd-9a1321e09d89.PNG)


- The balanced accuracy score is 52%.
- The high_risk precision is about 1% only with 60% sensitivity which makes a F1 of 1% only.
- Due to the high number of false positives, the low_risk sensitivity is only 43%.

## DELIVERABLE #2:

### SMOTEENN model

![m17 Smoteenn1](https://user-images.githubusercontent.com/87447639/143935079-df1966c1-b205-4c9a-aeba-5cd091eb685e.PNG)


![m17 Smoteenn2](https://user-images.githubusercontent.com/87447639/143935077-316ba63e-5742-4eb1-9763-45f6a21da5b0.PNG)


- The balanced accuracy score is 62%.
- The high_risk precision is about 1% only with 70% sensitivity which makes a F1 of 2% only.
- Due to the high number of false positives, the low_risk sensitivity is 55%.


## DELIVERABLE #3:

### BalancedRandomForestClassifier model

![M17 BalanceRForest1](https://user-images.githubusercontent.com/87447639/144230396-c9770e34-0711-4b6d-b490-aee8373f5f18.PNG)

![M17 BalanceRForest2](https://user-images.githubusercontent.com/87447639/144230416-a2aaf1b1-bcc1-48eb-aae6-9b9065d543fd.PNG)

- The balanced accuracy score is 79%.
- The high_risk precision is about 4% only with 67% sensitivity which makes a F1 of 7% only.
- Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier model

![M17 EasyEnsembleClass1](https://user-images.githubusercontent.com/87447639/144233420-cbffbe16-a9a9-4f11-b967-57c89ee8e7e4.PNG)

![M17 EasyEnsembleClass2](https://user-images.githubusercontent.com/87447639/144233429-1acaf960-6552-470b-9d09-f00d27284ef1.PNG)

- The balanced accuracy score is 93%.
- The high_risk precision is about 7% only with 91% sensitivity which makes a F1 of 14% only.
- Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

## Summary

In this analysis, we help Jill determine which of the models should be used to predict credit risk.
Based on the results, the RamdomOver Sampler, Smote, ClusterCentroids, and Smoteen model show weak accuracy in determining whether a credit risk is high because its accuracy is below 70%.
However, the last two models BalancedRamdomForest and EasyEnsembleClassifier show improvements in precision score above 78%, sensitive score with 67% and 91% respectively, and high precision score with 4% and 7% compared to previous models.
We know that none of the models is perfect, but if we have to recommend the bank to use any of these models to predict credit risk, we recommend the EasyEnsembleClassifier because it shows a recall of 92% so it detects almost all high risk credit, with low precision, but we have to keep in mind that many low risk credits are still falsely detected as high risk and we could get false positives.

