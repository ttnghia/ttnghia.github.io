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
- webgl
categories:
- code
- webgl
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

### WebGL Demo
Thanks [Vladimír Vondruš](https://github.com/mosra/) for building the awesome WebGL application. This is part of [Magnum](https://magnum.graphics/) graphics engine showcase. Note that this WebGL demo requires WebAssembly-capable browser with WebGL enabled.

Due to restriction of WebGL, this demo only runs on a single thread. The desktop app runs at much higher speed with multi-threading enabled.

Usage:
    * `Mouse drag` rotates the camera
    * `Shift + mouse drag` pans the camera
    * `Mouse wheel` zooms in/out
    * `H` shows/hides the overlaid menu
    * `R` resets the simulation
    * `Space` pauses/resumes the simulation

<link rel="stylesheet" href="/webgl/WebApplication.css" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<div id="container">
  <div id="sizer"><div id="expander"><div id="listener">
    <canvas id="canvas"></canvas>
    <div id="status">Initialization...</div>
    <div id="status-description"></div>
    <script src="/webgl/EmscriptenApplication.js"></script>
    <script async="async" src="/webgl/magnum-fluidsimulation3d.js"></script>
  </div></div></div>
</div>


### Gallery
<p align="center">
<img src="/images/sph-fluid-simulation-v2/1.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/sph-fluid-simulation-v2/2.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/sph-fluid-simulation-v2/3.png" alt="A screenshot of the program" style="width: 80%;"/>
</p>
