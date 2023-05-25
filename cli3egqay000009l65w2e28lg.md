---
title: "Understanding K-Nearest Neighbors (KNN) Algorithm"
datePublished: Thu May 25 2023 17:20:21 GMT+0000 (Coordinated Universal Time)
cuid: cli3egqay000009l65w2e28lg
slug: understanding-k-nearest-neighbors-knn-algorithm
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1685035115985/02928d16-1d87-4c5f-86e5-b9b78d6cd680.png
tags: data-science, machine-learning, regression, knn, sajjadrahman

---

K-Nearest Neighbors (KNN) algorithm is one of the simplest and most widely used classification algorithms in machine learning. KNN is a non-parametric algorithm that can be used for classification or regression. It is a supervised learning algorithm in which the input consists of labeled data points and the output is the class membership of a new data point. In this post, we'll look at how KNN works and how it can be used.

## How KNN Works

The KNN algorithm is based on the idea that similar data points are more likely to have the same label. In other words, if a new data point is similar to the majority of the data points in a class, it is likely to belong to that class.

The KNN algorithm works as follows:

1. Choose a value for K (the number of neighbors to consider).
    
2. Given a new data point, find the K nearest neighbors (data points) based on some distance metric (such as Euclidean distance).
    
3. Determine the class membership of the new data point based on the class membership of the K nearest neighbors (for classification) or the average of their values (for regression).
    

## Example

Let's say we want to use the KNN algorithm to classify whether a fruit is an apple or an orange, based on its weight and size. We have the following data:

| Weight (grams) | Size (cm) | Label |
| --- | --- | --- |
| 100 | 5 | apple |
| 150 | 7 | orange |
| 200 | 8 | orange |
| 120 | 6 | apple |
| 170 | 7 | orange |
| 130 | 6.5 | apple |

Suppose we want to classify a fruit that weighs 140 grams and is 6.5 cm in size. We can use the KNN algorithm as follows:

1. Choose a value for K, let's say K=3.
    
2. Find the 3 nearest neighbors to the new data point (140, 6.5) based on some distance metric (such as Euclidean distance). The nearest neighbors are (120, 6), (130, 6.5), and (150, 7).
    
3. Determine the class membership of the new data point based on the class membership of the K nearest neighbors. The 3 nearest neighbors are 2 apples and 1 orange, so the new data point is classified as an apple.
    

## Conclusion

K-Nearest Neighbors (KNN) algorithm is a simple but powerful classification algorithm in machine learning. It is easy to understand and implement and can be used for both classification and regression tasks. KNN is a flexible algorithm that can be used with different distance metrics and values of K. However, it is computationally expensive for large datasets and may not work well with high-dimensional data.