# Cryptocurrencies
  Analysis of Cryptocurrencies
  
## Overview of the analysis
Create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. To group the cryptocurrencies, we used a clustering algorithm. Then we will use visualizations to share the findings.  The following outputs were produced:

- Preprocessing the Data for PCA
- Reducing Data Dimensions Using PCA
- Clustering Cryptocurrencies Using K-means
- Visualizing Cryptocurrencies Results

## Resources
- Data Source: crypto_data.csv file
- Software: Python, Jupyter Notebook, Pandas, HVplot, Plotly, SKLearn

## Results
To accomplish the goal,  we needed to preprocess the database, performing an ETL to prepare the date to be used in the machine learning models.  We decided for unsupevised machine learning, as there is no known output for what we are looking for.  We used PCA to reduce dimension of the variables to three principal components.  After deciding in how many clusters to be used to group the cryptocurrencies we used a K-Means model to get the clusters.  We produced the following visualiztions:
\

   

### Undersampling
  - Bal. Accuracy: 0.58
  - Precision:     0.99
  - Recall:        0.58

   ![under](/under.png)
   
