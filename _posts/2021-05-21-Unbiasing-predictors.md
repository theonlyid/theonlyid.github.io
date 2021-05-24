---
title: "Unbiasing predictors"
date: 2021-05-21T15:30:30-04:00
categories:
  - projects
tags:
  - bias
  - healthcare
  - analytics
---

## Removing biased predictors from datasets - a tutorial

When working with datasets, we are often interested in learning the relationship of a quantity of interest, given some known variables (the predictors). The unknown value could either be the estimated value of a continuous variable, where the process is called regression, or an unknown class to which our sample belong to, called classification. Many tutorials on the internet provide wonderful insights into the many ways of performing regression and classification. The objective of these methods is, in one way or another, to minimize the error in our predictions, with the most commonly used metric being accuracy (of predictions). The game is to push that accuracy score as high as possible. 

However, an often overlooked aspect of training machine learning models is the source and meaning of the underlying features. What is the nature of the information you are using to build your model, and make predictions? Good data science practice requires deeper reflection into the nuts and bolts of the prediction machinery. 

Real-world data is a representation of the complexity and diversity of our society. The data, naturally, also reflects these differences and biases.
Predictions are incredibly valuable in the analysis of healthcare data as well. Does a patient have a particular disease given their blood-work? What's are the chances that a patient will return to the emergency room after being discharged?

We define a bias as a dependence (or deviation) in the predictions of our model based on a feature that we believe should not influence the prediction. For example, the socio-economic of a patient shouldn't affect the quality of healthcare attention they get such as the priority in an emergency waiting room. While it would be very easy to drop that information from our predictive model, the features in the collected data are often co-dependent, and simply ignoring a feature is not good enough. Luckily, there are mathematical tools that enable the removal sensitive information from datasets completely.

However, removing information does lower predictive accuracy, and so making less accurate predictions also be undesirable, specifically when it comes to healthcare. What one would ideally want is to understand the relationship between between accuracy and bias in the given dataset, so as to strike a balance between acceptable levels of both.

I've written an easy to follow [tutorial](https://gist.github.com/theonlyid/c13483f9ab2e07c769ee6b56dab3a1f7) on the evaluation and disentanglement of unwanted features in a dataset for making predictive models, and a work-around on how to strike a balance between bias and accuracy.