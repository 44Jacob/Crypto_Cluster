# Crypto_Cluster
##Cryptocurrency Market Analysis

This project conducts a thorough analysis of cryptocurrency market trends and clusters different cryptocurrencies based on their price change percentages over multiple timeframes using K-Means clustering. We utilize various data science techniques, including scaling, PCA for dimensionality reduction, and visualization to interpret our findings.

Installation
To run this project, you need the following libraries:

pandas
hvplot.pandas
scikit-learn
You can install these packages via pip: “ pip install pandas hvplot scikit-learn”

Data
The dataset used is crypto_market_data.csv, which includes the following features for various cryptocurrencies:

price_change_percentage_24h
price_change_percentage_7d
price_change_percentage_14d
price_change_percentage_30d
price_change_percentage_60d
price_change_percentage_200d
price_change_percentage_1y

Usage

Load and Inspect Data:
Load the data into a pandas DataFrame and inspect initial rows and descriptive statistics to understand distributions and variance.

Data Preprocessing:
Scale the data using StandardScaler to normalize feature scales, ensuring effective clustering.
Exploratory Analysis: Use hvPlot to create line charts of the data to visualize trends.

K-Means Clustering:
Determine the optimal number of clusters (k) using the Elbow method.
Fit the K-Means model and predict the clusters to group the cryptocurrencies.
Visualize the clusters using hvPlot scatter plots.

PCA Optimization:
Apply PCA to reduce dimensions to three principal components.
Re-apply K-Means using the PCA-transformed data and compare the inertia values.
Visualize and analyze differences in clustering outcomes.

Results Analysis:
Visually compare the clustering results obtained with and without PCA optimization.

Visualizations
The project includes various visualizations:

1-Line charts to view initial data trends.
2-Elbow curves to identify the optimal number of clusters.
3-Scatter plots to visualize clustering of cryptocurrencies both pre and post PCA.


Results
The analysis concludes that using PCA for dimensionality reduction maintains consistent clustering while slightly adjusting data dispersion. The project successfully demonstrates the impact of using fewer features on the robustness and accuracy of clustering outcomes.

Conclusions
This detailed examination of cryptocurrency market trends and clustering provides insights into market dynamics and the effectiveness of using advanced analytical techniques like PCA in understanding complex datasets.
