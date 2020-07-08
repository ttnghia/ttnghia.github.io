---
title: "Ray Tracing In One Weekend"
date: 2020-01-29T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- code
- graphics
- ray tracing
- rendering
- c++
- magnum
- webgl
categories:
- code
- webgl
image: images/ray-tracing-over-the-weekend/thumbnail.png
---


An implementation of a simple ray tracer adapted from Peter Shirley's book [Ray Tracing in One Weekend](https://raytracing.github.io/books/RayTracingInOneWeekend.html).

<!--more-->
### Description
This is an implementation of a simple ray tracer adapted from Peter Shirley's book [Ray Tracing in One Weekend](https://raytracing.github.io/books/RayTracingInOneWeekend.html). The current implementation runs on single thread and performs iterative rendering to refine the result. Typically, a high quality image can be achieved after around 100 iterations. In addition, a new scene can be easily generated to overwrite the current scene by a keyboard shortcut.

### Download
[Magnum example page with more description](https://doc.magnum.graphics/magnum/examples-raytracing.html)
[Code (github) from Magnum repository](https://github.com/mosra/magnum-examples/tree/master/src/raytracing)
[Windows binary](/exe/RayTracing.exe)

### WebGL Demo
Thanks [Vladimír Vondruš](https://github.com/mosra/) for building the awesome WebGL application. This is part of [Magnum](https://magnum.graphics/) graphics engine showcase. Note that this WebGL demo requires WebAssembly-capable browser with WebGL enabled.

Usage:
    * `Mouse drag` rotates the camera
    * `Shift + mouse drag` pans the camera
    * `Mouse wheel` zooms in/out
    * `R` resets the camera to its original transformation
    * `D` toggles depth-of-field rendering
    * `M` toggles marking the next render block by a different color
    * `N` generates a new random scene
    * `Space` pauses/resumes rendering
	
<link rel="stylesheet" href="/webgl/WebApplication.css" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<div id="container">
  <div id="sizer"><div id="expander"><div id="listener">
    <canvas id="canvas"></canvas>
    <div id="status">Initialization...</div>
    <div id="status-description"></div>
    <script src="/webgl/EmscriptenApplication.js"></script>
    <script async="async" src="/webgl/magnum-raytracing.js"></script>
  </div></div></div>
</div>


### Gallery
<p align="center">
<img src="/images/ray-tracing-over-the-weekend/1.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/ray-tracing-over-the-weekend/2.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/ray-tracing-over-the-weekend/3.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/ray-tracing-over-the-weekend/4.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/ray-tracing-over-the-weekend/5.png" alt="A screenshot of the program" style="width: 90%;"/>
</p>
