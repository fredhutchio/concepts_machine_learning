## Concepts in Machine Learning Class 2: Supervised Learning

### Objectives

Welcome to class 2 of Concepts in Machine Learning!

By the end of this class you should be able to:

* Define and understand the limitations of supervised learning
* Differentiate between regression and classification
* Assess whether or not supervised learning is an appropriate tool for a question
* Understand basic applications of supervised learning (linear regression, logistic regression)
* Understand what bias-variance trade off and overfitting are
* Create supervised learning problem statements


### Review! What is machine learning?

### Review! Anatomy of a machine learning problem

### Review! Supervised vs unsupervised machine learning

### What is supervised machine learning?

### How do you train a machine?
* illustrate training / testing with some clear examples ("show a computer thousands of images of hand drawn numbers with the labels containing the correct integer")

### When to use supervised machine learning

### Classification

* Assign a value
* Emphasize necessity of having a 'teacher' - labeled features are what the machine uses to learn how to classify
* Decision trees, support vector machine
* example use cases
 * classic: dog vs cat

### False-positives and false-negatives

### Regression

* Predict a continuous numerical value
* point out that logistic regression is actually a classification method
* linear/polynomial regression
* example use cases
 * classic: predicting income

### Bias-variance trade off
* Bias is the amount of error introduced by approximating real-world phenomena with a simplified model.
* Variance is how much your model's test error changes based on variation in the training data. It reflects the model's sensitivity to the idiosyncrasies of the data set it was trained on.
* As a model increases in complexity and it becomes more wiggly (flexible), its bias decreases (it does a good job of explaining the training data), but variance increases (it doesn't generalize as well). Ultimately, in order to have a good model, you need one with low bias and low variance.

### How to mitigate overfitting

1. More training data
2. 

### Evaluating a supervised learning model

Loss functions

### Practice with problem statements
Use Ted Lederas cvd dataset variables to construct a problem statement. One classification and one regression.

### Review! When to use supervised machine learning

### Review! Regression vs classification

### Review! Bias-variance trade off

### Review! Evaluating a supervised machine learning model

### Next week: Unsupervised learning

### Reading materials

---

## Concepts in Machine Learning Class 3: Unsupervised Learning

### Objectives

Welcome to class 2 of Concepts in Machine Learning!

By the end of this class you should be able to:

* Define unsupervised learning
* Differentiate between dimensionality reduction and clustering
* Assess whether or not unsupervised learning is an appropriate tool for a question
* Understand basic applications of unsupervised learning (PCA, Kmeans)
* Create unsupervised learning problem statements

### Review! What is machine learning?

### Review! Unsupervised vs unsupervised machine learning

### What is unsupervised machine learning?

"Unsupervised learning is a type of machine learning that looks for previously undetected patterns in a data set with no pre-existing labels and with a minimum of human supervision. In contrast to supervised learning that usually makes use of human-labeled data, unsupervised learning, also known as self-organization allows for modeling of probability densities over inputs."

Hinton, Geoffrey; Sejnowski, Terrence (1999). Unsupervised Learning: Foundations of Neural Computation. MIT Press.

### When to use unsupervised learning?

### What is fitting?

### What is clustering?

* Clustering is the organization of unlabled data into groups (clusters) based on how similar they are. 
* Clustering is a task that can be accomplished by various algorithms that differ in how they understand what constitutes a cluster and how they find clusters.
* k-means, hierarchical clustering

### Hard vs soft clustering

### Connectivity-based clustering (heirarchical)

"Connectivity-based clustering, also known as hierarchical clustering, is based on the core idea of objects being more related to nearby objects than to objects farther away. These algorithms connect "objects" to form "clusters" based on their distance. A cluster can be described largely by the maximum distance needed to connect parts of the cluster. At different distances, different clusters will form, which can be represented using a dendrogram, which explains where the common name "hierarchical clustering" comes from: these algorithms do not provide a single partitioning of the data set, but instead provide an extensive hierarchy of clusters that merge with each other at certain distances. In a dendrogram, the y-axis marks the distance at which the clusters merge, while the objects are placed along the x-axis such that the clusters don't mix." wikipedia

### Centroid-based clustering (k-means)

### The curse of dimensionality

### Dimensionality reduction

### Principle componant analysis (PCA)

### Evaluation and interpretation of unsupervised learning methods

### Review!

### Next Class

### Reading
