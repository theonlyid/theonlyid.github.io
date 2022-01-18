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


The implant is designed to have the following characteristics, that are explained below:
[low-power](#lowpower), [ultra-thin](#thin), [charge-balanced](#charge), [modular](#modular), [batteryless](#batteryless), [wireless](#wireless), [fully encapsulated](#hermitic) [easily implantable](#easyimplant)

<a id="lowpower"></a>

<br>

**Low Power**

A major advantage of using fNIRS for monitoring cortical brain activity is that it can be sampled at a very low rate with very limited loss of information. This enables us to use ultra-low power microcontrollers to control data acquisition across multiple channels. Using lower power enables us to entirely remove the battery from the implanted device. It also enables communication over a low-bandwidth RF coil, making the device completely implantable on one hand, and reducing the risk of the battery leaking hazardous chemicals into the body on the other. This also makes the device ultra-thin.

<a id="charge"></a>

<br>

**Charge balanced**

A charge balanced system ensures that no charge or current is being injected into the body, which is very good for the local biophysiological processes including cell replication and repair.

<a id="thin"></a>

<br>

**Ultra-thin**

Not having a bulky battery allows us to use flexible materials as PCB and scaffolding, enabling us to reduce the thickness of the device by an order of magntude.

<a id="modular"></a>

<br>

**Modular**

Almost all medical devices have sensors wired to the control module. Which means if either the module or sensor fails, it renders the device unusable. What if the device and sensors could be separately packaged, allowing us the replace or update either one or the other independently? This device has a vision for the future of implantable medical electronics, and allows for modularity and complete physical separation between control module and sensors.


<a id="batteryless"></a>

<br>

**Wireless and battery-less**

Wires coming out of an implant that penetrate the skin pose a huge risk of infection. The solution is batteries that are placed along with the implant and the skin in sealed completely after implantation. However, batteries have a life, and are a huge risk for leakage, posing a threat to the health and safety of the user. Removing the battery allows the implant to have a significantly smaller form factor, being almost invisible under the skin, while reducing the risks associated with batteries. How is it powered? With an RF coil that acts as both power and data transmitter.


<a id="hermitic"></a>

<br>

**Fully encapsulated**

Some parts of implants such as sensors extend from the implant and pose a risk as they may allow inflammatory and corrosive materials to enter the device, limiting the life of the implant, and causing hazardous chemicals to leak into the tissue. The implant I am developing can be fully hermitically sealed ensuring there are no gaps or spaces allowing corrosive chemicals to enter the body. This adds to the long term stability of the implant and significantly reduces the risk to the user.


<a id="easyimplant"></a>

<br>

**Easily implantable**

What advantage does an ultra-thin device have? It enables easy implantation using only local anesthesia and two small incisions on the scalp. This means there is no need to book a surgery, drastically reducing the time and cost of implantation and explantation.


<br>

**A glimpse...**

A prototype using the Texas Instrument's MSP-430/AFE4490 Launchpad, which has been designed for use as a PPG sensor for smart-watches.
I've written some code to configure the device parameters (such as sampling rates, LED brightness, etc) and to record the data. It resides in a repo [here](https://github.com/theonlyid/SendReceive).

A few pictures of the prototype are below:

<img class="col three" src="{{ site.url }}{{ site.baseurl}}/img/in1.jpg">

<img class="col one" src="{{ site.url }}{{ site.baseurl}}/img/in2.jpg">
<p>
<img class="col two" src="{{ site.url }}{{ site.baseurl}}/img/in3.png">
