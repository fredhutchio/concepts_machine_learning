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

**Example: we are trying to cluster patients to find if there are novel subgroupings within the dataset**

Here we are looking at the exact same example dataset as last class. You'll notice that our intended outcome is slightly different than when we were using the dataset for supervised learning. Instead of predicting whether or not a patient is likely to be diagnosed with cardiovascular disease we want to explore the data for underlying patterns.

| patient_Id    | age   | htn | treat | smoking | race     | t2d | gender | numAge | bmi | tchol| sbp | cvd |
| ------------- | ----- | --- | ----- | ------- | -------- | --- | ------ | ------ | --- | ---- | --- | --- |
| HHUID00076230 | 20-40 | Y   | Y     | N       | Asian/PI | N   | M      | 29     | 23  | 189  | 170 | N   |
| HHUID00547835 | 70-90 | N   | Y     | N       | White    | Y   | M      | 72     | 35  | 178  | 118 | N   |

**Reality/truth:** The factors that lead to someone being diagnosed with cardiovascular disease are complex and difficult to detangle. Because of this, there might be subgroups of patients with similar features that might be interesting to study. For example, we might find a cluster of patients who are young, don't smoke, and have relatively healthy cholestorol and blood pressure that are all diagnosed with cardiovascular disease. 

**Dataset:** When creating the dataset that will be used to make our predictions we will never capture the whole truth. We will capture as much of the truth as we can by collecting data on various features that we believe are related to the problem we are trying to solve. Many underlying factors that lead to the cardiovascular disease may be unknown or we might not be able to measure them or capture them in our dataset. Think of the hypothetical cluster of young, relatively healthy, non-smokers from above. Perhaps there is a variable that we are missing that would illuminate us as to why these patients were diagnosed with cardiovascular disease?

**Features/variables:** These are the measurable data that make up our dataset. Some features collected might be useless while others might carry a substantial amount of weight in making the prediction. Since this is a training set one of the variables included is the label that we are trying to predict (`cvd`).

**Inputs:** Features that we have collected and will use to cluster our datapoints. In this dataset our inputs would be all of the columns except `patient_Id` since it is the feature that we will be clustering on.

**Output:** Unlike in our supervised learning example `cvd` is no longer considered an output because unsupervised learning algorithms do not aim to predict a specific target variable. The output for an unsupervised learning algorithm is generally a visualization of clusters or a new representation of datapoints.

#### New term!

**Object:** An object is the variable we are trying to cluster on. This is the variable that each data point will represent. In our example of clustering patients, each data point in our cluster would represent a unique patient identifier.

### What is unsupervised machine learning?

<p align="center">
  <img width="600" alt="" src="images/unsupervised.png">
</p>

The goal of unsupervised learning is to detect the underlying structure and patterns in a dataset with no pre-existing labels. The lack of pre-existing labels means that the algorithm is able to work with minimal human supervision which is why we call these methods 'unsupervised'.

Unlike with supervised learning, unsupervised learning methods do not require annotated training data to work. With no training or testing required there is only one step, fitting.

There are two kinds of supervised learning that we will talk about today:
1. Unsupervised transformations: Create a new representation of a complex dataset that is easier to understand than the original.
2. Clustering: Partition data into distinct groups of similar objects.

### Some basic examples of supervised machine learning

#### Clustering similar images

<p align="center">
  <img width="600" alt="" src="images/clusteringImages.png">
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

You might have noticed that the second exammple is *almost* identical to last classes.

> #### Identifying handwritten letters
>
> * Input: Scanned, handwritten letters
> * Output: The actual character
> * Dataset: Need thousands of handwritten letters and to annotate the correct letter for each one

1. What is the difference between supervised classification and unsupervised clustering of handwritten letters? How might the output look different?

### Challenges of unsupervised machine learning

The main challenge of unsupervised learning is that it can be difficult to tell if the algorithm learned something useful. Since there is no labeled information to train on we cannot tell the algorithm what we're trying to predict and we have no clue about what the right output should look like. Because of this, it can be hard to tell if an algorithm "did well". Unsupervised learning algorithm outputs must be inspected manually to gain any information.

<p align="center">
  <img width="600" alt="" src="images/tsne.jpg">
</p>

Consider the above output from a dimensionality reduction method called t-Distributed Stochastic Neighbor Embedding (t-SNE). Here we are automatically clustering cells based on their RNA-sequencing results. You'll notice that while each cluster is uniquely colored we are given no information about why they are clustered this way other than the machine picked up some underlying pattern in their RNA-sequencing results. It is up to the investigator to further interrogate these clusters to figure out if there is a meaningful difference between these clusters.

### When to use unsupervised learning

Due to the challenges we discussed above, unsupervised learning is generally used in an exploratory step of analysis. 

Common applications of unsupervised learning:
* When you want to learn more about the underlying structures in the data.
* As a preprocessing step for supervised learning algorithms.
  * Learning a new representation of the data can highlight outliars, improve accuracy downstream, and reduce the memory/time required for further analysis. 

### What is clustering?

* Clustering is the organization of unlabled data into groups (clusters) based on how similar they are. 
* Clustering is a task that can be accomplished by various algorithms that differ in how they understand what constitutes a cluster and how they find clusters.
* *centroid based clustering* and *hierarchical clustering* are two different types of clustering.

#### Hard vs soft clustering

### Connectivity-based clustering (heirarchical)

The hallmark of heirarchical clustering is that these algorithms do not provide a single partitioning of the dataset. Instead, they provide a heirarchy of clusters that merge with eachother at certain distances. Often heirarchical clustering is visualized via a dendogram like the one below.

<p align="center">
  <img width="600" alt="" src="images/dendogram.png">
</p>

These algorithms connect "objects" to form "clusters" based on their [distance](https://en.wikipedia.org/wiki/Statistical_distance#:~:text=In%20statistics%2C%20probability%20theory%2C%20and,or%20a%20wider%20sample%20of). The y-axis marks the distance at which the clusters merge, while the objects are placed along the x-axis such that the clusters don't mix.

#### Making sense of dendograms

* The dendrogram shows data points as points on the bottom (numbered from 0 to 11). 
* A tree is plotted with these points (representing single-point clusters) as the leaves, and a new node parent is added for each two clusters that are joined.
* Reading from bottom to top, the data points 1 and 4 are joined first. Next, points 6 and 9 are joined into a cluster, and so on.
  * Points that are joined first are the most closely related.

### Centroid-based clustering



### The curse of dimensionality

### Dimensionality reduction

### Principle componant analysis (PCA)

### Evaluation and interpretation of unsupervised learning methods

### Review!

### Next Class

### Reading

https://idyll.pub/post/dimensionality-reduction-293e465c2a3443e8941b016d/
