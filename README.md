# Credit Risk Analysis

## Overview of the analysis
  Using accquired basic skill that we just develop in data preparation, statistical reasoning, and machine learning, we will try to analyze a credit card dataset from LendingClub, a peer-to-peer lending services company. Machine learning is the use of statistical algorithms to perform tasks such as learning from data patterns and making predictions. In this real-world situation, we determine the unbalance classification problem between good loans and risky loans that sourrounds the aspect of credit risk. Different number of statical mathematical algorithms will be used to evaluate the dataset in a supervised learning categorory to make vaild predictions. A comparison will made between each of the algorithm that are employed in the analysis.
  
## Results  
  
### Deliverable 1: Use Resampling Models to Predict Credit Risk
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
    
    
    ###  Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
    
    - An accuracy score for the model is calculated  
        0.6448578411395863 
       
    - A confusion matrix has been generated
      
      ![fig8](https://user-images.githubusercontent.com/78861458/121822987-59cde000-cc70-11eb-9d8a-53b515aed533.png)
      
    - An imbalanced classification report has been generated  
    
      ![fig9](https://user-images.githubusercontent.com/78861458/121823041-b3360f00-cc70-11eb-8f9e-71f64c16b25f.png)
      
     ###  Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk  
       Imblearn.ensemble library will be use to train and compare two different ensemble classifiers. Ensemble learning helps improve machine learning results by combining several models algorithms. This approach allows the production of better predictive performance compared to a single model
      
      BalancedRandomForestClassifier  
      
      - An accuracy score for the model is calculated  
           0.7884948995879731  
           
      - A confusion matrix has been generated  
      
        ![fig10](https://user-images.githubusercontent.com/78861458/121823281-458ae280-cc72-11eb-8c1e-c73e26b56c03.png) 
        
      - An imbalanced classification report has been generated 
      
        ![fig11](https://user-images.githubusercontent.com/78861458/121823472-6e5fa780-cc73-11eb-8074-d95977f01bbe.png)  
        
      - The features are sorted in descending order by feature 

        ![fig13](https://user-images.githubusercontent.com/78861458/121823667-c64ade00-cc74-11eb-932a-a0f223e00419.png)
        
       
      EasyEnsembleClassifier
      
      - An accuracy score of the model is calculated  
         0.9252448999275931

      - A confusion matrix has been generated  
      
        ![fig14](https://user-images.githubusercontent.com/78861458/121823786-702a6a80-cc75-11eb-8505-a8c3122a4db5.png)  
        
       - An imbalanced classification report has been generated  
       
         ![fig15](https://user-images.githubusercontent.com/78861458/121823839-bed80480-cc75-11eb-8995-6a39b23d6d06.png)
         
## Summary  
  
  In credit risk situations, sensitivity of the model is more important than the precision of the algorithms, this will determine how accurately the model will behave at both high risk and low risk level. The models used in deliverable 1 all show a reasonable amount of precision and sensitivity for predicting low risk in the dataset, but precision values for high risk in all three models are low, with the SMOTE algorithm returning the highest values of all three. F1 score is a determination of the imbalance between precision and sensitivity, low scores prove that there are imbalances and higher F1 scores indicates there are far less. The three models have low F1 scores for high-risk detection but reasonable results for low risk, this was seen in the imbalanced classification report. Low F1 scores in high-risk transaction shows that models are not doing a good job of determining accurately transaction that are high risk which will issues to adequately predict candidates who will or may not be delinquent with their accounts.   
       SMOTEENN used in Deliverable 2, combines the SMOTE and Edited Nearest Neighbors (ENN) algorithms. ENN is, if the two nearest neighbors of a data point belong to two different classes, that data point is dropped. Results in SMOTEENN models gave similar results as the models in deliverable 1, and this model offers no improvement in analyzing the dataset.     
   Ensemble learning is the process of combining multiple models, like decision tree algorithms, to help improve the accuracy and robustness, as well as decrease variance the model, and therefore increase the overall performance of the model. In Deliverable 3 we will try to improve on the performances of the previous models and determine which produce the best results for the dataset. The balanced score accuracy gained better values as well as the values in the imbalanced classification report were improved. Easy Ensemble AdaBoost Classifier gives a better a F1 score of 0.14 which is far greater than 0.02 in deliverable 1. Sensitivity and precision were significant higher which is a clear indication of the accuracy and robustness of the two Imblearn models.    
    All models return a perfect score of 1 for low-risk precision, one would prefer to have their model accurately make the correct prediction every time that it is used, but this not normally the case. This is due to the imbalances in the dataset and these imbalances can be address by cleaning the dataset, using only features that have significant  impact on the target value. 





 
      
        

      
        


      
      
        

      
        

        

          

        
           








    
    





      
  
