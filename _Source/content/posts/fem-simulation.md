---
title: "Finite Element Simulation"
date: 2020-09-02T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- code
- graphics
- fem
- simulation
- c++
- magnum
categories:
- code
image: images/fem-simulations/thumbnail.png
---


Some simple simulation examples using Finite Element Method.

<!--more-->
### Description
A Finite Element Method simulation using the technique proposed in the paper [Quasi-Newton Methods for Real-Time Simulation of Hyperelastic Materials](https://dl.acm.org/doi/10.1145/2990496). With a L-BFGS updates, the method can accelerate the simulation significantly, producing a real-time frame rate even for relatively large tetrahedral meshes. This example is heavily adopted from the [source code provided by the paper authors](https://github.com/ltt1598/Quasi-Newton-Methods-for-Real-time-Simulation-of-Hyperelastic-Materials).

After the simulation started, wind force will be added after 10 seconds. The wind parameters, along with other simulation parameters, can be changed at run time.


### Download
TBA.

### Usage
TBA.


### Video
<p align="center">
<div style="position:relative;padding-top:60%;">
<iframe src="https://player.vimeo.com/video/454149542" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
</p>

<p align="center">
<div style="position:relative;padding-top:60%;">
<iframe src="https://player.vimeo.com/video/454150165" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
</p>


<!--
### Gallery
<p align="center">
<img src="/images/fem-simulations/1.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/fem-simulations/2.png" alt="A screenshot of the program" style="width: 80%;"/>
</p>

-->