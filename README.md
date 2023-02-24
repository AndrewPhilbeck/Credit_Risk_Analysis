# Credit_Risk_Analysis

Analyzing the abilities of six different styles of machine learning to predict credit card fraud.

## Overview

I used a variety of different machine learning algorithms to see which was most successful at predicting credit card fraud. I employed the RandomOverSampler method and SMOTE Oversampling. Once those were complete I used undersampling algorithms: ClusterCentroids and SMOTEENN. Once these methods were done I used two ensemble methods: BalancedRandomClassifier and EasyEnsembleClassifier.

### RandomOverSampler:

Balanced Accuracy: 

![Random Balanced](https://user-images.githubusercontent.com/115502048/221288536-f54ee9f1-e74d-4b84-8fe0-f5bbc3548556.png)

Confusion Matrix: 

![Random Over Matrix](https://user-images.githubusercontent.com/115502048/221288576-248fd8c5-e145-4fe3-8739-4597907ca932.png)

Classification report imbalanced:

![Random Over Imbalanced](https://user-images.githubusercontent.com/115502048/221288618-01f29dc7-911c-4dfa-9b26-9bd9a92c0865.png)

### SMOTE

Balanced Accuracy: 

![SMOTE Balanced](https://user-images.githubusercontent.com/115502048/221288691-2811f932-d6fa-445a-830b-586fdffd1c03.png)

Confusion Matrix: 

![SMOTE Matrix](https://user-images.githubusercontent.com/115502048/221288740-dc2e218b-d864-42e5-ad94-4c4b0a125172.png)

Classification report imbalanced:

![SMOTE imbalanced](https://user-images.githubusercontent.com/115502048/221288775-961b54a5-81fd-44ad-bf67-fef56ce5b2b6.png)

### ClusterCentroids

Balanced Accuracy: 

![Cluster Balanced](https://user-images.githubusercontent.com/115502048/221288969-c55f963f-2988-42f1-96d4-2021a78ef1c6.png)

Confusion Matrix: 

![Cluster Matrix](https://user-images.githubusercontent.com/115502048/221289046-a98d9e4b-4514-4f7a-a579-42e124bb88f1.png)

Classification report imbalanced:

![Cluster Imbalanced](https://user-images.githubusercontent.com/115502048/221289139-f7a0c35c-d9f1-4c82-8ad5-e611ad4d49fd.png)

### SMOTEENN

Balanced Accuracy: 

![SMOTEENN balanced](https://user-images.githubusercontent.com/115502048/221289231-cd5cd8ae-5bf5-4982-9e3d-28d3e8d355d7.png)

Confusion Matrix: 

![smoteenn matrix](https://user-images.githubusercontent.com/115502048/221289306-05bddf0a-082c-4661-9762-e2411556d368.png)

Classification report imbalanced:

![smoteenn imbalanced](https://user-images.githubusercontent.com/115502048/221289369-b1af6a28-1723-41ef-bc92-6da347a0b8d8.png)

### BalancedRandomForest

Balanced Accuracy: 

![forest balanced](https://user-images.githubusercontent.com/115502048/221289432-e8eb7f47-d99e-413b-8fdd-f1e9bba88083.png)

Confusion Matrix: 

![forest matrix](https://user-images.githubusercontent.com/115502048/221289485-334c04fd-307d-4dc3-af60-9e5838c58e64.png)

Classification report imbalanced:

![forest imbalanced](https://user-images.githubusercontent.com/115502048/221289535-b67a9c5a-6059-4b5e-97ee-8699bb9823e2.png)

### EasyEnsembleClassifier

Balanced Accuracy: 

![Easy balanced](https://user-images.githubusercontent.com/115502048/221289634-0952bb95-d60b-4ed8-8419-180ca88fcb9f.png)

Confusion Matrix: 

![Easy Matrix](https://user-images.githubusercontent.com/115502048/221289702-a3fd7511-42dc-44bd-9995-2a6af87e7eed.png)

Classification report imbalanced:

![easy imbalanced](https://user-images.githubusercontent.com/115502048/221289827-4c33e421-e2fa-4c48-bf3e-c4aec7680fe1.png)

## Results of Analysis

### Scores

RandomOverSampler:
* Balanced: 65%
* Precision: .99
* Sensitivity: .59
* F1: .73

SMOTE:
* Balanced: 66%
* Precision: .99
* Sensitivity: .69
* F1: .81

ClusterCentroids:
* Balanced: 66%
* Precision: .99
* Sensitivity: .40
* F1: .56

SMOTEENN:
* Balanced: 65%
* Precision: .99
* Sensitivity: .57
* F1: .72

BalancedRandomForest:
* Balanced: 79%
* Precision: .99
* Sensitivity: .87
* F1: .93

EasyEnsembleClassifier:
* Balanced: 93%
* Precision: .99
* Sensitivity: .94
* F1: .97


## Summary

Studying the different outcomes of each algorithm there is a clear winner when it comes to detecting credit card fraud. While all the models had high precision scores only one combined that with a high sensitivity (recall) score as well. So despite the high level of precision most of the models had a low or lower than desired F1 score, which reveals the overall strength of the algorithm (a combination of both precision and sensitivity). With that in mind the EasyEnsembleClassifier is the clear favorite to help prevent credit card fraud.


