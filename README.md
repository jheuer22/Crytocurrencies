# Cryptocurrencies
Unsupervised Machine Learning of Cryptocurrencies 

## Analysis Overview 
In this project we are analyzing a database of cryptocurrencies using unsupervised machine learning to classify the data into groups according to their features. Once the data has been cleaned to only contain the currently traded cryptocurrencies, the data is sorted into a class based on our machine learning Model. This data was then used in a couple different visualizations to help display the data groups. This analysis can be used as a point of reference for an investment bank to help determine possible cryptocurrencies that would be good for future investment. 

We use the following methods for our analysis:
- cleaned and preprocessed the database
- reduced the data dimension using Principal Component Analysis
- created cryptocurrency clusters using K-Means
- utilized visual classification results with 2D and 3D scatter plots


## Results 

### Clustering Cryptocurrencies Using K-means

After preprocessing the dataset and reducing it to 532 rows of usable data, we created an Elbow Curve to analyze what k value we would be best to analyze our data with a K-Means algorithm. We plotted the elbow curve from k=0 to k=10 and determined that k=4, or 4 clusters would be best for our analysis.  

![Elbow_curve.png](Resources/Elbow_curve.png)


### Cryptocurrencies Table

When the dataset was grouped based on a k of 4, most of the cryptocurrencies were put into groups 0 or 1. There were only a few cryptocurrencies that were placed into the 2 or 3 classification. 

![Table_Classes.png](Resources/Table_Classes.png)


### 3D-Scatter plot with clusters

Once we determined that we should use 4 clusters, we performed a PCA Analysis to create groups for the data. This is a 3-D visualization was created to display the the 3 reduced dimensions produced in the PCA analysis. 

![3D_PCA.png](Resources/3D_PCA.png)


### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply

Below is a 2-D visualization of the reduces dimensions on TotalCoinsMined and TotalCoinSupply. This visualization is not a great way to represent the data since the differences in the classes are not a obvious. In this case, the 3-D representation from the PCA analysis is a better way to present the data. 

![2D-Scallerplot_TotalMined_v_TotalSupply.png](Resources/2D-Scallerplot_TotalMined_v_TotalSupply.png)


## Summary 

In our analysis we were able to classify 532 cryptocurrencies based on their features using Unsupervised Machine Learning techniques. In order to better recommend these cryptocurrencies on the resulting classifications, I would recommend a deeper dive into the classes that would include performing analysis on performance and potential for growth. This additional information would be valuable in recommendations for future investment.

