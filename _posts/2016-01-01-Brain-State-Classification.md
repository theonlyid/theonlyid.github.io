---
title: "Brain-state classification"
date: 2015-01-01T15:30:30-04:00
categories:
  - project
tags:
  - Neurotechnology
  - Machine Learning
---

## Real-time subject-independent classification of brain states

The ability to classify brain-states online is crucial for any real-time neurorehabilitation applications. Although most studies focus on EEG-based paradigms, the results for online, single-trial classifications in such a paradigm are nomimal. we turned our attention to fNIRS, another non-inavasive method to record neural activity non-invasively.

We implemented a simple SVM-based classifier to classify left vs right hand movements (clenching the fist) from the NIRS signal. To our surprise, the classifier could also detect "imagined" movements (the subject imagined clenching their fist without actually moving). Furthermore, the classifier could generalize across subjects owing to a novel bias-correction that was implemented on a trial-by-trial basis.

You can read my paper (the first report of online, multi-channel subject-independent classification of movement intentions!) [here](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0159959).