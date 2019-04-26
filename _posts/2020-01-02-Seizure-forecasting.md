---
title: "Seizure forecasting"
date: 2019-01-02T15:30:30-04:00
categories:
  - blog
tags:
  - Machine Learning
  - Neuroscience
  - Ongoing
---

## Forecasting epileptic seizures from ongoing EEG recordings

In this project, I'm interested in forecasting seizures from ongoing EEG activity.

The basic idea is to take data from 20-180s before seizure events and train a variational autoencoder for dimensionality reduction.
I will then train a recurrent neural network to classify normal vs 'pre-seizure' activity. 
The desired outcome is a metric with chances of a seizure occuring in the next 60 seconds.

This system can be integrated with wireless EEG recording systems, or implanted electronics, that are continuously sampling neural activity, and act as a warning system.

In the most basic application, I am integrating this system with the Muse headset. 

If you're interested in this project, please shoot me an email using the link in the bio.