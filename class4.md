
## Concepts in Machine Learning Class 4: Exploratory Data Analysis, Experimental Design, and Ethics in Machine Learning

Welcome to class 4 of Concepts in Machine Learning!

Last class we covered unsupervised learning methods including k-means clustering and principle component analysis. Today we will cover some common steps to exploratory data analysis and why it's important. We'll also touch on ethics in machine learning.

By the end of this class you should be able to:

* Describe what exploratory data analysis is and why it's important.
* Understand the ethical implications of machine learning.

### What is exploratory data analysis?

When starting a machine learning project it is important to remember that the data that you're using is as important as the model you choose. Making meaning of highly dimensional data is complicated and error-prone. To have a solid start for a machine learning project, you need to analyze the data up front. This process is called exploratory data analysis (EDA). The goal of EDA is to describe the data through statistical analysis and visualization that highlights important features of the data for further analysis. It's important to gain a deep understanding of:
* The properties of the data (i.e. schema and statistical properties)
* The quality of the data (i.e. missing values and incosistant data types)
* The predictive power of the data (i.e. correlations between features and the target)

There are many different approaches to exploratory data analysis. EDA is often unstructured and explorative of the data. It is generally easiest to work iteratively, starting with one problem and working out from there.

### An EDA checklist

1. What question(s) are you trying to solve (or prove wrong)?
2. What kind of data do you have and how do you treat different types?
3. What’s missing from the data and how do you deal with it?
4. Where are the outliers and why should you care about them?
5. How can you add, change or remove features to get more out of your data?

### Let's practice!

Remember the OHSU dataset we looked at earlier in this course:

| patient_Id    | age   | htn | treat | smoking | race     | t2d | gender | numAge | bmi | tchol| sbp | cvd |
| ------------- | ----- | --- | ----- | ------- | -------- | --- | ------ | ------ | --- | ---- | --- | --- |
| HHUID00076230 | 20-40 | Y   | Y     | N       | Asian/PI | N   | M      | 29     | 23  | 189  | 170 | N   |
| HHUID00547835 | 70-90 | N   | Y     | N       | White    | Y   | M      | 72     | 35  | 178  | 118 | N   |

#### 1. What question(s) are you trying to solve?

Start simple - with one problem and work out from there and add complexity as needed.

In this dataset a problem we could solve is - can we predict if someone will get cardiovascular disease based on these attributes?

#### 2. What kind of data do you have?

Investigate the data types in the data set.
 * go colummn by column and label as "ID", "numerical", "categorical", and "not sure"
 * Remove unnecessary columns

Make sure you understand what each column means. If you're lucky your dataset will come with a data dictionary which will include a description of each column. Most of the times though, you have to do a little research.

### 3. What's missing from your data?

There are some common ways to denote empty cells. It's important to understand what an empty cell means in your data set (i.e. is NA different than "")

Show visual check of missing data

Options with missing data:
 * remove the column
  * ml algorithms like as much data as possible so this might not be ideal for smaller datasets
 * impute
   * i.e. fill in missing age values with avg age.
   * talk about pros and cons of removing vs imputing

#### Challenge - explore a dataset

Let's practice some initial explorations of a dataset.

1. Do you immediately know what all of the column headers from the OHSU dataset mean? If not look them up!

<p align="center">
  <img src="http://letmegooglethat.com/?q=what+does+t2d+mean+cardiovascular+disease" width="250" />
</p>


2. Explore the cardiovascular dataset using this shiny application: https://tladeras.shinyapps.io/cvdnight1/


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

https://medium.com/@CoalitionForCriticalTechnology/abolish-the-techtoprisonpipeline-9b5b14366b16

### Closing

Upcoming R and Python machine learning courses
