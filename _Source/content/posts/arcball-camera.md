---
title: "ArcBall Camera"
date: 2020-02-03T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- code
- graphics
- c++
- magnum
- webgl
categories:
- code
- webgl
image: images/arcball-camera/thumbnail.png
---


An implementation of [Ken Shoemake's arcball camera](https://www.talisman.org/~erlkonig/misc/shoemake92-arcball.pdf) with smooth navigation feature.

<!--more-->
### Description
This is an implementation of [Ken Shoemake's arcball camera](https://www.talisman.org/~erlkonig/misc/shoemake92-arcball.pdf) with smooth navigation feature. Using arcball, the camera control is more accurate and consistent.


### Download
[Magnum example page with more description](https://doc.magnum.graphics/magnum/examples-arcball.html)
[Code (github) from Magnum repository](https://github.com/mosra/magnum-examples/tree/master/src/arcball)
[Windows binary](/exe/ArcBallCamera.exe)

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
    <script async="async" src="/webgl/magnum-arcball.js"></script>
  </div></div></div>
</div>

### Usage
* `Mouse drag` rotates the camera
* `Shift + mouse drag` pans the camera
* `Mouse wheel` zooms in/out
* `R` resets the camera to its original transformation
* `L` toggles lagging (smooth camera navigation)

### Gallery
<p align="center">
<img src="/images/arcball-camera/1.png" alt="A screenshot of the program" style="width: 70%;"/>
</p>
