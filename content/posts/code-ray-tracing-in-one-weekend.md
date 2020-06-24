---
title: "Ray Tracing In One Weekend"
date: 2020-06-13T00:00:00-07:00
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
categories:
- code
image: images/code-ray-tracing-over-the-weekend/thumbnail.png
---



<!--more-->
### Description
This is an implementation of a simple ray tracer adapted from Peter Shirley's book [Ray Tracing in One Weekend](https://raytracing.github.io/books/RayTracingInOneWeekend.html). The current implementation runs on single thread and performs iterative rendering to refine the result. Typically, a high quality image can be achieved after around 100 iterations. In addition, a new scene can be easily generated to overwrite the current scene by a keyboard shortcut.



### Download
[Magnum example page with more description](https://doc.magnum.graphics/magnum/examples-raytracing.html)
[Code (github) from Magnum repository](https://github.com/mosra/magnum-examples/tree/master/src/raytracing)
[Windows binary](/exe/RayTracing.exe)


### Gallery
<p align="center">
<img src="/images/code-ray-tracing-over-the-weekend/1.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/code-ray-tracing-over-the-weekend/2.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/code-ray-tracing-over-the-weekend/3.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/code-ray-tracing-over-the-weekend/4.png" alt="A screenshot of the program" style="width: 90%;"/>
<br />
<img src="/images/code-ray-tracing-over-the-weekend/5.png" alt="A screenshot of the program" style="width: 90%;"/>
</p>
