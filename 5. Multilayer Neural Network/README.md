# Multilayer Neural Networks

A fully connected multi-layer neural network is called a Multilayer Perceptron (MLP) or Multilayer Neural Networks. It has at least 3 layers including one input layer, one output layer and at least one hidden layer. An MLP is a typical example of a feedforward artificial neural network. It can efficiently handle very non-linear data, discovering its features with deep hidden layer structures. However, MLP model structure could be so complex that it usually overfits the data. 

# Data

We will continue to use wine datasets to implement the multilayer neural networks. However, one needs to be cautious while implementing MNN onto a dataset that has a limited dimensions(attributes) and samples because it usually leads to a too sophisticated model frameworks and overfitting.

# Aim

Since in the previous attempts, we found that single layer perceptron cannot find a separation plane on a non-linear separable dataset, here we will try instead to implement MNN to see if it works well on the datasets.
