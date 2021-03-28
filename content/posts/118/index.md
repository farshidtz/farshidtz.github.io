---
title: Parallel Convex-Hull solver
date: 2013-01-25T00:00:00Z
description: A parallel Planar Convex-Hull solver which operates on a single or a cluster of machines to analyse performance improvements.
aliases: ["/projects/118"]
---

Based on the definition from  [Princeton](http://www.cs.princeton.edu/courses/archive/spr10/cos226/demo/ah/ConvexHull.html), the convex hull of a set of points is:

- Formally: It is the smallest convex set containing the points.  
- Informally: It is a rubber band wrapped around the "outside" points.

This application was designed to compare time complexity of convex hull problem in both parallel and sequential algorithms. The convex hull problem is solved based on the  [Graham's scan](http://www.cs.princeton.edu/courses/archive/spr10/cos226/demo/ah/GrahamScan.html) algorithm.

![](MPI_1Ma1Pr_100.png)

## Techniques

-   Parallelization using  [OpenMPI](http://www.open-mpi.org/)  in C++
-   Graphical visualization using C++ Graphics library (Linux)


{{< figure src="convex_hull_time_comparison.png" title="Comparison of execution time for 100, 1000, 10000 and 30000 points for MPI runs with 1 Machine 1 Process , 1 Machine 4 Processes and 2 Machines 8 Processes" >}}


## Source Code
https://github.com/farshidtz/convexhull  
[Graph Library](libgraph.tar.gz)