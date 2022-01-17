---
layout: post
title: "Project 6"
description: "A wireless, batteryless, completely implantable fNIRS system"
date: 2021-12-01T15:30:30-04:00
img: /img/in1.jpg
---

**A wireless, minimally-invasive, batteryless, completely implantable fNIRS system**

Epidural fNIRS, having shown remarkable promise in capturing correlates of highly localized neural events, when combined with the results from my studies on neurovascular coupling, emerges as the perfect tool for recording neural activity without compromising the dura.

Our results from EEG-fNIRS studies demonstrate that it is easier to classify brain-states using fNIRS than EEG (due to the non-stationarity of the EEG signal and its features). This makes epidural fNIRS a fantastic candidate for long term epilepsy / stroke monitoring as well as neurofeedback applications.

With that in mind, I have been working on a peri-osteal wireless implant that will record fNIRS activity and enable neurofeedback.

<a id="lowpower"></a>

The implant is designed to have the following characterists, that are explained below:
[low-power](#lowpower), [ultra-thin](#thin), [charge-balanced](#charge), [modular](#modular), [batteryless](#batteryless), [wireless](#wireless), [fully encapsulated](#hermitic) [easily implantable](#easyimplant)

<a id="thin"></a>

**Low Power**

A major advantage of using fNIRS for mointoring cortical brain activity is that it can be sampled at a very low rate with very limited loss of information. This enables us to use ultra-low power microcontrollers to control data acqusition across multiple channels. Using lower power enables us to entirely remove the battery from the implanted device. It also enables communication over a low-bandwidth RF coil, making the device completely implantable on one hand, and reducing the risk of the battery leaking hazardous chemicals into the body on the other. This also makes the device ultra-thin.

<a id="charge"></a>

**Ultra-thin**

Not having a bulky battery allows us to use flexible materials as PCB and scaffolding, enabling us to reduce the thickness of the device by an order of magntude.

<a id="modular"></a>

**Modular**

The modularity 

A prototpye is currenlty under development using the Texas Instrument's MSP-430/AFE4490 Launchpad, which has been designed for use as a PPG sensor for smart-watches.
I've written some code to configure the device parameters (such as sampling rates, LED brightness, etc) and to record the data. It resides in a repo [here](https://github.com/theonlyid/SendReceive).

A few pictures of the prototype are below:

<img class="col three" src="{{ site.url }}{{ site.baseurl}}/img/in1.jpg">

<img class="col one" src="{{ site.url }}{{ site.baseurl}}/img/in2.jpg">
<p>
<img class="col two" src="{{ site.url }}{{ site.baseurl}}/img/in3.png">
