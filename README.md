## Firstly we clean up the data from our [housing.csv](https://github.com/rituraj-navindgikar/ML/blob/main/housing.csv) file 
- We find correlations in data using seaborn's heatmap, these are the features with very high correlations and teach the model same thing again and again
- therefore we combine those into a new feature and delete the old features

## The General Step is to
- Impute missing data
- Handling outliers
- Understanding correlations
- feature engineering
- encoding
- algorithm experimentation
  
## This Python Notebook uses the following Supervised learning Approaches to train and test on [housing.csv](https://github.com/rituraj-navindgikar/ML/blob/main/housing.csv)
- LINEAR REGRESSION 
- RANDOM FOREST REGRESSOR
- XGBoost


## Clustering
### k-means clustering
1. choose a number `k` and distance metric
2. find k nearest neighbors of sample that we want to classify
3. assign the class label by majority vote
4. update the centriods of each class
5. repeat steps above untill convergence


## K Evaluation for K-Means
- we specify the `k value` for k-means clustering. However, we do not know the best `k value` for given dataset
### 1. Elbow Method
- track the intertia of model as `k value` increases, the inertia is the sum of squared distances of samples to their closest cluster center
### 2. Silhouette coefficient
- the silhouette coefficient is a measure of how similar an object is to its own cluster compared to other clusters, ranges from -1 to +1