---
layout: post
title: Project 5
description: Real-time subject-independent classification of brain states
date: 2021-01-02T15:30:30-04:00
img: /img/sic.jpg
categories:
  - projects
tags:
  - Neurotechnology
  - Machine Learning
---

The ability to classify brain-states online is crucial for any real-time neurorehabilitation application. Although most studies focus on EEG-based paradigms, the results for online, single-trial classifications in such a paradigm are nomimal, given the large non-stationarity of features in EEG data. We turned our attention to fNIRS, another non-inavasive method to record neural activity non-invasively.

We implemented a simple SVM-based classifier to classify left vs right hand movements (clenching the fist) from the NIRS signal. To our surprise, the classifier could also detect "imagined" movements (the subject imagined clenching their fist *without actually moving*). Furthermore, the classifier could generalize across subjects owing to a novel bias-correction that was implemented on a trial-by-trial basis. This means that we could train a classifier on a group of subjects based on their motor execution, and we could classify imagined movements from a new group of subjects! Cross subject, cross-modality classification. 

You can read my paper (the first report of online, multi-channel subject-independent classification of movement intentions!) [here](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0159959).
