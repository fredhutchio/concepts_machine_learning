## Concepts in Machine Learning Class 2: Supervised Learning

### Objectives

Welcome to class 2 of Concepts in Machine Learning!

In the last class, we touched on all of the main concepts that we will be covering in this course including supervised and unsupervised learning, exploratory data analysis, and ethics.

By the end of this class you should be able to:

* Define and understand the limitations of supervised learning
* Differentiate between regression and classification
* Assess whether or not supervised learning is an appropriate tool for a question
* Understand basic applications of supervised learning (linear regression, logistic regression)
* Create supervised learning problem statements

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

ex: we are trying to predict whether or not someone will get the flu this flu season.

reality/truth: a persons health history, location, occupation, diet, socialization habits, among many other things will play into if someone gets the flu or not. 

dataset: when creating the dataset that will be used to make our prediction we have to understand that we will never capture the whole truth. We will capture as much of the truth as we can by collecting data on various features that we believe are related to the problem we are trying to solve. 

features/variables: These are the measurable data that make up our dataset. Some features collected might be useless while others might carry a substantial amount of weight in making our prediction.

inputs: features that we will use to make our prediction

output: a prediction or inference about the data.

### An overview of supervised learning

The goal of supervised machine learning is to fit a model that relates response variables to predictors and can accurately predict the response for future observations of predictor variables. We will cover supervised learning more in depth in class 2 of this series.

Supervised learning is one of the most commonly used forms of machine learning and it's generally easier to implement and interpret than unsupervised learning alogrithms. 

A hallmark of supervised learning algorithms is that they work in two steps: training and testing. This requires training the algorithm on example datasets with inputs that are annotated (or labled) with the correct response. Once training is complete the algorithm will be tested on a seperate labled dataset and it's performance is evaluated.

Ideally an the algorithm will be specific enough to accurately predict the response variable, but generalizable so that it works with new datasets.

There are two subclasses of supervised learning:
1. Regression: predicting a numeric
2. Classification: predicting a category

### Training a machine starts with data collection

All supervised learning algorithms require large training and testing datasets. 

Creating labeled datasets is one of the most time intensive pieces of supervised machine learning. Sometimes this can be done automatically by merging datasets or scraping the internet, but many times the labeling must be done manually. Automatic labelling is quicker and cheaper, but generally messier and less accurate. Manual data collection is expensive and time consuming, but with fewer errors. You likely have been involved in some form of labeling yourself! It's not uncommon for companies to use their own customers for free labeling.

We will take a more in depth look at what makes a good dataset in class 4 when we discuss exploratory data analysis and ethics.

**Insert Captcha comic**

Data collection and labeling is an intensive process and it can be incredibly difficult to create a comprehensive, 'good', dataset. In fact, while some companies might release the source code for their machine learning algorithms, the underlying data that they use is generally kept private. Since the underlying data is so important to the results and interpretation of machine learing algorithms.

### How do you train a machine?

Training is the hallmark of a supervised learning algorithm because this is the step where a 'supervisor' essentially gives the machine the answers. A machine is trained by feeding it large labeled datasets (aka training or validation sets) like we just learned about above. The algorithm works by finding patterns in the dataset and building it's own set of rules to determine what the outcome might be based on new inputs. When we say large we mean that these training sets should have at a minimum tens of thousands of rows.

### How do you test a machine?

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
