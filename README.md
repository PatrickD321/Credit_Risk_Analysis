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
      RandomOverSampler 
      
      ![fig1](https://user-images.githubusercontent.com/78861458/121821803-5e42ca80-cc69-11eb-8953-fc477847f947.png)
      
      
      SMOTE 
      
      ![fig2](https://user-images.githubusercontent.com/78861458/121822084-263c8700-cc6b-11eb-806e-d2c8fb47f6b4.png)
      
      
      ClusterCentroids 
      
      ![fig3](https://user-images.githubusercontent.com/78861458/121822011-a9a9a880-cc6a-11eb-88a2-25cf8e5f46a4.png)
      
      
  - An imbalanced classification report has been generated  
    RandomOverSampler
    
    ![fig4](https://user-images.githubusercontent.com/78861458/121822221-e88c2e00-cc6b-11eb-8a16-da1a2ed1d1ef.png)
    
    
    SMOTE
    
    ![fig5](https://user-images.githubusercontent.com/78861458/121822288-4fa9e280-cc6c-11eb-9a33-d03d7c64671f.png)
    
    
    ClusterCentroids
    
    ![fig7](https://user-images.githubusercontent.com/78861458/121822480-48cf9f80-cc6d-11eb-9466-8c14d6015689.png)
    
    
    ## Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
    
    - An accuracy score for the model is calculated (5 pt)
    
    





      
  
