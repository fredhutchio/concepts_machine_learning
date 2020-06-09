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

## Concepts in Machine Learning Class 1: Introduction to Machine Learning

### Objectives

Welcome to Concepts in Machine Learning from fredhutch.io! This course is designed for researchers who are interested in machine learning, and assumes no prior programming or statistics experience. There are no prerequisites for this course.

This course will introduce you to machine learning and give a broad overview of supervised and unsupervised machine learning. The goal of this course is to provide some conceptual background for our Machine Learning in R and Python series. Further, researchers who complete this course should have an understanding of how machine learning can be applied in biology research.

By the end of this course you should be able to:

* Identify questions that are and are not appropriate applications of machine learning
* Understand the importance of exploratory data analysis, experimental design, and data collection to applying machine learning algorithms
* Recognize the four main paradigms of machine learning
* Differentiate between supervised and unsupervised ML methods and applications
* Recognize and have a basic understanding of common approaches to supervised (regression, classification) and unsupervised (clustering, dimensionality reduction) machine learning.

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
* Incorporates data into a statistical model
* Improves with experience without human intervention

### Machine learning as code

When we think of machine learning and how it applies to code we can consider machine learning to be a specific way of programming computers.

* Most programming isn’t machine learning - it’s procedural
    * Build out a set of rules that a human codes. This set of rules is called an algorithm. This ruleset remains static unless the coder intervenes and specifies more rules.
* In ML the algorithm is also designed and coded by a human. However, this kind of algorithm is able to learn from the data about specific parameters that will shape a statistical model for making predictions and inferences. The coder doesn’t necessarily know or control these parameters - the machine does.

**Machine learning is an algorithm (or set of rules) that self adjusts based on the large datasets that it is given**

### When to use machine learning

Just like any other statistical method there are specific situations where applying machine learning is appropriate. 

You cannot code the rules: 
* Tasks that cannot be solved using a simple, rule-based solution. 
* When rules depend on too many factors and many of these rules overlap or need to be tuned very finely, it soon becomes difficult for a human to accurately code the rules. You can use ML to effectively solve this problem.
* This is true for drawing conclusions about highly dimensional data

You cannot scale:
* You might be able to manually recognize a few hundred emails and decide whether they are spam or not. However, this task becomes tedious for millions of emails. ML solutions are effective at handling large-scale problems.

### Biology is suited for machine learning

In the past data generation had been a bottleneck in biology research but this is no longer true. Biology research is generating huge amounts of complex and increasingly integrated data!

Biology is suited for machine learning applications:
* You cannot code the rules
    * Biological systems are incredibly complex with many inputs leading to complex phenotypes. 
    * Example: if you want to determine whether or not a patient is likely to get cancer we’d need to take many datasets into account (demographic data, health/nutrition data, family history, genetic data, etc). We cannot determine and code the rules for a computer to calculate if a person is likely to get cancer or not.

* You cannot scale
    * Our human brains cannot make sense of these huge integrated datasets or even just one of them.
    * Example: a human looking at a series of bases would take years to make sense of the human genome. A computer can find patterns in our genome with relative ease.

