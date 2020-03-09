---
title: "Neural event identification using manifold learning"
date: 2019-02-02T15:30:30-04:00
categories:
  - projects
tags:
  - Machine Learning
  - Neuroscience
---

## Unsupervised approaches towards identifying discrete neural events from continuous time-series data

Most neural signal analysis methods consist of identifying and evaluating changes in the power/amplitude of various frequency bands in either a block design (meaning a stimulus/task is repeated several times, and signal averages are compared across various conditions). However, such methods do not factor in the complex dynamics of neural activity, which consists of overlapping patterns spread across, and interacting over, mulitple temporal and spatial scales. Furthermore, the dominant frequencies of spectral bands identified in traditional analysis methods (such as gamma, alpha, theta, etc) are highly subject-dependent and can vary considerably depending on the health of the brain.

For example, patients that have suffered a traumatic brain injury, or those that suffer from ALS, have very different rhythms that do not fall within the traditional spectral windows commonly used for such analyses. Thus arises the need for a purely data-driven approach towards identifying neural events that places no assumptions on the type, number, or duration of events, or where the events should be localized in the frequency domain.

I am currently developing and testing unsupervised approaches that identify discrete events from continuous neural recordings (both EEG and intracortical recordings from both humans and primates). The discretization of continuous data into events will enable the application of models such as HMMs for forecasting / predicting certain events such as epileptic seizures. Or, in patients with traumatic brain injury that are comatose, they will help identify events that might predict the recovery rate of the individual, as well as extent of injury to neural tissue. Lastly, they could enable the tracking of treatment efficacy, for example, the response of the patient to different drugs.

Such tools are critical for enabling deeper insights into the changes that occur during neurological diseases, for tracking progress during recovery and rehabilitation, and finally for identifying predictors for specific outcomes.

You can see a glimpse of ongoing work [here](https://github.com/theonlyid/event_detection/blob/master/Event%20detection.ipynb "Jupyter notebook").
