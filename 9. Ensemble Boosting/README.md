# Ensemble boosting

The ensemble boosting algorithms introduced in this course include Adaboost and Gradient Boosting Decision Tree(GBDT).

The core principle of AdaBoost is to fit a sequence of weak learners (i.e., models that are only slightly better than random guessing, such as small decision trees) on repeatedly modified versions of the data. The predictions from all of them are then combined through a weighted majority vote (or sum) to produce the final prediction. The data modifications at each so-called boosting iteration consist of applying a group of weights to each of the training samples. Initially, those weights are all set to 1/N, where N is the sample size, so that the first step simply trains a weak learner on the original data. For each successive iteration, the sample weights are individually modified and the learning algorithm is reapplied to the reweighted data. At a given step, those training examples that were incorrectly predicted by the boosted model induced at the previous step have their weights increased, whereas the weights are decreased for those that were predicted correctly. As iterations proceed, examples that are difficult to predict receive ever-increasing influence. Each subsequent weak learner is thereby forced to concentrate on the examples that are missed by the previous ones in the sequence.

![image](https://user-images.githubusercontent.com/106775775/202560928-fc4b2496-9506-455f-88d9-a65c7689cfd7.png)

Gradient boosting is a machine learning technique used in regression and classification tasks, among others. It gives a prediction model in the form of an ensemble of weak prediction models, which are typically decision trees. When a decision tree is the weak learner, the resulting algorithm is called gradient-boosted trees; it usually outperforms random forest. A gradient-boosted trees model is built in a stage-wise fashion as in other boosting methods, but it generalizes the other methods by allowing optimization of an arbitrary differentiable loss function.

# Data

Again, we will use dry bean datasets to solve a classification problem. 

# Aim

For both Adaboost and GBDT, this time we will also tune the hyperparameters to search for a best model.
