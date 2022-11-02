# Perceptron(Single Layer)

A perceptron is a neuron that receives inputs and produce an output. Basically a linear regression model is a kind of perceptron. The structure of perceptron includes an input layer, a hidden layer, an activation function and an output layer. The activation function(ReLU, Sigmoid) transform numerical values onto a binary space of {0,1} in the case of perceptron.

# Datasets

Here we use a dataset of wine data from UCI machine learning repository. The whole datasets have 178 rows and 13 attributes, with the target column is the type label of wine. The wine types are ternary from 1 to 3. The attributes are generally some facets that a type of wine could have, like the alcohol and ash flavor.

1) Alcohol: The alcohol by volume in a specific type of wine
2) Malic acid: The concentration of malic acid in a specific type of wine
3) Ash: the concentration of ash content produced during aging in wine
4) Alcalinity of ash: the concentration of alkali in ash content
5) Magnesium: the concentration of magnesium(Mg) in wine 
6) Total phenols: the concentration of phenols in wine
7) Flavanoids: the concentration of flavanoids in wine
8) Nonflavanoid phenols: the concentration of nonflavanoid phenols in wine
9) Proanthocyanins: the concentration of proanthocyanins in wine
10) Color intensity: the color darkness of wine
11) Hue: the hue of wine
12) OD280/OD315 of diluted wines: This is a method for determining the protein concentration, which can determine the protein content of various wines.
13) Proline: the concentration of proline(a kind of amino acid) in wine.

# Aim

We would use a single layer perceptron model to predict the default condition of each loan borrower.
