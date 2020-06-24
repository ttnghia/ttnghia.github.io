---
title: "Particle Sampling with SPH-based Relaxation"
date: 2018-06-14T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- code
- graphics
- particle
- simulation
- c++
categories:
- code
image: images/code-particle-sampling-with-sph-relaxation/thumbnail.png
---

A tool for generating evenly distributed particles from a given geometry.

<!--more-->
### Description
Particle-based simulation is prevalent in computer graphics. In order to run the simulations, we firstly need to have particles. Therefore, generating particles in a desired distribution is very important, if not indispensable. If the simulation resolution is not high enough, uneven distributed particles could probably lead to wrong solutions, or at least ugly looking results.

I have struggled a lot in trying to generate evenly distributed particles for my simulation projects and came up with several solutions. One of them is Lloyd relaxation, but it requires two levels particle sampling - one normal scale and one much smaller scale, leading to huge amount of memory usage and yields very slow performance. Another solution is using [SPH-based blue noise relaxation](https://dl.acm.org/citation.cfm?id=2818102), which has a very good performance and produces good results and became my top choice. I implement that algorithm in my program `ParticleSampler`, which allows to generate particles from a given geometry, run relaxation over the generated particles, and save the results to disk for further processing somewhere else. More details about the program and its usage is discussed more in detail in my github project below.


### Download
[Code (github) with examples scene and docs](https://github.com/ttnghia/ParticleSampler)


### Gallery
<p align="center">
<table style="border-collapse: collapse; border: none; width: 100%">
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_box.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_capsule.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_ellipsoid.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_hexagon.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_sphere.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_triangle.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_torus.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_torus88.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/2D_torusInfInf.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
</table>
<br/>
<table style="border-collapse: collapse; border: none; width: 100%">
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_box.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_capsule.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_cone.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_cylinder.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_ellipsoid.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_hexagonal_prism.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_sphere.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_torus.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_torus2inf.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_torus28.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_torus88.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_torusinfinf.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_triangular_prism.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_mesh_bear.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_mesh_bunny.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
</table>
<br/>
<table style="border-collapse: collapse; border: none; width: 100%">
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_mesh_dragon.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_mesh_elk.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
<tr>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_mesh_lion.png" alt="A screenshot of the program" style="width: 95%;"/></td>
<td><img src="/images/code-particle-sampling-with-sph-relaxation/3D_mesh_tricertp.png" alt="A screenshot of the program" style="width: 95%;"/></td>
</tr>
</table>
</p>




### Video
<p align="center">
<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196205" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196253" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196292" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196353" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196386" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196450" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>

<div style="position:relative;padding-top:75%;">
<iframe src="https://player.vimeo.com/video/275196421" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
<br/>
</p>
