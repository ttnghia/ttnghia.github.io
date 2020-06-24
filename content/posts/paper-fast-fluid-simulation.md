---
title: "[Paper] Fast Fluid Simulations with Sparse Volumes on the GPU"
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
categories:
- publication
image: images/paper-fast-fluid-simulation/thumbnail.jpg
---




<!--more-->
<p style="text-align: center !important; font-size: 20px; font-weight: 500;">
Kui Wu, Nghia Truong, <a href="http://cemyuksel.com">Cem Yuksel</a>, <a href="http://ramakarl.com">Rama Hoetzlein</a>
<br />
<em>Eurographics 2018</em>
<br/><br/>
<img src="/images/paper-fast-fluid-simulation/teaser.jpg" style="width: 100%;"/>
</p>


### Abstract
We introduce efficient, large scale fluid simulation on GPU hardware using the fluid-implicit particle (FLIP) method over a sparse hierarchy of grids represented in [NVIDIA GVDB Voxels](https://developer.nvidia.com/gvdb). Our approach handles tens of millions of particles within a virtually unbounded simulation domain. We describe novel techniques for parallel sparse grid hierarchy construction and fast incremental updates on the GPU for moving particles. In addition, our FLIP technique introduces sparse, work efficient parallel data gathering from particle to voxel, and a matrix-free GPU-based conjugate gradient solver optimized for sparse grids. Our results show that our method can achieve up to an order of magnitude faster simulations on the GPU as compared to FLIP simulations running on the CPU.


### Download
[Paper (preprint, 13MB pdf)](/pdf/2018GVDB.pdf) 


### BibTeX
```
@article{Wu2018,
author = {Wu, Kui and Truong, Nghia and Yuksel, Cem and Hoetzlein, Rama},
title = {Fast Fluid Simulations with Sparse Volumes on the GPU},
journal = {Computer Graphics Forum},
volume = {37},
number = {2},
pages = {157-167},
year = {2018},
doi = {10.1111/cgf.13350}
}
```


### Video
<p align="center">
<div style="position:relative;padding-top:60%;">
<iframe src="https://www.youtube.com/embed/7VPPKKpde3A" allow="autoplay; encrypted-media" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
</p>

### Gallery
<p align="center">
<img src="/images/paper-fast-fluid-simulation/screenshots.jpg" alt="Fast Fluid Simulations with Sparse Volumes on the GPU" style="width: 100%;"/>
</p>
