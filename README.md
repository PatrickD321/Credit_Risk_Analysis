# Credit Risk Analysis

## Overview of the analysis
  Using accquired basic skill that we just develop in data preparation, statistical reasoning, and machine learning, we will try to analyze a credit card dataset from LendingClub, a peer-to-peer lending services company. Machine learning is the use of statistical algorithms to perform tasks such as learning from data patterns and making predictions. In this real-world situation, we determine the unbalance classification problem between good loans and risky loans that sourrounds the aspect of credit risk. Different number of statical mathematical algorithms will be used to evaluate the dataset in a supervised learning categorory to make vaild predictions. A comparison will made between each of the algorithm that are employed in the analysis.
  
## Deliverable 1: Use Resampling Models to Predict Credit Risk
  Using Pandas and our knowledge of of the imbalanced-learn and scikit-learn libraries, the three machine learning models were evaluated by using resampling to determine which is better at predicting credit risk. The credit_risk_resampling.ipynb script produce the results as follows:
  - An accuracy score for the model is calculated  
      RandomOverSampler - 0.6605446354972261  
      SMOTE - 0.6546563712732358  
      ClusterCentroids - 0.5443246441108096      
      
      
  - A confusion matrix has been generated  
      RandomOverSampler -  ![fig1](https://user-images.githubusercontent.com/78861458/121821803-5e42ca80-cc69-11eb-8953-fc477847f947.png)  
      SMOTE - ![fig2](https://user-images.githubusercontent.com/78861458/121821944-3b64e600-cc6a-11eb-9820-458ea59c145f.png)  
      ClusterCentroids - ![fig3](https://user-images.githubusercontent.com/78861458/121822011-a9a9a880-cc6a-11eb-88a2-25cf8e5f46a4.png)


      
  
