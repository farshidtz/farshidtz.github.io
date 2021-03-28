---
title: cvPaint - Simple drawing using camera
date: 2012-01-18T00:00:00Z
description: Simple painting using the camera input.
aliases: ["/projects/112"]
---

cvPaint is an application which allows simple drawing using camera input. The key features include changing color, size, erasing and saving the image by holding a pointer on the available toolbars.

<!-- https://www.youtube.com/watch?v=o556bMSQkOo -->
{{< youtube o556bMSQkOo >}}


This application is developed in C++ using the well known OpenCV Library. The application demo and the list of all features are available below:

## Control Features with Camera

-   Changing the brush color
-   Changing the brush thickness
-   Clearing the screen
-   Saving the image
-   Closing the application

## Noise Handing

-   Setting threshold for the maximum distance between two points
-   Getting use of the pointer's area to distinguish between the pointer itself and noises
-   Using a 5x5 Median Filter to reduce the background noise

## Source Code
https://github.com/farshidtz/cvPaint