---
layout: post
title: "Implantable fNIRS"
description: "A wireless, batteryless, completely implantable fNIRS system"
date: 2018-01-01T15:30:30-04:00
img: /img/in1.jpg
---

**A wireless, minimally-invasive, batteryless, completely implantable fNIRS system**

Epidural fNIRS, having shown remarkable promise in capturing correlates of highly localized neural events, when combined with the results from my studies on neurovascular coupling, emerges as the perfect tool for recording neural activity without compromising the dura.

Our results from EEG-fNIRS studies demonstrate that it is easier to classify brain-states using fNIRS than EEG (due to the non-stationarity of the EEG signal and its features). This makes epidural fNIRS a fantastic candidate for long term epilepsy / stroke monitoring as well as neurofeedback applications.

With that in mind, I am currently working on a peri-osteal wireless implant that will record fNIRS activity and enable neurofeedback.

A prototpye is currenlty under development using the Texas Instrument's MSP-430/AFE4490 Launchpad, which has been designed for use as a PPG sensor for smart-watches.
I've written some code to configure the device parameters (such as sampling rates, LED brightness, etc) and to record the data. It resides in a repo [here](https://github.com/theonlyid/SendReceive).

A few pictures of the prototype are below:

<img class="col three" src="{{ site.url }}{{ site.baseurl}}/img/in1.jpg">

<img class="col one" src="{{ site.url }}{{ site.baseurl}}/img/in2.jpg">
<p>
<img class="col two" src="{{ site.url }}{{ site.baseurl}}/img/in3.png">
