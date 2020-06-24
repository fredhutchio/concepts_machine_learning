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

### Review! Anatomy of a machine learning problem

**Example: we are trying to predict whether or not someone will be diagnosed with cardiovascular disease.**

Here's an example training dataset for predicting whether or not a patient might be diagnosed with cardiovascular disease. This dataset shows paired input and output data and would be considered an annotated or labeled training dataset.

| patient_Id    | age   | htn | treat | smoking | race     | t2d | gender | numAge | bmi | tchol| sbp | cvd |
| ------------- | ----- | --- | ----- | ------- | -------- | --- | ------ | ------ | --- | ---- | --- | --- |
| HHUID00076230 | 20-40 | Y   | Y     | N       | Asian/PI | N   | M      | 29     | 23  | 189  | 170 | N   |
| HHUID00547835 | 70-90 | N   | Y     | N       | White    | Y   | M      | 72     | 35  | 178  | 118 | N   |

**Reality/truth:** a persons health history, location, occupation, diet, habits, stress levels, among many other things will play into if someone gets cardiovascular disease. 

**Dataset:** when creating the dataset that will be used to make our predictions we will never capture the whole truth. We will capture as much of the truth as we can by collecting data on various features that we believe are related to the problem we are trying to solve. Many underlying factors that lead to the cardiovascular disease may be unknown or we might not be able to measure them or capture them in our dataset.

**Features/variables:** These are the measurable data that make up our dataset. Some features collected might be useless while others might carry a substantial amount of weight in making the prediction. Since this is a training set one of the variables included is the label that we are trying to predict (`cvd`).

**Inputs:** Features that we have collected and will use to make our prediction. In this dataset our inputs would be all of the columns except `patient_Id` and `cvd`. We would likely remove `pateint_Id` because a random identifier won't have any predictive power and `cvd` would not be included as an input since it is the target we are trying to predict.

**Output:** The variable that we are trying to predict. In this case `cvd`.

**Object:** An object is the variable we are trying to cluster on. In this case we might want to cluster patients to identify subgroups or outliars so `patient_Id` would represent each object. 

### What is unsupervised machine learning?

The goal of unsupervised learning is to detect the underlying structure and patterns in a dataset with no pre-existing labels. The lack of pre-existing labels means that the algorithm is able to work with minimal human supervision which is why we call these methods 'unsupervised'.

Unlike with supervised learning, unsupervised learning methods do not require annotated training data to work. With no training or testing required there is only one step, fitting.

There are two kinds of supervised learning
1. Unsupervised transformations: Create a new representation of a complex dataset that is easier to understand than the original.
2. Clustering: Partition data into distinct groups of similar objects.

### Some basic examples of supervised machine learning

#### Clustering similar images

<p align="center">
  <img width="350" alt="images/clusteringImages.png" src="">
</p>

* Input: Images from a google search for the term "Cookies"
* Output: Similar images sorted into groups

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
* *k-mean clusterings* and *hierarchical clustering* are two common examples of clustering

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
