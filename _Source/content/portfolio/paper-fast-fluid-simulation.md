+++
date = "2018-04-10"
title = "[Paper] Fast Fluid Simulations with Sparse Volumes on the GPU"
draft = false
image = "img/portfolio/paper-fast-fluid-simulation/thumbnail.jpg"
showonlyimage = false
description = " "
weight = 1
+++

<!--more-->
<p align="center">
[Kui Wu](http://www.cs.utah.edu/~kwu/), Nghia Truong, [Cem Yuksel](http://cemyuksel.com/), [Rama Hoetzlein](http://www.ramakarl.com/website/) <br/>
[Eurographics 2018](https://www.eurographics2018.nl/) <br/><br/>
<img src="/img/portfolio/paper-fast-fluid-simulation/teaser.jpg" alt="Fast Fluid Simulations with Sparse Volumes on the GPU" style="width: 100%;"/>
</p>


#### Abstract
We introduce efficient, large scale fluid simulation on GPU hardware using the fluid-implicit particle (FLIP) method over a sparse hierarchy of grids represented in [NVIDIA GVDB Voxels](https://developer.nvidia.com/gvdb). Our approach handles tens of millions of particles within a virtually unbounded simulation domain. We describe novel techniques for parallel sparse grid hierarchy construction and fast incremental updates on the GPU for moving particles. In addition, our FLIP technique introduces sparse, work efficient parallel data gathering from particle to voxel, and a matrix-free GPU-based conjugate gradient solver optimized for sparse grids. Our results show that our method can achieve up to an order of magnitude faster simulations on the GPU as compared to FLIP simulations running on the CPU.


#### Download
[Paper (preprint, 13MB pdf)](/pdf/portfolio/GVDB_FLIP.pdf) <br/>

---
<p align="center">
<h4 align="center">Video and Screenshots</h4>

<div style="position:relative;padding-top:60%;">
<iframe src="https://www.youtube.com/embed/7VPPKKpde3A" allow="autoplay; encrypted-media" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

---
<img src="/img/portfolio/paper-fast-fluid-simulation/screenshots.jpg" alt="Fast Fluid Simulations with Sparse Volumes on the GPU" style="width: 100%;"/>

---

Updated: April 2018.