---
title: "[Code] FFT-based Ocean Surface Simulation"
date: 2017-07-02T00:00:00-07:00
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
- rendering
- c++
series:
-
categories:
-
image: images/code-fft-based-ocean-simulation/thumbnail.jpg
---


<!--more-->

### Description

* The program is implemented in Qt 5.9 framework.
* Multi-threading by Intel TBB and fftw3_threads libraries.
* Skybox textures in folder Textures/Sky are automatically loaded at start up.
* Press Spacebar key to pause/resume the simulation.
* Simulation parameters can be changed and take effects in real time.
* A binary (in Pre-Build folder) has been provided.
* As my implementation depends on a lot of external libaries, the source code can only be compiled by me.


### References:

* Jerry Tessendorf, 1999. [Simulating Ocean Water](https://people.cs.clemson.edu/~jtessen/papers_files/coursenotes2004.pdf)
* Some code in my program is adapted from this repository: [https://github.com/ZijinZheng/OceanSurface](https://github.com/ZijinZheng/OceanSurface)


### Download
[Code (github) with windows prebuild](https://github.com/ttnghia/OceanSurfaceSimulation)


### Video
<p align="center">
<div style="position:relative;padding-top:60%;">
<iframe src="https://player.vimeo.com/video/223991874" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
</p>


### Gallery
<p align="center">
<img src="/images/code-fft-based-ocean-simulation/1.jpg" alt="FFT-based Ocean Surface Simulation" style="width: 100%;"/>
<br />
<img src="/images/code-fft-based-ocean-simulation/2.jpg" alt="FFT-based Ocean Surface Simulation" style="width: 100%;"/>
<br />
<img src="/images/code-fft-based-ocean-simulation/3.jpg" alt="FFT-based Ocean Surface Simulation" style="width: 100%;"/>
<br />
<img src="/images/code-fft-based-ocean-simulation/4.jpg" alt="FFT-based Ocean Surface Simulation" style="width: 100%;"/>

</p>