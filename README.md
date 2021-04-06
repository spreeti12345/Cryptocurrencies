# Cryptocurrencies

## Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
We use the following methods for the analysis:
 1: Preprocessing the Data for PCA
 2: Reducing Data Dimensions Using PCA
 3: Clustering Cryptocurrencies Using K-means
 4: Visualizing Cryptocurrencies Results

## Resources
Data Source: crypto_data.csv, CryptoCompare
Software: Python, Anaconda Navigator, Jupyter Notebook 

## Results
Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies.


Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies.
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

<img width="539" alt="Elbow curve" src="https://user-images.githubusercontent.com/74282781/113672308-69c3b500-966c-11eb-99c5-7aac57ac6b57.png">

The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

## Visualizing Cryptocurrencies Results

### 3D-Scatter plot with clusters
<img width="670" alt="3d Scatter plot" src="https://user-images.githubusercontent.com/74282781/113672346-79db9480-966c-11eb-9156-262d11df19a8.png">


This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.

The scatter plots show the distribution and the four clusters of cryptocurrencies.
We can identify the outliers like the unique cryptocurrency in the class #2.

### Tradable Cryptocurrencies Table

<img width="587" alt="tradable cryptocurrencies" src="https://user-images.githubusercontent.com/74282781/113672945-33d30080-966d-11eb-87e8-1ed268d1c3fc.png">

Most of the cryptocurrencies are part of class #0 and #1.
The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.


### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply
<img width="587" alt="PCA plot" src="https://user-images.githubusercontent.com/74282781/113672423-9d9eda80-966c-11eb-838c-cd4527bd48da.png">


Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

## Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features.
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.
