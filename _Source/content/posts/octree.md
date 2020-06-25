---
title: "Octree"
date: 2020-06-24T00:00:00-07:00
description: 
draft: false
hideToc: false
enableToc: true
enableTocContent: false
tocPosition: outer
tags:
- code
- graphics
- octree
- c++
- magnum
categories:
- code
image: images/octree/thumbnail.png
---


An implementation of [loose octree](https://anteru.net/blog/2008/loose-octrees/) with application in collision detection for particle simulation.

<!--more-->
### Description
This is a simple, single-threaded implementation of a [loose octree](https://anteru.net/blog/2008/loose-octrees/) which is commonplace in computer graphics. It is used for various purposes, for example, for collision detection in particle simulation, as in this program.


### Download
[Magnum example page with more description](https://doc.magnum.graphics/magnum/examples-octree.html)
[Code (github) from Magnum repository](https://github.com/mosra/magnum-examples/tree/master/src/octree)
[Windows binary](/exe/Octree.exe)

### Usage
* `Mouse drag` rotates the camera
* `Shift + mouse drag` pans the camera
* `Mouse wheel` zooms in/out
* `R` resets the camera to its original transformation
* `B` shows/hides tree node bounding boxes
* `Space` pauses/resumes particle simulation

Additionally, various options can be set via command line:

```
-s, --spheres N — number of spheres to simulate (default: 50)
-r, --sphere-radius R — sphere radius (default: 0.1)
-v, --sphere-velocity V — sphere velocity (default: 1)
```

For example:

```
Octree.exe -s 20 -r 0.1 -v 1.0
```

### Gallery
<p align="center">
<img src="/images/octree/1.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/octree/2.png" alt="A screenshot of the program" style="width: 80%;"/>
<br />
<img src="/images/octree/3.png" alt="A screenshot of the program" style="width: 80%;"/>
</p>

