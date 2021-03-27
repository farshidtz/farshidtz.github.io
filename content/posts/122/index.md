---
title: "Smartphone Position Detection Using Neural Networks"
date: 2015-10-16T00:00:00Z
description: 
aliases: ["/projects/122"]
---

This application is developed in C++ using the well known OpenCV Library. The application demo and the list of all features are available below:

**Control Features with camera:**

-   Changing the brush color
-   Changing the brush thickness
-   Clearing the screen
-   Saving the image
-   Closing the application

**Noise Handing:**

-   Setting threshold for the maximum distance between two points
-   Getting use of the pointer's area to distinguish between the pointer itself and noises
-   Using a 5x5 Median Filter to reduce the background noiseThis project demonstrates an approach to detect common smart phone positions, including “In Hand”, “Side Pocket”, “In Handbag”, and “On Table (Idle)”. We apply sensor data fusion on a set of hardware- and software-based Android sensors. As a result, data entries containing sensor fusion features are classified individually, without looking at patterns. The overall system design and accuracy are presented using a Google Nexus 6 device.

<center>
{{< figure src="network.png" title="The fully connected NN used for classification. Nodes: 13 - 8 - 8 - 4" width="80%" >}}


{{< figure src="prediction.png" title="Prediction system diagram. Remote prediction using Weka." width="80%" >}}

{{< figure src="android-app-logging.jpg" title="Android Application: Logging mode" width="40%" >}}

{{< figure src="android-app-prediction.jpg" title="Android Application: Prediction mode" width="40%" >}}
</center>


[Source Codes](https://github.com/farshidtz/mss2015) | [Slides](slides.pdf)