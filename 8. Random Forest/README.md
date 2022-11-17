# Random Forest

Random forests is a supervised learning algorithm. It can be used both for classification and regression. It is also the most flexible and easy to use algorithm. A forest is comprised of trees. It is said that the more trees it has, the more robust a forest is. Random forests creates decision trees on randomly selected data samples, gets prediction from each tree and selects the best solution by means of voting. It also provides a pretty good indicator of the feature importance. The algorithm works in four steps:

1. Select random samples from a given dataset.
2. Construct a decision tree for each sample and get a prediction result from each decision tree.
3. Perform a vote for each predicted result.
4. Select the prediction result with the most votes as the final prediction.

![image](https://user-images.githubusercontent.com/106775775/202558852-547bb40e-fe63-443f-9cd1-32232cd6b8f9.png)


Advantages:
1. Random forests is considered as a highly accurate and robust method because of the number of decision trees participating in the process.
2. It does not suffer from the overfitting problem. The main reason is that it takes the average of all the predictions, which cancels out the biases.
3. The algorithm can be used in both classification and regression problems.
4. Random forests can also handle missing values. There are two ways to handle these: using median values to replace continuous variables, and computing the proximity-weighted average of missing values.
5. The algorithm can get the relative feature importance, which helps in selecting the most contributing features for the classifier.

Disadvantages:
1. Random forests is slow in generating predictions because it has multiple decision trees. Whenever it makes a prediction, all the trees in the forest have to make a prediction for the same given input and then perform voting on it. This whole process is time-consuming.
2. The model is difficult to interpret compared to a decision tree, where you can easily make a decision by following the path in the tree.

Random Forests vs Decision Trees
1. Random forests is a set of multiple decision trees.
2. Deep decision trees may suffer from overfitting, but random forests prevents overfitting by creating trees on random subsets.
3. Decision trees are computationally faster.
4. Random forests is difficult to interpret, while a decision tree is easily interpretable and can be converted to rules.

# Data

Here we continue to use the dry bean datasets used in decision tree. Please view that folder to see the data descriptions.

# Aim

We will use both bagging classifier and random forest classifier to see if one of the algorithms outperforms or not.
