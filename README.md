# Credit Risk Analysis

## Purpose

The task was to use imbalanced-learn and scikit-learn to evaluate the use of machine learning models to resample data and provide feedback.
A credit card dataset from the LendingClub organization, a peer-to-peer lending services company, will be processed through these 6 different models. The results and accuracy scores will be compared along with pictures.

## Results
Here will be a list of different models and their scores:

  *Accuracy = Acc*

  *Precision = Pre*

  *Recall = Rec*



### Random Oversampler
![Random_Oversampler](https://github.com/Cyber-Wolfe/Credit_Risk_Analysis/blob/main/Captures/Random_Oversampler.PNG)

**Accuracy: % 62.99**

**Precision:**

0 = 0.01

1 = 1.00

**Recall:**

0 = 0.66
        
1 = 0.60


### SMOTE Oversampling
![SMOTE_Oversampling](https://github.com/Cyber-Wolfe/Credit_Risk_Analysis/blob/main/Captures/SMOTE_Oversampling.PNG)

**Accuracy: % 63.40**

**Precision:**

0 = 0.01

1 = 1.00

**Recall:**

0 = 0.63
        
1 = 0.64

### Under Sampling

![Under_Sampling](https://github.com/Cyber-Wolfe/Credit_Risk_Analysis/blob/main/Captures/Under_Sampling.PNG)

**Accuracy: % 63.40**

**Precision:**

0 = 0.01

1 = 1.00

**Recall:**

0 = 0.71
        
1 = 0.55

### Over/Under Sampling

![Over_Under_Sampling](https://github.com/Cyber-Wolfe/Credit_Risk_Analysis/blob/main/Captures/Over_Under_Sampling.PNG)

**Accuracy: % 63.27**

**Precision:**

0 = 0.01

1 = 1.00

**Recall:**

0 = 0.71
        
1 = 0.55

### Balance Random Forest Classifier

![Balance_Random_Forest_Classifier](https://github.com/Cyber-Wolfe/Credit_Risk_Analysis/blob/main/Captures/Balance_Random_Forest_Classifier.PNG)

**Accuracy: % 86.60**

**Precision:**

0 = 0.03

1 = 1.00

**Recall:**

0 = 0.63
        
1 = 0.87

### Easy Ensemble Classifier

![Easy_Ensemble_Classifier](https://github.com/Cyber-Wolfe/Credit_Risk_Analysis/blob/main/Captures/Easy_Ensemble_Classifier.PNG)

**Accuracy: % 94.60**

**Precision:**

0 = 0.01

1 = 1.00

**Recall:**

0 = 0.56
        
1 = 0.47

## Summary
The sampling models that had been used gave low accuracy, wildly different precision and decent recall, hovering in the low to mid 60s and the classifier models have the same kind of precision as the sampling models. The classifier model's recall though is in the mid 60s for the forest and mid 50s for the ensemble. Their precision seems to still be low, with 0.01 but the accuracy is incredibly high, being 87% for the forest and 94% for the ensemble.

So what does this mean, it means that the Easy Ensemble Classifier has the highest accuracy but their precision is very low on one side which isn't too promising. The recall is also way too low on both sides to be considered worthwhile to use.

I wouldn't recommend to use these models because they are reporthing out a min value of about 63% for accuracy and their precision scores are too drastically one sided to be considered precies although accurate. Maybe with the data being much more pruned the values could change and the models could prove to be more reliable but in their current state I couldn't advise to use them.
