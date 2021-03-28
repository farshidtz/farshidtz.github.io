---
title: "Smartphone Position Detection Using Neural Networks"
date: 2015-10-16T00:00:00Z
description: Make the smartphone context-aware by knowing whether it is in hand, in sidepocket, in a handbag, or left on a surface.
aliases: ["/projects/122"]
otherContributors: ["Omar Al-Safi"]
---

This project demonstrates an approach to detect common smart phone positions, including “In Hand”, “Side Pocket”, “In Handbag”, and “On Table (Idle)”. We apply sensor data fusion on a set of hardware- and software-based Android sensors. As a result, data entries containing sensor fusion features are classified individually, without looking at patterns. The overall system design and accuracy are presented using a Google Nexus 6 device.

<center>
{{< figure src="network.png" title="The fully connected NN used for classification. Nodes: 13 - 8 - 8 - 4" width="80%" >}}

{{< figure src="prediction.png" title="Prediction system diagram. Remote prediction using Weka." width="80%" >}}

{{< figure src="android-app-logging.jpg" title="Android Application: Logging mode" width="40%" >}}

{{< figure src="android-app-prediction.jpg" title="Android Application: Prediction mode" width="40%" >}}
</center>

## Source Code
https://github.com/farshidtz/mss2015

## Talk
[Slides](slides.pdf)