---
title: "Fluid Simulation 2D"
date: 2019-11-12T00:00:00-07:00
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
image: images/fluid-simulation-2d/thumbnail.png
---


A 2D fluid simulation using the hybrid grid/particle approach with APIC ([Affine Particle-in-Cell](https://dl.acm.org/doi/10.1145/2766996)) transfer.

<!--more-->
### Description
A 2D fluid simulation using the hybrid grid/particle approach with APIC ([Affine Particle-in-Cell](https://dl.acm.org/doi/10.1145/2766996)) transfer.


### Download
[Magnum example page with more description](https://doc.magnum.graphics/magnum/examples-fluidsimulation2d.html)
[Code (github) from Magnum repository](https://github.com/mosra/magnum-examples/tree/master/src/fluidsimulation2d)
[Windows binary](/exe/FluidSimulation2D.exe)

### WebGL Demo
Thanks [Vladimír Vondruš](https://github.com/mosra/) for building the awesome WebGL application. This is part of [Magnum](https://magnum.graphics/) graphics engine showcase.

<link rel="stylesheet" href="/webgl/WebApplication.css" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<div id="container">
  <div id="sizer"><div id="expander"><div id="listener">
    <canvas id="canvas"></canvas>
    <div id="status">Initialization...</div>
    <div id="status-description"></div>
    <script src="/webgl/EmscriptenApplication.js"></script>
    <script async="async" src="/webgl/magnum-fluidsimulation2d.js"></script>
  </div></div></div>
</div>


### Usage
* `Mouse drag` rotates the camera
* `E` emits more particles
* `H` shows/hides the overlaid menu
* `R` resets the simulation
* `Space` pauses/resumes the simulation

### Gallery
<p align="center">
<table style="border-collapse: collapse; border: none; width: 100%">
<tr>
<td>
<img src="/images/fluid-simulation-2d/1.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
<td>
<img src="/images/fluid-simulation-2d/2.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
</tr>
<tr>
<td>
<img src="/images/fluid-simulation-2d/3.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
<td>
<img src="/images/fluid-simulation-2d/4.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
</tr>
</table>

<table style="border-collapse: collapse; border: none; width: 100%">
<tr>
<td>
<img src="/images/fluid-simulation-2d/5.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
<td>
<img src="/images/fluid-simulation-2d/6.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
</tr>
<tr>
<td>
<img src="/images/fluid-simulation-2d/7.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
<td>
<img src="/images/fluid-simulation-2d/8.png" alt="A screenshot of the program" style="width: 100%;"/>
</td>
</tr>
</table>
</p>
