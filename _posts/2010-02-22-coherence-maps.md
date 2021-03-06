---
layout: post
title: 'Coherence Maps'
published: true
---

Last week I've created a small program which allows me to render all of my compressed depth maps separately. This way I can manually look at each depth map and get an idea of how correct they are. I also implemented a way to render what I call **Coherence Maps**. These maps give an idea on how coherent each pixel is over all depth maps. When a pixel is white, it means that the depth value for this pixel is the same for all depth maps, and thus we have perfect coherence. A black pixel means the opposite, namely a lot of variation in the depth values for that pixel. This means a low coherence and low compression rate.

Some examples of these coherence maps are shown below:

{:.text-center}
![Coherence Map for Stanford Dragon](/uploads/2010/11/coherence-map-dragon.png)
![Coherence Map of Sphere](/uploads/2010/11/coherence-map-sphere.png)

{:.text-center}
Stanford Dragon (left) and Sphere (right)

{:.text-center}
![Coherence Map for Utah Teapot](/uploads/2010/11/coherence-map-teapot.png)
![Coherence Map for Stanford Bunny](/uploads/2010/11/coherence-map-bunny.png)

{:.text-center}
Utah Teapot (left) and Stanford Bunny (right)
