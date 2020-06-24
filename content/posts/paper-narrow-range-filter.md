---
title: "A Narrow-Range Filter for Screen-Space Fluid Rendering"
date: 2018-04-10T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- publication
- graphics
- fluid
- simulation
- rendering
- code
- c++
categories:
- publication
image: images/paper-narrow-range-filter/thumbnail.jpg
---


<!--more-->
<p style="text-align: center !important; font-size: 20px; font-weight: 500;">
Nghia Truong and <a href="http://cemyuksel.com">Cem Yuksel</a>
<br />
<em>ACM SIGGRAPH Symposium on Interactive 3D Graphics and Games 2018</em>
<br/><br/>
<img src="/images/paper-narrow-range-filter/teaser.png" style="width: 100%;"/>
</p>



### Abstract
We introduce a simple screen-space filtering technique for real-time rendering of particle-based fluid simulations. Starting with a depth-map generated directly from the particle data, our new filter formulation smooths the depth-map by considering the depth values in a narrow range. The depth values outside of this range are carefully handled to achieve the desired surface shape near discontinuities. The simplicity of our formulation leads to a computationally efficient filter. We present examples with complex particle-based fluid simulations and provide comparisons, clearly showing that our filter provides improved surface quality in terms of surface smoothness and preserving boundaries near discontinuities, as compared to prior filtering methods.


### Download
[Paper (preprint, 23MB pdf)](/pdf/NarrowRangeFilter.pdf) 
[Code (github)](https://github.com/ttnghia/RealTimeFluidRendering)


### BibTeX
```
@article{Truong2018,
author = {Truong, Nghia and Yuksel, Cem},
title = {A Narrow-Range Filter for Screen-Space Fluid Rendering},
year = {2018},
issue_date = {July 2018},
publisher = {The Association for Computers in Mathematics and Science Teaching},
volume = {1},
number = {1},
journal = {Proc. ACM Comput. Graph. Interact. Tech.},
month = jul,
articleno = {17},
numpages = {15}
}
```


### Video
<p align="center">
<div style="position:relative;padding-top:60%;">
<iframe src="https://player.vimeo.com/video/264166270" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
</p>


### Gallery
<p align="center">
<img src="/images/paper-narrow-range-filter/armadillo.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
<br />
<img src="/images/paper-narrow-range-filter/bunny.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
<br />
<img src="/images/paper-narrow-range-filter/lucy.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
<br />
<img src="/images/paper-narrow-range-filter/tori.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
<br />
<img src="/images/paper-narrow-range-filter/spheres.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
<br />
<img src="/images/paper-narrow-range-filter/emitter.jpg" alt="A Narrow-Range Filter for Screen-Space Fluid Rendering" style="width: 100%;"/>
</p>
