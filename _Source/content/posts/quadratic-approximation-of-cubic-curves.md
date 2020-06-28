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
categories:
- code
- publication
libraries:
- katex
image: images/quadratic-approximation/thumbnail.png
---

A simple degree reduction technique for converting piecewise cubic splines into piecewise quadratic splines that maintain parameterization and $C^1$ continuity.

<!--more-->
<p style="text-align: center !important; font-size: 20px; font-weight: 500;">
Nghia Truong, <a href="http://cemyuksel.com">Cem Yuksel</a> and Larry Seiler
<br />
<a href="https://www.highperformancegraphics.org/2020/"><em>High-Performance Graphics 2020</em>]</a>
<br/><br/>
<img src="/images/quadratic-approximation/teaser.png" style="width: 100%;"/>
</p>



### Abstract
We present a simple degree reduction technique for piecewise cubic polynomial splines, converting them into piecewise quadratic splines that maintain the parameterization and $C^1$ continuity. Our method forms identical tangent directions at the interpolated data points of the piecewise cubic spline by replacing each cubic piece with a pair of quadratic pieces. The resulting representation can lead to substantial performance improvements for rendering geometrically complex spline models like hair and fiber-level cloth. Such models are typically represented using cubic splines that are $C^1$-continuous, a property that is preserved with our degree reduction. Therefore, our method can also be considered a new quadratic curve construction approach for high-performance rendering. We prove that it is possible to construct a pair of quadratic curves with $C^1$ continuity that passes through any desired point on the input cubic curve. Moreover, we prove that when the pair of quadratic pieces corresponding to a cubic piece have equal parametric lengths, they join exactly at the parametric center of the cubic piece, and the deviation in positions due to degree reduction is minimized.


### Download
[Paper: coming soon](/pdf/QuadraticApproximation.pdf) 
[Code (github)](https://github.com/ttnghia/QuadraticApproximation)

### Video

Coming soon.

### Gallery

(To be updated)

<p align="center">
<img src="/images/quadratic-approximation/1.png" style="width: 100%;"/>
<br />
<img src="/images/quadratic-approximation/2.png" style="width: 100%;"/>
<br />
</p>
