# Concepts in Machine Learning Course

This course consists of four one hour classes and covers the basic concepts of classical machine learning (supervised and unsupervised methods). This course is meant to be an introduction and overview to machine learning and does not include any code or statistics. 

**There are no prerequisites to this course.**

**This course is a prerequisite to Machine Learning in Python and R.**

By the end of this course you should be able to:

* Identify questions that are and are not appropriate applications of machine learning
* Understand the importance of exploratory data analysis, experimental design, and data collection to applying machine learning algorithms
* Recognize the four main paradigms of machine learning
* Differentiate between supervised and unsupervised ML methods and applications
* Recognize and have a basic understanding of common approaches to supervised (regression, classification) and unsupervised (clustering, dimensionality reduction) machine learning.
* Identify biology research areas where machine learning can be applied.

---

## Concepts in Machine Learning Class 1: Introduction to Machine Learning

### Objectives

Welcome to Concepts in Machine Learning from fredhutch.io! This course is designed for researchers who are interested in machine learning, and assumes no prior programming or statistics experience. There are no prerequisites for this course.

This course will introduce you to machine learning and give a broad overview of supervised and unsupervised machine learning. The goal of this course is to provide some conceptual background for our Machine Learning in R and Python series. Further, researchers who complete this course should have an understanding of how machine learning can be applied in biology research.

By the end of this class you should be able to:

* Define machine learning
* Recognize the four paradigms of machine learning
* Understand basic terminology like algorithm, inputs, outputs, supervised, unsupervised
* Differentiate between unsupervised and supervised ml

### What **isn't** machine learning?

Buzzwords like ‘machine learning’, ‘deep learning’, and ‘artificial intelligence’ get thrown around quite a bit these days. Sometimes they seemed to be used as synonyms, others as distinct entities. It can be hard to determine exactly what these big, vague terms mean to the layperson. So let’s start with what *isn’t* machine learning.

**Machine learning is NOT:**

* Magic
* A secret sauce
* Seasoning to be sprinkled liberally over a mundane application
* A substitute for a good understanding of your problem

### What **is** machine learning?

Recent advances in compute power, cloud technologies, data collection and data generation have thrust machine learning into the mainstream. Increasingly machine learning is looked to as a tool to solve Big Complex Problems like cancer. Often though the term machine learning is used as a sort of black box, but what actually is machine learning?

Let’s orient ourselves to the terms I mentioned in the previous slides that you may be familiar with (ML, AI, Deep learning) to get a sense of how things fit together.

* AI is a term that embodies anything that enables computers to act more like humans.
  * Turing test
  * “I talk to siri and she answers”
  * This is a whole field of knowledge like ‘biology’ or ‘chemistry’

* Machine learning is a subset of AI
  * Focused on the extraction of patterns from large datasets

* Deep learning is a collections of similar machine learning methods.
  * A group of similar techniques that use neural networks
  * There are other groups of related methods that are subsets of machine learning as a whole
    * support vector machine
    * decision trees

### Machine learning defined

Let's look at how machine learning is defined.

**Wikipedia:** Machine learning (ML) is the study of computer algorithms that improve automatically through experience. It is seen as a subset of artificial intelligence. Machine learning algorithms build a mathematical model based on sample data, known as "training data", in order to make predictions or decisions without being explicitly programmed to do so.

**Merriam Webster:** the process by which a computer is able to improve its own performance (as in analyzing image files) by continuously incorporating new data into an existing statistical model.

**[Nature Genetics Review:](https://www.nature.com/articles/nrg3920)** The field of machine learning includes the development and application of computer algorithms that improve with experience.

**Common themes**

* A kind of algorithm
  * A finite sequence of well-defined, computer-implementable instructions, typically to solve a class of problems or to perform a computation (Wikipedia)
  * Essentially a protocol for a computer
* Incorporates data into a statistical model
* Improves with experience without human intervention


### Machine learning as code

When we think of machine learning and how it applies to code we can consider machine learning to be a specific way of programming computers.

* Most programming isn’t machine learning - it’s procedural
    * Build out a set of rules that a human codes. This set of rules is called an algorithm. This ruleset remains static unless the coder intervenes and specifies more rules.
* In ML the algorithm is also designed and coded by a human. However, this kind of algorithm is able to learn from the data about specific parameters that will shape a statistical model for making predictions and inferences. The coder doesn’t necessarily know or control these parameters - the machine does.

**Machine learning is an algorithm (or set of rules) that self adjusts based on the large datasets that it is given**

### When to use machine learning

Just like any other statistical method there are specific situations where applying machine learning is appropriate. Just as important as the algorithm itself is a solid understanding of experimental design, domain expertise in the problem area youre trying to solve, and an understanding of data governance and ethics.

You cannot code the rules: 
* Tasks that cannot be solved using a simple, rule-based solution. 
* When rules depend on too many factors and many of these rules overlap or need to be tuned very finely, it soon becomes difficult for a human to accurately code the rules. You can use ML to effectively solve this problem.
* This is true for drawing conclusions about highly dimensional data

You cannot scale:
* You might be able to manually recognize a few hundred emails and decide whether they are spam or not. However, this task becomes tedious for millions of emails. ML solutions are effective at handling large-scale problems.

#### Challenge!

1. Write an algorithm/protocol/ruleset for making a PBJ sandwich
2. Write an algorithm/protocol/ruleset for determining if an email is spam

### Biology is suited for machine learning

In the past data generation had been a bottleneck in biology research but this is no longer true. Biology research is generating huge amounts of complex and increasingly integrated data!

Biology is suited for machine learning applications:
* You cannot code the rules
    * Biological systems are incredibly complex with many inputs leading to complex phenotypes. 
    * Example: if you want to determine whether or not a patient is likely to get cancer we’d need to take many datasets into account (demographic data, health/nutrition data, family history, genetic data, etc). We cannot determine and code the rules for a computer to calculate if a person is likely to get cancer or not.

* You cannot scale
    * Our human brains cannot make sense of these huge integrated datasets or even just one of them.
    * Example: a human looking at a series of bases would take years to make sense of the human genome. A computer can find patterns in our genome with relative ease.

### How is machine learning applied?

Machine learning applications are all around us! Every time Spotify serves up a customized playlist or radio station based on the music that you like, Facebook loads your newsfeed, your phone autocorrects you, or you interact with a voice assitant like Siri, you are interacting with machine learning algorithms.

Every-day applications:
* Search engines
* Recommendation systems (Yelp, Netflix, Spotify)
* Voice assistants
* Social media feeds
* Text prediction

#### Machine learning techniques are becoming increasingly important to biological research.

Researchers are developing algorithms that use machine learning to classify histopathological images, visualize and find clusters within single cell datasets, and much more.

Biology specific applications:
* Automated gating for single cell mass and flow cytometry
* Visualization and clustering of single-cell RNA sequencing data
* Classification of histopathological images of breast tissue to identify malignant tumors

Work happening here at Fred Hutch
Gottardo lab - automatic gating for flow cytometry data (FAUST)
Emily Silgards Data Science group - use natural language processing to extract information from electronic medical records
Michael Zager’s group - single cell visualization and clustering using methods like tSNE

### How do these machine learning applications work?

There are different types of machine learning and each have their own specific applications and requirements.

Four major paradigms in machine learning:
* **Supervised**
* **Unsupervised**
* Semi-supervised
* Reinforcement learning

The focus of this course will be on supervised and unsupervised learning, but it’s good to be aware that these are not the only types of ml.

### Anatomy of a machine learning problem
discuss inputs and outputs

dataset, features - really break down how a dataset doesn't capture the entirety of The Truth only the features we have collected.

### An overview of supervised learning
emphasize - labled data, concrete interpretations, 2 steps, 2 subclasses, used to make predictions

#### Example supervised learning questions

### The two steps of supervised learning: training and testing

### An overview of unsupervised learning

#### Example unsupervised learning questions

### One step to unsupervised learning: fitting

### Review!

### Next week: supervised machine learning

### Reading material

---

## Concepts in Machine Learning Class 2: Supervised Learning

### Objectives

Welcome to class 2 of Concepts in Machine Learning!

By the end of this class you should be able to:

* Define supervised learning
* Differentiate between regression and classification
* Assess whether or not supervised learning is an appropriate tool for a question
* Understand basic applications of supervised learning (linear regression, logistic regression)
* Understand what bias-variance trade off and overfitting are

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

