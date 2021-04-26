# Written Analysis of the Supervised Machine Learning and Credit Risk challenge Module 17

## Overview of Analysis
This project purpose is to use Python and Scikit-learn library to build and evaluate different machine learning models to help predict credit risk. Using the models compare the strengths and weaknesses of these 6 models and access how well a model work to finally recommend which machine learning model should be used to predict credit risk by the Fastlending peer to peer credit lending company. To arrive at the 6 machine learning models the following approach was used:

- Oversampling the data using the RandomOverSampler and SMOTE algorithms.
- Undersamping the data using the ClusterCentroids algorithm.
- Combination sampling (of Over and Under) using the SMOTEENN algorithm.
- Use Ensemble Learners Balanced Random Forest Classifier and an Easy Ensemble AdaBoost to compare two machine learning models that reduce bias, to determine which algorithm results in the best performance.


Data Source: 
![LoanStats_2019Q1.csv]

## Deliverable: 
This challenge consists of three technical analysis deliverables and a written report to present results. 

- Deliverable 1: Use Resampling Models to Predict Credit Risk
- Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
- Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)


## Results

The results are displayed on Jupiter notebooks links 

![credit_risk_resampling.ipynb](https://github.com/archinarula/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb) and
![credit_risk_ensemble.ipynb](https://github.com/archinarula/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)

Key findings and highlights of this analysis is:

1. Naive Random Oversampling Model:

The balanced accuracy score is 66%.
There is low high_risk population (87), with high_risk precision about 1% only with 64% sensitivity 
There is high number of the low_risk population(17118), its precision is almost 100% with a sensitivity of 67% 

2. SMOTE Oversampling Model:

The balanced accuracy score is 63%.
There is low high_risk population (87), with high_risk precision about 1% only with 62% sensitivity 
There is high number of the low_risk population(17118), its precision is almost 100% with a sensitivity of 64% 

3. ClusterCentroids Undersampling Model:

The balanced accuracy score is 51%.
There is low high_risk population (87), with high_risk precision about 1% only with 59% sensitivity 
There is high number of the low_risk population(17118), its precision is almost 100% with a sensitivity of 43%


4. SMOTEENN Combination Sampling Model:

The balanced accuracy score is 62%.
There is low high_risk population (87), with high_risk precision about 1% only with 70% sensitivity 
There is high number of the low_risk population(17118), its precision is almost 100% with a sensitivity of 54%

5. Balanced Random Forest Classifier Ensemble Learners Model:

The balanced accuracy score is 79%.
There is low high_risk population (87), with high_risk precision about 4% only with 67% sensitivity 
There is high number of the low_risk population(17118), its precision is almost 100% with a sensitivity of 91%

6. Easy Ensemble AdaBoost Classifier Ensemble Learners Model:

The balanced accuracy score is 93%.
There is low high_risk population (87), with high_risk precision about 7% only with 91% sensitivity 
There is high number of the low_risk population(17118), its precision is almost 100% with a sensitivity of 94%

## Summary

All 6 models show weak precisions for the high risk population in determining credit risk
The Ensemble models are far better than the Over, Under or Combination sampling methods due to its higher accuracy score and improved sensitivity in determining credit risk

Recommendations:
From the 6 definately the Easy Ensemble AdaBoost Classifier Model is the best to use with the highest accuracy score of 93% and improved sensitivity of 91% for determining credit risk of high risk population. 

However since this models precision rate is also very low (7%) so lots of low risk credits are falsely predicted as high risk which would be not good for the lending agency/bank as it would miss opportunity to extend credit to those good customers. Hence, I will not recommend any of these 6 models would be good for the bank to determine credit rating as precision rate needs to be higher for the model to work well for this business scenario. 







 



