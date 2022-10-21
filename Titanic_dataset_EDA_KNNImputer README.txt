Missing Values in the dataset is one heck of a problem before we could get into Modelling.

A lot of machine learning algorithms demand those missing values be imputed before proceeding further.

The popular (computationally least expensive) way that a lot of Data scientists try is to use mean / median / mode or if it’s a Time Series, then lead or lag record.

There must be a better way — that’s also easier to do — which is what the widely preferred KNN-based Missing Value Imputation.

Each sample’s missing values are imputed using the mean value from n_neighbors nearest neighbors found in the training set. 

Two samples are close if the features that neither is missing are close.

By default, a euclidean distance metric that supports missing values, nan_euclidean_distances, is used to find the nearest neighbors.

THIS NOTEBOOK HAS BEEN DONE USING KNN IMPUTER TO FILL THE MISSING VALUES AND SKEWNESS IS PLOTTED.

DATASET: TITANIC DATASET 