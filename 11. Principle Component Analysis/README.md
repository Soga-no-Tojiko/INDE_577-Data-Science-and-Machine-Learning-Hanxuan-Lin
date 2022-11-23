# Principal Component Analysis (PCA)

Principal component analysis (PCA) is a technique that is useful for the compression and classification of data. The purpose is to reduce the dimensionality of a data set (sample) by finding a new set of variables, smaller than the original set of variables, that nonetheless retains most of the sample's information. By information we mean the variation present in the sample, given by the correlations between the original variables. The new variables, called principal components (PCs), are uncorrelated, and are ordered by the fraction of the total information each retains.

![image](https://user-images.githubusercontent.com/106775775/203593314-b321e23a-f60f-4c55-9bb7-921d23a9e3fe.png)

Basically, it takes five steps to conduct a principal component analysis on a dataset:
1. Standardize the range of continuous initial variables
2. Compute the covariance matrix to identify correlations
3. Compute the eigenvectors and eigenvalues of the covariance matrix to identify the principal components
4. Create a feature vector to decide which principal components to keep
5. Recast the data along the principal components axes

After the analysis, the original data points space is re-projected onto another hyperplane formed by all the orthogonal principle components. However, since the princple components are a linear combination of original attributes, there is usually no explicit meaning of a PC. If model explainablity is important, like building a financial model for risk management, PCA would not be favored.



# Data & Aim

We will use the wine datasets again. Since it has 13 attributes, we are going to see how many principle components would be included after decomposition, and how much variance could be explained by the PCs.

