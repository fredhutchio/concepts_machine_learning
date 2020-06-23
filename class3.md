## Concepts in Machine Learning Class 3: Unsupervised Learning

### Objectives

Welcome to class 2 of Concepts in Machine Learning!

In the last class we dug a little deeper into supervised machine learning concepts and methods. Today we will do essentially the same thing but cover unsupervised learning!

By the end of this class you should be able to:

* Define unsupervised learning
* Differentiate between dimensionality reduction and clustering
* Assess whether or not unsupervised learning is an appropriate tool for a question
* Understand basic applications of unsupervised learning (PCA, Kmeans)
* Create unsupervised learning problem statements

### Review! What is machine learning?

Machine learning is a:
* field of study within the larger field of artificial intellegence
* way of programming computers
* an algorithm that incorporates large datasets into a statistical model and improves with experience

### Review! When to use machine learning

Machine learning is especially good at tackeling problems where **you cannot code the rules** and **you cannot scale**.

Some examples we've talked about are:
* Classifying emails as spam
* Recognizing hand written letters
* Predicting a patients clinical outcome
* Clustering cells by cell type based on genetic data

### What is unsupervised machine learning?

The goal of unsupervised learning is to detect the underlying structure and patterns in a dataset with no pre-existing labels. The lack of pre-existing labels means that the algorithm is able to work with minimal human supervision which is why we call these methods 'unsupervised'.

Unlike with supervised learning, unsupervised learning methods do not require annotated training data to work. With no training or testing required there is only one step, fitting.

There are two kinds of supervised learning
1. Unsupervised transformations: Create a new representation of a complex dataset that is easier to understand than the original.
2. Clustering: Partition data into distinct groups of similar objects.

### Some basic examples of supervised machine learning

#### Clustering images by person

<p align="center">
  <img width="350" alt="" src="">
</p>

* Input: Images of people's faces (Ex: the [Labeled Faces in the Wild dataset](https://www.kaggle.com/jessicali9530/lfw-dataset))
* Output: Images sorted so that each unique face found in the dataset has its own folder

#### Grouping handwritten letters

<p align="center">
  <img width="350" alt="" src="images/handwriting.png">
</p>

* Input: Scanned, handwritten letters
* Output: Groups of similar characters
* Dataset: Need thousands of handwritten letters

#### Challenge!

You might have noticed that the second exammple is *almost* identical to yesterdays.

> #### Identifying handwritten letters
>
> * Input: Scanned, handwritten letters
> * Output: The actual character
> * Dataset: Need thousands of handwritten letters and to annotate the correct letter for each one

1. What is the main difference between supervised classification and unsupervised clustering?

### What is fitting?

### What is clustering?

* Clustering is the organization of unlabled data into groups (clusters) based on how similar they are. 
* Clustering is a task that can be accomplished by various algorithms that differ in how they understand what constitutes a cluster and how they find clusters.
* k-means and hierarchical clustering are two common examples of clustering

### Hard vs soft clustering

### Connectivity-based clustering (heirarchical)

<p align="center">
  <img width="600" alt="" src="images/dendogram.png">
</p>

* Based on the core idea of objects being more related to nearby objects than to objects farther away.
* These algorithms connect "objects" to form "clusters" based on their [distance](https://en.wikipedia.org/wiki/Statistical_distance#:~:text=In%20statistics%2C%20probability%20theory%2C%20and,or%20a%20wider%20sample%20of). 
* In a dendrogram, the y-axis marks the distance at which the clusters merge, while the objects are placed along the x-axis such that the clusters don't mix.

* At different distances, different clusters will form, which can be represented using a dendrogram, which explains where the common name "hierarchical clustering" comes from: these algorithms do not provide a single partitioning of the data set, but instead provide an extensive hierarchy of clusters that merge with each other at certain distances.

### Centroid-based clustering (k-means)

### The curse of dimensionality

### Dimensionality reduction

### Principle componant analysis (PCA)

### Evaluation and interpretation of unsupervised learning methods

### Review!

### Next Class

### Reading

https://idyll.pub/post/dimensionality-reduction-293e465c2a3443e8941b016d/
