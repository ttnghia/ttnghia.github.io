+++
date = "2018-04-10"
title = "A Narrow-Range Filter for Screen-Space Fluid Rendering"
draft = false
image = "img/portfolio/narrow-range-filter/thumbnail.jpg"
showonlyimage = false
weight = 1
+++

<!--more-->
<p align="center">
Nghia Truong & [Cem Yuksel](http://cemyuksel.com/) <br/>
[ACM SIGGRAPH Symposium on Interactive 3D Graphics and Games 2018](http://i3dsymposium.github.io/2018/) <br/><br/>
<img src="/img/portfolio/narrow-range-filter/teaser.png" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
</p>


#### Abstract
We introduce a simple screen-space filtering technique for real-time rendering of particle-based fluid simulations. Starting with a depth-map generated directly from the particle data, our new filter formulation smooths the depth-map by considering the depth values in a narrow range. The depth values outside of this range are carefully handled to achieve the desired surface shape near discontinuities. The simplicity of our formulation leads to a computationally efficient filter. We present examples with complex particle-based
fluid simulations and provide comparisons, clearly showing that our filter provides improved surface quality in terms of surface smoothness and preserving boundaries near discontinuities, as compared to prior filtering methods.


#### Download
[Paper (preprint, 23MB pdf)](/pdf/portfolio/NarrowRangeFilter.pdf) <br/>
[Demo: https://github.com/ttnghia/RealTimeFluidRendering](https://github.com/ttnghia/RealTimeFluidRendering) <br/>

---
<p align="center">
<h4 align="center">Video and Screenshots</h4>


<div style="position:relative;padding-top:60%;">
<iframe src="https://player.vimeo.com/video/264166270" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

---
<img src="/img/portfolio/narrow-range-filter/armadillo.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>

<img src="/img/portfolio/narrow-range-filter/bunny.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>

<img src="/img/portfolio/narrow-range-filter/lucy.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>

<img src="/img/portfolio/narrow-range-filter/tori.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>

<img src="/img/portfolio/narrow-range-filter/spheres.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>

<img src="/img/portfolio/narrow-range-filter/emitter.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>

---

Updated: April 2018.