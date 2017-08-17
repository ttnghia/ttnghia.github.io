---
layout: post
title:  "Simple Signed Distance Field Visualizer"
date:   2017-08-16 21:50:00
preview: /images/2017-08-16-sdf-visualizer/thumbnail.jpg
category: Rendering
tags: [Rendering]
---

* The program is written for my personal testing of signed distance field implementation.
* Particles are generated and grouped into two parts: one with particles at negative distance values to object surface (inside), and one with particles at positve distance values (outside). The particles' colors fall off as the absolute distance increasing.
* Support clipped-plane to look inside the object.
* Signed distance functions for various primitives are implemented. Constructive solid geometry is considered as a nested signed distance function. The signed distance function for a triangle mesh is much more difficult. Its implementation is adapted by [Chris Batty's implementation](https://github.com/christopherbatty/SDFGen).
---

# Screenshots:

![1](/images/2017-08-16-sdf-visualizer/1.png)

![2](/images/2017-08-16-sdf-visualizer/2.png)

![3](/images/2017-08-16-sdf-visualizer/3.png)

![3](/images/2017-08-16-sdf-visualizer/4.png)

![3](/images/2017-08-16-sdf-visualizer/5.png)

![3](/images/2017-08-16-sdf-visualizer/6.png)

![3](/images/2017-08-16-sdf-visualizer/7.png)
<br>

---

# Code:
[https://github.com/ttnghia/SDFVisualizer](https://github.com/ttnghia/SDFVisualizer)

---

# References

* [http://iquilezles.org/www/articles/distfunctions/distfunctions.htm](http://iquilezles.org/www/articles/distfunctions/distfunctions.htm)
* [https://github.com/christopherbatty/SDFGen](https://github.com/christopherbatty/SDFGen)
