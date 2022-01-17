---
layout: post
title: "Project 2"
description: "Using PPG for patient health monintoring"
date: 2010-01-01T15:30:30-04:00
img: /img/in3.png
---

**Using PPGs for patient health monintoring**

The PPG signal is signal rich in information that can be used to infer many physiological parameters such as pulse-rate and blood-oxygenation.
This is how it has traditionally been used in hospitals. However, it can provide to more interesting physiological parameters, specially in the ICU, and more so durin brain trauma:

1. It can be used to infer blood pressure (wiith a little bit of signal processing)

2. When measured from the scalp, it is a very reliably proxy of brain activity, and based on my earlier work, can be used to tease apart spiking from low frequency activity.

**How is that relevant?**

1. Changes in blood pressure can be used to infer the depth of anesthesia without the need for an extra device that is attached to arm. The BP measurements are returned at the same rate as pulse, so keeping track of faster changes is made way easier.

2. The arousal state of a patient can be determined by the burst-suppression patterns in the EEG. Since fNIRS is a great proxy for brain activity, and is much more robust to movements and purutrbations, it makes a great canditate for monitoring patient brain function in the ICU.

<b>
Discretizing complex dynamics
</b>

The dynamics of the two signals can be fed into an event-state detection algorithm (such as the one described in [Project 1](/portfolio/05_event-state-detection)) that can divide the timeseries into different events and states, which can be tracked over time, and used as variables to predict the outcome of different treatments or interventions.

This is a project that is very close to my heart, and I am eagery waiting for an opportunity to validate and implement a working system in the ICU.
