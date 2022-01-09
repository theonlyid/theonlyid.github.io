---
layout: post
title: "Seizure detection using spectral contrasting"
date: 2018-01-01T15:30:30-04:00
description: "Spectral contrasting for seizure detection and classification"
img: /img/sz.png
---

**Detecting epileptic seizures from EEG recordings**

Neurologists and epileptologists spend a significant amount of their time sifting through EEG recordings that span anywhere between 1 to 9 hours of recoridings, by manually inspecting the data in 10 second increments, looking for markers of a malfunctioning brain. These markers, however, are often small, transient changes in a highly complex and chaotic signal.

I'm interested in developing a method to automatically flag neural events (such as seizures, eye-blinks or sleep) from EEG data. My approach is focussed on overcoming the complex, non-stationary nature of the EEG signal, which poses a difficult challenge for everything from LDA to deep learning.

Specifically, I'm interested in feature mining and feature engineering, to enable a drastic reduction in the size of the feature space of the model.
I've implemented a technique that I've termed 'spectral contrasting', that signficantly reduces the feature space of the input dataset by attempting to overcome the non-stationarity in the data.
This enables us to classify seizure events at a much better accuracy than by using the original timeseries data alone!

A jupyter notebook documenting the method and the analysis is [here](https://github.com/theonlyid/seizuredetection/blob/master/docs/final_notebook.ipynb "Jupyter Notebook").
Spectral contrasting is already enabling subject-independent classification of seizures from single trials, something which is considered incredibly difficult on EEG data.

I've developed a python toolkit for implementing spectral contrasting. The code can found [here](https://github.com/theonlyid/seizuredetection "Github Repo").

The dataset used is a subset of the Temple University EEG Corpus dataset (a freely available dataset), which contains labelled time-series data for normal and seizure activity.
