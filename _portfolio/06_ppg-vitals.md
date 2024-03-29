---
layout: post
title: "Project 2"
description: "Using PPG for patient health monitoring"
date: 2010-01-01T15:30:30-04:00
img: /img/in3.png
---

**Using PPGs for patient health monitoring**

The PPG signal is rich in information that can be used to infer many physiological parameters such as pulse-rate and blood-oxygenation.
This is how it has traditionally been used in hospitals and healthcare settings. However, it can also provide more interesting physiological parameters, specially in the ICU, enabling a long-term assessment and tracking of patient health, arousal and discomfort.

Two simple applications are:

1. It can be used to infer blood pressure (with a little bit of signal processing)

2. When measured from the scalp, it is a very reliably proxy of brain activity, and based on my earlier work, can be used to tease apart spiking from low frequency activity.

**How is that relevant?**

1. Changes in blood pressure can be used to infer the depth of anesthesia without the need for an extra device that is attached to the patient's arm. The BP measurements are returned at the same rate as pulse, enabling a much higher sampling rate of blood pressure, and thus denser data to estimate trends.

2. The arousal state of a patient can be determined by the burst-suppression patterns in the EEG. Since fNIRS is a great proxy for brain activity, and is much more robust to movements and perturbations, it makes a great candidate for monitoring patient brain function in the ICU.

<b>
Discretizing complex dynamics
</b>

The dynamics of the two signals can be fed into an event-state detection algorithm (such as the one described in [Project 1](/portfolio/05_event-state-detection)) that can divide the timeseries into different events and states, which can be tracked over time, and used as variables to predict the outcome of different treatments or interventions.

This is a project that is very close to my heart, and I am eagerly waiting for an opportunity to validate and implement a working system in the ICU.
