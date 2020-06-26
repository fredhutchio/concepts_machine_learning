## Solutions for Class 3

### What is the difference between supervised classification and unsupervised clustering of handwritten letters? How might the output look different?

Clustering is somehwat similar to classification in that each item gets a label. The difference is that with unsupervised learning there is no *a priori* truth so the labels essentially have no real meaning. Let's think about this in the context of handwritten letters. It might be that cluster 2 found by the unsupervised algorithm contains different representations of the letter `L` in cursive. You can only know this after manually inspecting the cluster and the number '2' is arbitrary. The only information that this unsupervised algorithm is giving is that all the letters labeled as '2' are similar in some way.
