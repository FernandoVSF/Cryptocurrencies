# Cryptocurrencies
  Analysis of Cryptocurrencies
  
## Overview of the analysis
Create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. To group the cryptocurrencies, we used a clustering algorithm. Then we will visualizations to share the findings.  The following outputs were produced:

- Preprocessing the Data for PCA
- Reducing Data Dimensions Using PCA
- Clustering Cryptocurrencies Using K-means
- Visualizing Cryptocurrencies Results



The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.
The following outpits will be produced:

- Use Resampling Models to Predict Credit Risk
- Use the SMOTEENN Algorithm to Predict Credit Risk
- Use Ensemble Classifiers to Predict Credit Risk
- A Written Report on the Credit Risk Analysis (README.md)

## Resources
- Data Source: crypto_data.csv file
- Software: Python, Jupyter Notebook, Pandas, HVplot, Plotly, SKLearn

## Results
We analysed different models, and below we present the balanced accuracy, precision and recall scores for each of them:

### Naive Random Oversampling
  - Bal. Accuracy: 0.65
  - Precision:     0.99
  - Recall:        0.61

   ![naive](/naive.png)
  
### SMOTE Oversampling
  - Bal. Accuracy: 0.66
  - Precision:     0.99
  - Recall:        0.69

   ![smote](/smote.png)

### Undersampling
  - Bal. Accuracy: 0.58
  - Precision:     0.99
  - Recall:        0.58

   ![under](/under.png)
   
### Combination (Over and Under) Sampling
  - Bal. Accuracy: 0.64
  - Precision:     0.99
  - Recall:        0.57

   ![combi](/combi.png)   
   
### Balanced Random Forest Classifier
  - Bal. Accuracy: 0.79
  - Precision:     0.99
  - Recall:        0.87

   ![BRF](/BRF.png)   

### Easy Ensemble AdaBoost Classifier
  - Bal. Accuracy: 0.93
  - Precision:     0.99
  - Recall:        0.94

   ![EEC](/EEC.png)   
  
## Summary

Please find below a summary table of all analysis:

Model | Bal Accy | Precision | Recall
--- | --- | --- | --
NRO | 0.65 | 0.99 |0.61
SMOTE | 0.66 | 0.99 | 0,69
Undersampling | 0.58 | 0.99 | 0.58
Combination | 0.64 | 0.99 | 0.57
BRF | 0.79 | 0.99 | 0.87
EEC | 0.93 | 0.99 | 0.94

Looking at the results, we can conclude that we have high precision scores for all models, since given data assymetry, not many low risk are predicted as high risk.  However we can see a lot of difference in the models through the recall score, which shows the ability of finding all positive high risk samples.

Therefore, we recommend using Easy Ensemble AdaBoost Classifier, since it ensemblse AdaBoost learners trained on different balanced boostrap samples, increasing the ability of finding positive high risk samples, providing the highest ballanced accuracy score.

In the other hand we don't recommed for this exercise the use of undersampling, since it involves loss of data from the majority class, decreasing even more the recall rate, and therefore, the ballanced accuracy score.
