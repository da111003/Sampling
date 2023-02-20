# Sampling
Sampling Assignment

## Description
Dataset Used : Credit Card
<br>Problem : Binary Classification<br>
<br>
Dataset is imbalanced and is balanced using random over-sampling technique.
Multiple Sampling Techniques are used and 5 different models are applied to get the best accuracy.
The dataset is divided into a 25-75 ratio of testing and training set.

## Methodology
1. Balancing Dataset
2. Creating different types of samples
3. Training different machine learning models
4. Testing the models
5. Analysing the Result obtained

## Sampling Technique Description and Sampling Size Formula
1. Simple Random Sampling
A simple random sample is a subset of a statistical population in which each member of the subset has an equal probability of being chosen.  

<br><b>n = (Z^2 * p * (1- p)) / E^2

>Z = 1.96 (for 95% confidence)
>
>p = 0.5
>
>E = 0.03 (assumed 3%)
>
>n = 1067

2. Stratified Sampling
Stratified sampling is a method of sampling that involves the division of a population into smaller subgroups known as strata.

<br><b>n = (Z^2 * p * (1- p)) / (E/S)^2

>Z = 1.96 (for 95% confidence)
>
>p = 0.5
>
>E = 0.07 (assumed 7%)
>
>S = 2
>
>n = 784 (392 for each class)

3. Systematic Sampling
Systematic sampling is a probability sampling method where we select members of the population at a regular interval.
Samples taken on every 5th interval

4. Cluster Sampling
Cluster sampling is a probability sampling method in which we divide a population into clusters and then randomly select some of these clusters as sample.

>Rows per Cluster = 20
>
>Number of Clusters = 28 (sqrt(n/2) where n is the total number of rows)

5. Multi-Stage Sampling
In this method we have used a combination of sampling technique, i.e. cluster and simple random. The dataset is divided into clusters and then random samples are chosen from those clusters.


## Final Result Table
|                        | Simple Random | Stratified | Systematic | Cluster | Multi-Satge |
| ---------------------- | ------------- | ---------- | ---------- | ------- | ----------- |
| Logistic Regression    |91.11          |91.23       |80.22       |90.00    |96.00        |
| Decision Tree          |99.62          |96.42       |90.90       |94.16    |98.00        |
| Support Vector Machine |69.66          |63.26       |70.12       |72.17    |70.00        |
| Gaussian Naive Bayes   |76.02          |75.00       |77.92       |66.95    |58.00        |
| K-Nearest Neighbors    |98.12          |95.91       |92.20       |88.69    |86.00        |
  

## Discussion
From the table, we can conclude that we achieve maximum accuracy when we apply Decision Tree Algorithm upon taking samples using the Simple Random Sampling technique. We get an accuracy of 99.62%.

___

## License
[MIT](https://choosealicense.com/licenses/mit/)

___

## Written By
Name : Deepak Aggarwal
  
Roll No. : 102003483

Sub-Group: 3COE19
