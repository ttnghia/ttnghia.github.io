---
title: "Quadratic Approximation of Cubic Curves"
date: 2020-06-28T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- publication
- graphics
- curve
- hair
- rendering
- code
- c++
- webgl
categories:
- code
- publication
- webgl
libraries:
- katex
image: images/quadratic-approximation/thumbnail.png
---

A simple degree reduction technique for converting piecewise cubic splines into piecewise quadratic splines that maintain parameterization and $C^1$ continuity.

<!--more-->
<p style="text-align: center !important; font-size: 20px; font-weight: 500;">
Nghia Truong, <a href="http://cemyuksel.com">Cem Yuksel</a> and Larry Seiler
<br />
<a href="https://www.highperformancegraphics.org/2020/"><em>High-Performance Graphics 2020</em></a>
<br/><br/>
<img src="/images/quadratic-approximation/teaser.png" style="width: 100%;"/>
</p>



### Abstract
We present a simple degree reduction technique for piecewise cubic polynomial splines, converting them into piecewise quadratic splines that maintain the parameterization and $C^1$ continuity. Our method forms identical tangent directions at the interpolated data points of the piecewise cubic spline by replacing each cubic piece with a pair of quadratic pieces. The resulting representation can lead to substantial performance improvements for rendering geometrically complex spline models like hair and fiber-level cloth. Such models are typically represented using cubic splines that are $C^1$-continuous, a property that is preserved with our degree reduction. Therefore, our method can also be considered a new quadratic curve construction approach for high-performance rendering. We prove that it is possible to construct a pair of quadratic curves with $C^1$ continuity that passes through any desired point on the input cubic curve. Moreover, we prove that when the pair of quadratic pieces corresponding to a cubic piece have equal parametric lengths, they join exactly at the parametric center of the cubic piece, and the deviation in positions due to degree reduction is minimized.


### Download
[Paper: (preprint, 10MB pdf)](/pdf/QuadraticApproximation.pdf)
[Code (github)](https://github.com/ttnghia/QuadraticApproximation)
[Windows binary](https://github.com/ttnghia/QuadraticApproximation/releases)


### WebGL Demo

Usage:
    * `Left mouse drag` rotates the camera
    * `Right mouse drag` translates the camera
    * `Mouse wheel` zooms in/out
    * `S` toggles smooth camera navigation

Notes:
    * This WebGL demo requires WebAssembly-capable browser with WebGL enabled and may not work correctly in Firefox.
    * The blue spheres are the control points of the cubic Bezier curve and red spheres are the control points of the approximated quadratic Bezier curves.
	* The blue control points (spheres) can be move around. Just click on them, and some handles will show up that allow translation.


<link rel="stylesheet" href="/webgl/WebApplication.css" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<div id="container" class="width-1000 aspect-1-1" oncontextmenu="return false;">
  <div id="sizer"><div id="expander"><div id="listener">
    <canvas id="canvas"></canvas>
    <div id="status">Initialization...</div>
    <div id="status-description"></div>
    <script src="/webgl/EmscriptenApplication.js"></script>
    <script async="async" src="/webgl/QuadraticApproximation.js"></script>
  </div></div></div>
</div>


### Video

<p align="center">
<div style="position:relative;padding-top:60%;">
<iframe src="https://player.vimeo.com/video/436551506" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>
</p>


### Gallery (Demo App)

<p align="center">
<img src="/images/quadratic-approximation/1.png" style="width: 80%;"/>
<br />
<img src="/images/quadratic-approximation/2.png" style="width: 80%;"/>
<br />
</p>
