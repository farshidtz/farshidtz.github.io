---
title: Freehand Circling for Object Selection Using a Head-mounted Camera
date: 2014-08-05T00:00:00Z
description: Circle around anything in your view and search for it! A head-mounted system to connect you with your search engine.
aliases: ["/projects/121"]
otherContributors: ["Jiawei Gu", "Jiabin He"]
---

Baidu Eye is prototype head-mounted device with front facing camera. As a research intern in  [Baidu's Institute of Deep Learning](http://idl.baidu.com/en/), I was responsible for developing a light algorithm that allows wearer to circle around things in his view using his pointing finger in order to select a specific object from a large scene. The selected item was then sent to [Baidu's image search API](http://stu.baidu.com/) for object recognition.

This can be used for searching image of products, banners, logos, and even clipping a portion of an advertisement.

## Main challanges

-   Avoiding registration of close points to prevent hand shaking errors
-   Ending selection by approaching a loop
-   **Getting a clean shot of object that is not covered by hand**
<!-- https://www.youtube.com/watch?v=L39pFYDagDY -->
{{< youtube L39pFYDagDY >}}

- Counteracting background movements to fix the selection using:
  -   Lucas-Kanade optical flow algorithm
  -   Classifying camera versus other movements (hand, background noise)

<!-- https://www.youtube.com/watch?v=mAVJ8_AXx28 -->
{{< youtube mAVJ8_AXx28 >}}
