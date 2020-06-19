
## Concepts in Machine Learning Class 4: Exploratory Data Analysis, Experimental Design, and Ethics in Machine Learning

Welcome to class 4 of Concepts in Machine Learning!

By the end of this class you should be able to:

* Describe what exploratory data analysis is and why it's important.
* Understand the ethical implications of machine learning.

### Review!
* Review how machine learning works, trianing testing, information about datasets, features

### What is exploratory data analysis?

### EDA is a detour

* not very structured
* exploration 
* iterative

### An EDA checklist

1. What question(s) are you trying to solve (or prove wrong)?
2. What kind of data do you have and how do you treat different types?
3. What’s missing from the data and how do you deal with it?
4. Where are the outliers and why should you care about them?
5. How can you add, change or remove features to get more out of your data?


### Let's practice!

We will use a synthetic dataset of cardiovascular disease risk data from Ted Laderast at OHSU.

View the related course materials here: https://github.com/laderast/cvdNight1 and https://github.com/laderast/cvdNight2

Explore the dataset here: https://tladeras.shinyapps.io/cvdnight1/

More information about the generation of this dataset is available here: https://www.biorxiv.org/content/early/2017/12/12/232611

#### 1. What question(s) are you trying to solve?

Start simple - with one problem and work out from there as needed.

In this dataset a problem we could solve is - can we predict if someone will get cvd based on these attributes.

### 2. What kind of data do you have?

Investigate the data types in the data set
 * go colummn by column and to id numerical, categorical, not sure
 * Remove unnecessary columns (ex ID column)


 * data dictionaries
 * consulting a subject matter expert
 * google!

### 3. What's missing from your data?

There are some common ways to denote empty cells. It's important to understand what an empty cell means in your data set (i.e. is NA different than "")

Show visual check of missing data

Options with missing data:
 * remove the column
  * ml algorithms like as much data as possible so this might not be ideal for smaller datasets
 * impute
   * i.e. fill in missing age values with avg age.
   * talk about pros and cons of removing vs imputing
   
### 4. Outliars and how to handle them
 
### 5. How to add, change, and remove features to get the most out of your data.

### Ethics in machine learning

* what do we mean by ethics?
* general ethical concerns of machine learning algorithms

* Replicating biases
 * ML algorithms learn from datasets but what happens when biases are baked into the dataset?
 * Need a good example here
* Missing data
* Intent behind design
 * Bellmont Report
 * Basically - even if we can do it SHOULD we
 * Examples: ml to identify gay people/"criminals"/etc based on facial features. Getting close to eugenics here.
* Take into account possible malevolent uses, interpretations
 * Facial recognition

### Review

### Extra materials

If you have some coding experience:
* [Practice setting up your first machine learning model in Python with Kaggle](https://www.kaggle.com/learn/intro-to-machine-learning)
* [Practice setting up a machine learning model in R with TidyModels](https://www.tidymodels.org/start/models/)

### Closing

Upcoming R and Python machine learning courses
