---
title: "Seizure detection"
date: 2019-01-01T15:30:30-04:00
categories:
  - blog
tags:
  - Machine Learning
  - Neuroscience
  - Ongoing
---

## Detecting epileptic seizures from EEG recordings

In this project, I'm interested in detecting seizures from EEG recordings.
Specifically, I'm interested in feature mining and feature engineering, to enable a drastic reduction in the size of the feature space.
I've implemented a technique that I termed 'spectral contrasting', that signficantly reduces the feature space of the input dataset.
This enables us to classify seizure events at a much better accuracy than by using the original timeseries data alone.

A jupyter notebook documenting the analysis is [here](https://github.com/theonlyid/seizuredetection/docs/final_notebook.ipynb "Jupyter Notebook").

I've developed a python toolkit for implementing spectral contrasting. The code can found [here](https://github.com/theonlyid/seizuredetection "Github Repo").

The dataset used is a subset of the Temple University EEG Corpus dataset, which contains labelled time-series data for normal and seizure activity.

