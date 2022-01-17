---
layout: post
title: "Project 1"
description: "Event-state detection in neural timeseries"
date: 2010-01-01T15:30:30-04:00
img: /img/event-state.png
---

**Event-state detection in neural timeseries**

Traditionally, the anlaysis of broadband activity recorded through electrophysiology (such as EEG, ECoG, LFP, etc) is anlyzed by filtering and decomposing the signal into various bands such as the theta, delta, gamma, etc. The instantaneous or average power in these bands is then measured and used as a feature for further analysis.

A fundamental problem with this analysis is the heuristic nature of the definition of the bands, combined with a one-size-fits-all approach and the inability to account for differences in subjects. Furthermore, consitent band-limits are very hard to find across healthy subjects, let alone in unhealthy individuals, who may have a completely different EEG power-spectrum altoghether. This would render all the insight built from healthy individuals useless for unhealthy subjects that are either comatose or have experienced traumatic brain injury. 

There is a need to relax these strict analytical parameters and learn them from the subject's data. This would enable more personalized assessments and analysis. 

I recenlty developed a method that enables discretization of complex signals across multiple timescales. I have demonstrated how it works on an openly availabe dataset in a jupyter notebook [tutorial](/tutorials/event-detection/).

The algorithm defines neural events as a specific distribution over the power spectrum. It identifies various events from the data, by clustering a decomposition of the STFT. From there it identifies states by defining a state as specific distribution over the all events.

In the example, I have analyzed a segment of iEEG signals from a patient suffering from epilepsy, where the first and last 180s of the recording represent background activity, and the rest represent a seizure.

**The results in brief:**

1. Using a purely unsupervised approach, I was able to recover the original labels in the dataset (background vs seizure).

2. Since each state is a distribution over different events, we could use the events to clean the  noisy labels, acheiving very high classification accuracies.

**By cleaning lables using this algorithm we reduced the seizure classification error by ~93%**


**Results at a glimpse**

| Labels | bal Acc | F1 |
| :----- | :-------: |  -: |
| Original | 0.905 | 0.81 |
| Improved* | 0.997 | 0.94 |

<br>
Please checkout my [notebook](/tutorials/event-detection/) for more information. 