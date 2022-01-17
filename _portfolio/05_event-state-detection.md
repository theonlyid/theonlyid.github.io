---
layout: post
title: "Project 1"
description: "Event-state detection in neural timeseries"
date: 2010-01-01T15:30:30-04:00
img: /img/event-state.png
---

**Event-state detection in neural timeseries**

Traditionally, the anlaysis of broadband activity recorded through electrophsyiology (such as EEG, ECoG, LFP, etc) is anlysed by filtering and decomposing the signal into various bands such as the theta, delta, gamma, etc. The instantaneous or average power in these bands is then meaured and used as a feature for further analysis.

A fundamental problem with this analysis is the arbitrary nature in the definition of the bands, and the inability to account for differences in different subjects. Furthermore, stable band-limits are very hard to find in healthy subjects let alone in unhealthy subjects that can have a completely different power-spectrum altoghether. This would render all the insight built from healthy individuals all bus useless for unhealthy  subjects that are either comatose, or have experienced traumatic brain injury. 

There's need to relax these strict analytical parameters and learn them from the subject's data themselves. This would enable more personalized assessments and analysis. 

I have recenlty demonstrated a method that enables discretization of complex signals across multiple scales. I've demonstrated how it works on open data in a jupyter notebook [tutorial](/tutorials/event-detection/).

The algorithm defines an event as a specific distribution over the power spectrum. It identifies various events from the data, based on the parameters of the STFT. From there it identifies states by defining a state to be a distribution over the events.

I've used a segment of iEEG signals from a patient suffering from epilepsy, where the first and last 180s of the recording represent background activity, and the rest represent a seizure.

**The results in brief:**

1. Using a purely unsupervised approach, I was able to recover the original labels in the data (background vs seizure) as states.

2. Since each state is a distribution over different events, we could use the events to refine the otherwise noisy labels.

**By cleaning lables using this algorithm we reduced the seizure classification error by ~93%**


**Results at a glimpse**

| Labels | bal Acc | F1 |
| :----- | :-------: |  -: |
| Original | 0.905 | 0.81 |
| Improved* | 0.997 | 0.94 |

<br>
Please checkout my [notebook](/tutorials/event-detection/) for more information. 