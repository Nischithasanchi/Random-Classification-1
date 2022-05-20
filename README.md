# RANDOM CLASSIFICATION
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Related Theoritical Concept:
A Random Forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting.Random forest classifier creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object.

## Algorithm
1.In Random forest n number of random records are taken from the data set having k number of records.

2.Individual decision trees are constructed for each sample.

3.Each decision tree will generate an output.

4.Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.

## Program:
```
/*
Program to implement random classification.
Developed by   : SANCHI NISCHITHA
RegisterNumber :  212219040097
*/
import matplotlib.pyplot as plt
from sklearn import datasets
X,y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)
fig=plt.figure(figsize=(10,8))
plt.plot(X[:,0][y==0], X[:,1][y==0],'pc')
plt.plot(X[:,0][y==1], X[:,1][y==1],'bo')
plt.xlabel("Feature 1")
plt.ylabel("Feaure 2")
plt.title("Random Classification Data with 2 classes")

## Output
![163679559-de878cf3-01d8-4fed-b647-b023fc13461b](https://user-images.githubusercontent.com/104021170/169485234-cad3b297-ff6b-4f09-9981-57ffcf9230a5.jpg)




## Result:
Thus the random classifier was successfully implemented using python programming.
