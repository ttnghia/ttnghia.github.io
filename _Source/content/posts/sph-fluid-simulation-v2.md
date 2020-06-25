---
title: "SPH Fluid Simulation (v2)"
date: 2019-11-08T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- code
- graphics
- fluid
- simulation
- particle
- c++
- magnum
categories:
- code
image: images/sph-fluid-simulation-v2/thumbnail.png
---



<!--more-->
### Description
A basic implementation of SPH (Smoothed-Particle Hydrodynamics) solver with a dynamic boundary. In order to run in real time, accuracy has been heavily sacrificed for performance. 

I also had another SPH simulation code which only deals with static boundary [here](/posts/sph-fluid-simulation-v1/). 


### Download
[Magnum example page with more description](https://doc.magnum.graphics/magnum/examples-fluidsimulation3d.html)
[Code (github) from Magnum repository](https://github.com/mosra/magnum-examples/tree/master/src/fluidsimulation3d)
[Windows binary](/exe/SPHFluidSimulation.exe)

### Usage
* `Mouse drag` rotates the camera
* `Shift + mouse drag` pans the camera
* `Mouse wheel` zooms in/out
* `H` shows/hides the overlaid menu
* `R` resets the simulation
* `Space` pauses/resumes the simulation

### Gallery
<p align="center">
<img src="/images/sph-fluid-simulation-v2/1.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/sph-fluid-simulation-v2/2.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/sph-fluid-simulation-v2/3.png" alt="A screenshot of the program" style="width: 80%;"/>
</p>
