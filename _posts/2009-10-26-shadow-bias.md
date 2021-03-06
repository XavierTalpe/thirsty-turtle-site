---
layout: post
title: 'Shadow bias'
published: true
---

As Jurgen pointed out this afternoon, a bias of 0.25 (see post below) for my depth maps isn't good since depth values are already clamped in the range of [0, 1]. Adding another quarter of that to my depth values is obviously no correct way of rendering shadows. The images below show the improved results with smaller bias values:

{:.text-center}
![Dragon](/uploads/2010/11/Dragon1.png)
![Dragon](/uploads/2010/11/Dragon2.png)

{:.text-center}
**Bias of 0.005**

{:.text-center}
![Dragon](/uploads/2010/11/Dragon3.png)
![Dragon](/uploads/2010/11/Dragon4.png)

{:.text-center}
**Bias of 0.01**

Compared to a 0.25 bias my shadows look a lot more realistic now and less out of place:

{:.text-center}
![Dragon](/uploads/2009/10/Dragon8.png)
