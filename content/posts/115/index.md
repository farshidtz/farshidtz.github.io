---
title: 2D Mapping Using an Autonomous Robot
date: 2013-01-22T00:00:00Z
description: A robot is utilized to perform simple mapping tasks using sonar sensor in a structured environment.
aliases: ["/projects/115"]
otherContributors: ["Bahador Saket"]
---

This project represents a method for performing 2D mapping with a mobile robot on a single floor of a structure. The observation of an environment with the robot requires positioning and sensing systems which are associated with different types of errors.

The robot uses the differential drive movement system to navigate in an environment containing walls, edges and corners. The movement of robot is tracked with odometry and goes through Kalman Filter to get optimized estimations.

The robot navigates in the environment and on every interval, scans the surroundings with circular rotations of a sonar sensor. The result of the sonar readings is subject to specular reflection errors which will go through several techniques to get as minimized as possible. Circular sonar scans generate local maps where will be combined to create the global map of the environment.

## Techniques

-   Robotic movement and sensing control via Bluetooth (Using  [Monobrick C++ Communication Library](http://www.monobrick.dk/software/c-library/) for NXT)
-   Noise reduction of movement system with [Kalman Filter](http://en.wikipedia.org/wiki/Kalman_filter) by getting external references from the sonar sensor
-   Interpretation of sonar readings with a geometric model to detect and reduce specular reflections
-   Mapping local maps to global map with generation of probability of occupancy
-   Filtering the global map to reduce environmental noises
-   Generation of a graphical image representing the map of the working environment

## Demo
The video below is the demo of mapping in a small environment. The robot scans the environment in every 5cm of movement. The complete mapping of this environment takes about 30 minutes.

<!-- https://www.youtube.com/watch?v=sl4xhit_E8w -->
{{< youtube sl4xhit_E8w >}}
