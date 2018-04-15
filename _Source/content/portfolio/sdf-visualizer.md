+++
date = "2017-08-16"
title = "Signed Distance Field Visualizer"
draft = false
image = "img/portfolio/sdf-visualizer/thumbnail.png"
showonlyimage = false
weight = 1
+++

<!--more-->

#### Description

* The program is written for my personal testing of signed distance field implementation.
* Particles are generated and grouped into two parts: one with particles at negative distance values to object surface (inside), and one with particles at positve distance values (outside). The particles' colors fall off as the absolute distance increasing.
* Signed distance functions for various primitives are implemented. Constructive solid geometry is considered as a nested signed distance function. The signed distance function for a triangle mesh is much more difficult. Its implementation is adapted by [Chris Batty's implementation](https://github.com/christopherbatty/SDFGen).
* Support clipped-plane to look inside the object.

#### References

* [http://iquilezles.org/www/articles/distfunctions/distfunctions.htm](http://iquilezles.org/www/articles/distfunctions/distfunctions.htm)
* [https://github.com/christopherbatty/SDFGen](https://github.com/christopherbatty/SDFGen)


#### Download
Code (can compile only by me): [https://github.com/ttnghia/SDFVisualizer](https://github.com/ttnghia/SDFVisualizer)


---
<p align="center">
<h4 align="center">Screenshots</h4>

<img src="/img/portfolio/sdf-visualizer/1.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

<img src="/img/portfolio/sdf-visualizer/2.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

<img src="/img/portfolio/sdf-visualizer/3.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

<img src="/img/portfolio/sdf-visualizer/4.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

<img src="/img/portfolio/sdf-visualizer/5.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

<img src="/img/portfolio/sdf-visualizer/6.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

<img src="/img/portfolio/sdf-visualizer/7.png" alt="Signed Distance Field Visualizer" style="width: 100%;"/>

---

Updated: April 2018.
