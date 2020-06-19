# What Code to look at
## main.ipynb 
This is the code with the latest progress. It uses 8 columns from the breast cancer dataset. Each column has a linear correlation with at least one other column. The dataset is filled with 5% missing values, defined as "10000000". The neural network reconstructs the whole dataset and tries to predict the missing values. It learns and predicts all values, and prints two loss values - one for all predicted values and one for predicted missing values.

**CURRENT STATUS:**
1) Losses on normalized data reaches 0.03 which is still high considering that the data is normalized between 0 and 1
2) Neural network almost always predicts the same values (the mean for each column) - overfitting?

## eckerle.ipynb
Uses eckerle dataset with a distribution similar to a normal distribution. This code is used to show how a pearson R value fails to detect any relationship, but the neural network can still reconstruct the second column from the first even in an unseen set, suggesting that it can detect such relationships.

## Other
The other files were written for experimentation and for learning basic pytorch

#### model1.ipynb
Reconstructs a single column based on other columns from the IRIS dataset

#### model2.ipynb
Reconstructs a single column based on other columns from the Breast Cancer Dataset

#### model3.ipynb
Autoencoder that reconstructs linear correlations in wisconsin breast dataset 

#### model4.ipynb
Autoencoder that reconstructs custom dataset consisting of normal distribution correlation with gaussian noise


#### breast_classifier.ipynb
Classifies breast dataset as Benign or Malignant

#### iris.py.ipynb
Classifies the type of iris

## CSV Files
These are newly constructed dataset, saved for testing accuracy of classifiers