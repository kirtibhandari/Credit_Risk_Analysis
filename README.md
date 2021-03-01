# **Credit-Risk Analysis**

## **Overview:**

The project at hand requires the application of machine learning to provide solution to a real-world challenge, credit card risk.

A credit card risk, as a real-life instance, involves a situation where most of the customers are eligible for the issuance of the loans than those who do not qualify and come under the risky and non risky loans, respectively. In machine learning, this kind of situation is an unbalanced classification problem where members in one class, outnumbers the members in other class. Hence, we are required to test the given data set by employing various methodologies or techniques. Here, for the current analysis, we have used different techniques to train and evaluate the models using unbalanced classes.

In machine learning, there is a family of re sampling techniques which are particularly designed to tackle with situations like this, which is a situation of class imbalance. Class imbalance is a common problem when we want to classify the data i.e., when one class is much larger than the other class as explained above the current real-life situation of credit card risk prediction. to address this situation three techniques namely oversampling, under sampling and a combination approach of oversampling and under sampling are being used in the current analysis.

The requirements of the project involve using imbalanced learn and ski-kit learn libraries to build and evaluate models using resampling. In this analysis we have been provided a credit card data set from a peer-to-peer lending services company. we have used algorithms namely **RandomOverSampler**, and **SMOTE** to oversample the data, the **ClusterCentroids** algorithm two under sample the data. Then, in one of the techniques we have used combinatorial approach that involves over and under sampling, named **SMOTEENN** algorithm. Further, do machine learning models that reduce bias, have been compared, to predict credit risk, namely **RandomForestClassifier** and **EasyEnsembleClassifier**.

After using all the advised six algorithms, we have evaluated the performance of these models and presented recommendation on the usage of any of these to predict credit risk, depending upon their balanced accuracy scores, the obtained precision and recall scores. 

Precision here means positive predictive value which is a measure of how reliable a positive classification is. Here, recall, or say sensitivity, implies how many people who are under credit risk, were correctly predicted.

## **Results:**

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

### **1. Naive Random Oversampling:** ###
![](https://github.com/kirtibhandari/Credit_Risk_Analysis/blob/main/Resources/oversampling.png)

**Balanced accuracy Score:** The above results show the balanced accuracy score of 66%, meaning thereby that this model predicts the high risk and low risk applications accurately, 66% of the times.

**Precision:** The results of this algorithm has precision value of 0.01 i.e., 1%. This means it is only 1% likely that the applications predicted to be of high risk;and 1.00, for low risk; are actually high risk or low risk applications in the original data set as well.

**Recall:** The above algorithm shows recall value of 74 % for high risk applications and 58 % for low risk applications. This implies that there is a 74% chance that the actual high risk applications will also be predicted to be high risk and there is a 58% chance that the actual low risk applications will also be predicted to be low risk.

### **2. SMOTE Oversampling:**

![](https://github.com/kirtibhandari/Credit_Risk_Analysis/blob/main/Resources/smote.png)

**Balanced accuracy Score:** The above results show the balanced accuracy score of 65%, meaning thereby that this model predicts the high risk and low risk applications accurately, 65% of the times.

**Precision:** The results of this algorithm has precision value of 0.01 i.e., 1%. This means it is only 1% likely that the applications predicted to be of high risk;and 1.00, for low risk; are actually high risk or low risk applications in the original data set as well.

**Recall:** The above algorithm shows recall value of 62 % for high risk applications and 68 % for low risk applications. This implies that there is a 62% chance that the actual high risk applications will also be predicted to be high risk and there is a 68% chance that the actual low risk applications will also be predicted to be low risk.
### **3. ClusterCentroids Under-sampling:**

![](https://github.com/kirtibhandari/Credit_Risk_Analysis/blob/main/Resources/under-sampling.png)

**Balanced accuracy Score:** The above results show the balanced accuracy score of 54%, meaning thereby that this model predicts the high risk and low risk applications accurately, 54% of the times.

**Precision:** The results of this algorithm has precision value of 0.01 i.e., 1%. This means it is only 1% likely that the applications predicted to be of high risk;and 1.00, for low risk; are actually high risk or low risk applications in the original data set as well.

**Recall:** The above algorithm shows recall value of 69 % for high risk applications and 40 % for low risk applications. This implies that there is a 69% chance that the actual high risk applications will also be predicted to be high risk and there is a 40% chance that the actual low risk applications will also be predicted to be low risk.
### **4. SMOTEENN (Over & Under sampling):**

![](https://github.com/kirtibhandari/Credit_Risk_Analysis/blob/main/Resources/smoteenn.png)

**Balanced accuracy Score:** The above results show the balanced accuracy score of 68%, meaning thereby that this model predicts the high risk and low risk applications accurately, 68% of the times.

**Precision:** The results of this algorithm has precision value of 0.01 i.e., 1%. This means it is only 1% likely that the applications predicted to be of high risk;and 1.00, for low risk; are actually high risk or low risk applications in the original data set as well.

**Recall:** The above algorithm shows recall value of 77 % for high risk applications and 59 % for low risk applications. This implies that there is a 77% chance that the actual high risk applications will also be predicted to be high risk and there is a 59% chance that the actual low risk applications will also be predicted to be low risk.
### **5. BalancedRandomClassifier:**

![](https://github.com/kirtibhandari/Credit_Risk_Analysis/blob/main/Resources/balanced.png)

**Balanced accuracy Score:** The above results show the balanced accuracy score of 78%, meaning thereby that this model predicts the high risk and low risk applications accurately, 78% of the times.

**Precision:** The results of this algorithm has precision value of 0.03 i.e., 3%. This means it is only 3% likely that the applications predicted to be of high risk;and 1.00, for low risk; are actually high risk or low risk applications in the original data set as well.

**Recall:** The above algorithm shows recall value of 70% for high risk applications and 87% for low risk applications. This implies that there is a 70% chance that the actual high risk applications will also be predicted to be high risk and there is a 87% chance that the actual low risk applications will also be predicted to be low risk.

### **6. EasyEnsembleClassifier:**

![](https://github.com/kirtibhandari/Credit_Risk_Analysis/blob/main/Resources/easyensemble.png)

**Balanced accuracy Score:** The above results show the balanced accuracy score of 93%, meaning thereby that this model predicts the high risk and low risk applications accurately, 93% of the times.

**Precision:** The results of this algorithm has precision value of 0.09 i.e., 9%. This means it is only 9% likely that the applications predicted to be of high risk;and 1.00, for low risk; are actually high risk or low risk applications in the original data set as well.

**Recall:** The above algorithm shows recall value of 92% for high risk applications and 94% for low risk applications. This implies that there is a 92% chance that the actual high risk applications will also be predicted to be high risk and there is a 94% chance that the actual low risk applications will also be predicted to be low risk.
## **Summary:**

As per the results, obtained from all six machine learning models, and described above, we clearly see that the choice of a model to predict the credit risk, clearly depends on further course of action as chosen by higher management, based upon what their priority is, or in other words, what feature is more important for a company. They want to base their decision on accuracy scores or precision i.e., reliability of prediction of high risk and low risk values or on the recall, means sensitivity, i.e., people detected at higher risk are those who are actually at high risk. 

The balanced accuracy scores , 66% for **RandomOverSampler** , 65% for **SMOTE** oversampling, 54% for **ClusterCentroids** under sampling , 68% for **SMOTEENN** combination of over and under sampling, 78% for **BalancedRandomForest** classifier  and 93% for **EasyEnsembleClassifier**. 

All first four algorithms have the same value of 0.01 that is 1% for precision of predicted positive classification of high-risk members and last two algorithms have 0.03 and 0.09 that is 3% and 9% precision. 

Furthermore, we have, for high risk members, recall value of 74% for RandomOverSampler, 62% for oversampling, 69% for undersampling, 77% for combination of over and under sampling, 70% for BalancedRandomForest classifier and most of all, 92% for EasyEnsembleClassifier.  

On the basis of above, we clearly see that EasyEnsembleClassifier algorithm has the most balanced accuracy score, most precision and most recall value as compared to others. 

From the above summary, if we consider about precision, which is only 9% for high risk members, it is still not an acceptable percentage, whereas if we see the balanced accuracy score and recall values, we still have the acceptable percentage numerically. 

But it all depends upon companies policies and the important feature combination to decide upon what they consider as important. If they want to proceed with placing actual low risk members which are predicted high risk as per the algorithm used, depending upon how many actual low risk members were labeled as high risk. 

They might want to consider for a tradeoff depending upon what is the requirement of the situation. 

All algorithms have low f1 scores, 2%; except 6% for BalancedRandomClassifier and 16% for EasyEnsembleClassifier but still the scores are not up to acceptable percentages.

On the basis of above , because of the low f1 scores which is the harmony score between precision and recall, due to low precision and recall values, we are unable to recommend any of the above algorithms for prediction of credit card risk.


