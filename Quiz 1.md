## Quiz 1 Result:

###### Question 1
Which of the following statements are true?

* Clustering analysis in unsupervised learning since it does not require labeled training data. :white_check_mark:
* It is impossible to cluster objects in a data stream. We must have all the data objects that we need to cluster ready before clustering can be performed.:x:
* Clustering analysis has a wide range of applications in tasks such as data summarization, dynamic trend detection, multimedia analysis, and biological network analysis.:white_check_mark:
* When clustering, we want to put two dissimilar data objects into the same cluster.:x:

---
###### Question 2
What are some common considerations and requirements for cluster analysis?

* We need to consider how to incorporate user preference for cluster size and shape into the clustering algorithm.:white_check_mark:
* In order to perform cluster analysis, we need to have a similarity measure between data objects.:white_check_mark:
* We need to be able to handle a mixture of different types of attributes (e.g., numerical, categorical).:white_check_mark:
* We must know the number of output clusters a priori for all clustering algorithms.:x:

---
###### Question 3
Which of the following statements are true?

* Graphs, time-series data, text, and multimedia data are all examples of data types on which cluster analysis can be performed.:white_check_mark:
* Agglomerative clustering is an example of a distance-based clustering method.:white_check_mark:
* When dealing with high-dimensional data, we sometimes consider only a subset of the dimensions when performing cluster analysis.:white_check_mark:
* We can only visualize the clustering results when the data is 2-dimensional.:x:


---
###### Question 4
The following real dataset contains information about Iris setosa and versicolor.
What is the __Euclidean distance__ between these two objects?

|Species|Sepal length|Sepal width|Petal length|Petal width|
| ----- |:----------:| ---------:| ----------:| ---------:|
| Iris setosa| 4.9|	3.0|	1.4	|0.2 |
|Iris versicolor|	5.6|	2.5|	3.9|	1.1|

__Result: 2.8__:white_check_mark:


---
###### Question 5
The following real dataset contains information about Iris setosa and versicolor.

|Cases|	F1|	F2|	F3|	F4|	F5|	F6|	F7|	F8|	F9|	F10|
| --- |:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|__1__|	0|	1|	1|	0|	0|	0|	1|	1|	1|	1|
|__2__|	0|	1|	0|	0|	1|	0|	1|	0|	0|	1|
Assume all the activities are asymmetric binary variables. What is the distance between Case 1 and Case 2?

__d(i,j) = r + s / q + r + s = 4/7__ :white_check_mark:


---
###### Question 6
The following real world dataset contains two samples from Car Evaluation Database, which was derived from a simple hierarchical decision model originally developed for the demonstration of DEX (M. Bohanec, V. Rajkovic: Expert System for Decision Making. Sistemica 1(1), pp. 145-157, 1990.).  The model evaluates cars according to the following concept structure:

...

To calculate the distance between objects with categorical attributes, we use a set of binary attributes to represent each categorical attribute. Assume all the binary attributes are symmetric. What is the distance between Car 1 and Car 2?


* s:4
* r:4
* q:2
* t:11


__d(i,j) = s+r/q+s+r+t = 8/21__ :white_check_mark:

---
###### Question 7
Given the following two short texts with punctuation removed, calculate the cosine similarity between them based on the bag of words model.

__Text1__: all grown-ups were once children but only few of them remember it

__Text2__: all children should be very understanding of grown-ups

T1 = (1, 1, 1, 1, 1, 1, 1, 1, 1, 1,1, 1, 0, 0, 0, 0)

T2 = (1, 1, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 1, 1, 1)

cos(T1,T2) = T1*T2/ ||T1|| ||T2|| = 4/ √12 √ 8

__Result: 0.408__ :white_check_mark:


---
###### Question 8
With regard to the species of Iris versicolor, we have sampled data on the features of sepal length and sepal width, as follows:

|Feature|	Sepal length|	Sepal width|
|------:|--------------:|--------------|
|Case 1|	7.0|	3.2|
|Case 2|	6.4|	3.2|
|Case 3|	6.9|	3.1|
|Case 4|	5.5|	2.3|
|Case 5|	6.5|	2.8|

What is the correlation coefficient between sepal length and sepal width?


ρ12 = σ12/σ1 σ2 = nΣi=l (xil - μl)(xi2 - μ) / √ nΣi=l (x - μ2)2

__Result: 0.882__ :white_check_mark:


---
###### Question 9

Considering the K-means algorithm, after current iteration, we have 3 centroids (0, 1) (2, 1), (-1, 2). Will points (2, 3) and (2, 0.5) be assigned to the same cluster in the next iteration?


__Result: YES__ :white_check_mark:

---
###### Question 10

Considering the K-means algorithm, if points (-1, 3), (-3, 1), and (-2, -1) are the only points which are assigned to the first cluster now, what is the new centroid for this cluster?


__Result: (-2, 1)__ :white_check_mark:

---
###### Question 11

K-means++ algorithm is designed for better initialization for K-means, which will take the farthest point from the currently selected centroids. Suppose k = 2 and we have selected the first centroid is (0, 0). Among the following points (these are all the remaining points), which one should we take for the second centroid?


__Result: (3, 0)__ :white_check_mark:


---
###### Question 12

Considering the K-median algorithm, if points (0, 3), (2, 1), and (-2, 2) are the only points which are assigned to the first cluster now, what is the new centroid for this cluster?


__Result: (0, 2)__ :white_check_mark:

---
###### Question 13

Which of the following statements about the K-means algorithm are correct?

* The K-means algorithm is sensitive to outliers.:white_check_mark:

* For different initializations, the K-means algorithm will definitely give the same clustering results.:x:
* The centroids in the K-means algorithm may not be any observed data points.:white_check_mark:

* The K-means algorithm can detect non-convex clusters.:x:
