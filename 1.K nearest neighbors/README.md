# K nearest neighbor

The K nearest neighbors(KNNs) is an algorithm for classification problem. Its basic thought is to judge the majority label from the nearest k datapoints and take it for the label of that datapoint under searching. KNN is a lazy algorithm that does not require a pre-learning of the dataset. It just scans through every datapoints in the datasets, which could be extremely time-consuming and even suffer from a dimensional disaster. Despite that, KNN has benn commonly used for its simplicity of implementing for many years.



## Datasets


Here we use a dataset of loan default during 2018Q3 from LendingClub, a famous P2P lending company, for this KNN implementation. The datasets include 81 attributes after dropping columns that have imbalanced data and too much NAN values, and more than 100 thousands rows. For simplicity, we only extract ten percent samples from the raw data. Below are some examples of the attribute descriptions:

loan_amnt                   128412 non-null  int64       loan amount in 2018Q3
term                        128412 non-null  int64       loan term in 2018Q3, the raw type is string('36 months')
int_rate                    128412 non-null  float64     the interest rate for each loan
installment                 128412 non-null  float64     the installment for each loan
grade                       128412 non-null  int64       the credit grade for each loan borrower
emp_length                  128412 non-null  int64       the employment length of each loan borrower, the raw data type is string('>10 years')
...
target                      128412 non-null  int64       if a borrower is default in this time period. 1 is for default and 0 is for not default

## Aim


In this project we will focus on using KNN to classify those people who has a high probability of default.
