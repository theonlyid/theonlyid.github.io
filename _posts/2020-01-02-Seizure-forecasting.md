---
title: "Forecasting epileptic seizures from ongoing EEG recordings"
date: 2019-01-02T15:30:30-04:00
categories:
  - projects
tags:
  - Machine Learning
  - Neuroscience
---

Imagine a patient suffering from epilepsy, who has a seizure interval ranging from days to months. Imagine being them. Imagine having an otherwise normal life, yet constantly fearing that the next minute could have you suddenly on ground succumbing to a tonic-clonic seizure. An incredibly stress-filled life, isn't it?

What if a small medical device, placed just under the skin above your ear could enable a warning system? The activity recorded could be sent to an app on your phone, that processes the data and forecasts the possibility of a seizure in the next minute or two, giving you enough time to secure yourself, or warn a caretaker. What if it could inject a small, imperceptible current to 'interfere' with your seizure?

In this project, I'm interested in developing an algorithm for seizure forecasting from EEG data.

The basic idea is to take data from 20-180s before seizure events and train a variational autoencoder for dimensionality reduction.
I will then train a recurrent neural network to classify normal vs 'pre-seizure' activity.
The desired outcome is a metric with the probability of a seizure occuring in the next 60 seconds, hours or days (imagine weather forecasts with the chances of rain in the coming hours or days).

Like the [seizure detection]({{ site.url}}{{ site.baseurl}}/projects/Seizure-detection/) project, the results of which will in turn be used here, the idea is to engineer the best features to enable reliable forecasting of upcoming seizures.

If you're interested in this project, please shoot me an email using the link in the bio.
