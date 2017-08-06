---
layout: post
title:  "Ocean Simulation using Fast Fourier Transform"
date:   2017-07-02 21:50:00
preview: /images/2017-07-02-ocean-simulation-using-fft/thumbnail.JPG
category: Simulation
tags: [Simulation]
---

* The program is implemented in Qt 5.9 framework.
* Multi-threading by Intel TBB and fftw3_threads libraries.
* Skybox textures in folder Textures/Sky are automatically loaded at start up.
* Press Spacebar key to pause/resume the simulation.
* Simulation parameters can be changed and take effects in real time.
* A binary (in Pre-Build folder) has been provided.
* As my implementation depends on a lots of external libaries, the source code can only be compiled by me.

---

# Screenshots:

![1](/images/2017-07-02-ocean-simulation-using-fft/1.JPG)

![2](/images/2017-07-02-ocean-simulation-using-fft/2.JPG)

![3](/images/2017-07-02-ocean-simulation-using-fft/3.JPG)

![4](/images/2017-07-02-ocean-simulation-using-fft/4.JPG)

---
<br>
# Video:
---
<iframe src="https://player.vimeo.com/video/223991874" width="960" height="540" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

---
<br>
# Code
[Github repository](https://github.com/ttnghia/FFTOceanSimulation)

---
<br>
# References

The computation code in my program is adapted from this repository: [https://github.com/ZijinZheng/OceanSurface](https://github.com/ZijinZheng/OceanSurface)