# Perceptron(Single Layer)

A perceptron is a neuron that receives inputs and produce an output. Basically a linear regression model is a kind of perceptron. The structure of perceptron includes an input layer, a hidden layer, an activation function and an output layer. The activation function(ReLU, Sigmoid) transform numerical values onto a binary space of {0,1} in the case of perceptron.

# Datasets

Here we use a dataset of loan default during 2018Q3 from LendingClub, a famous P2P lending company, for this KNN implementation. We would probably use the same datasets for the other algorithms as it is a very comprehensive. The datasets include 81 attributes after dropping columns that have imbalanced data and too much NAN values, and more than 100 thousands rows. For simplicity, we only extract around 6000 rows from the raw data. Below are some examples of the attribute descriptions:

loan_amnt 128412 non-null int64 loan amount in 2018Q3

term 128412 non-null int64 loan term in 2018Q3, the raw type is string('36 months')

int_rate 128412 non-null float64 the interest rate for each loan

installment 128412 non-null float64 the installment for each loan

grade 128412 non-null int64 the credit grade for each loan borrower

emp_length 128412 non-null int64 the employment length of each loan borrower, the raw data type is string('>10 years')

...

target 128412 non-null int64 if a borrower is default in this time period. 1 is for default and 0 is for not default

# Aim

We would use a single layer perceptron model to predict the default condition of each loan borrower.
