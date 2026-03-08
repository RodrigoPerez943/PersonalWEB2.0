---
title: "Failed Project: Robotic Arm"
date: 2024-08-13T10:30:39+02:00
description: "Design, printing, and control ideas for a robotic arm to polish gemstones."
draft: false
toc: false
images:
pin: false
---

One day I saw a video about gemstone polishing and faceting. Everything was manual, so I thought about building a robotic arm that could facet stones based on a 3D model.

I knew almost nothing about CAD at that point, so I took a short course and started building.

---

## General idea

1. A **robotic arm** holding the stone, with **three axes** plus final rotation.
2. A rotating **abrasive base** to remove layers.
3. A **control algorithm** for arm movement.

![Arm](/PersonalWEB2.0/images/brazo.gif)

---

## My workflow

1. Bought servos on AliExpress.
2. Designed the arm around those servos.
3. Started coding with Arduino.

Main issue: cheap servos had too much backlash and too little torque, so the system was not precise enough.

{{< figure src="images/brazo.jpg" alt="arm" caption="3D Printed Arm" class="webp" loading="lazy" width="600">}}

---

## The algorithm (I never finished)

The plan was to model the stone as a 3D matrix, compare it with the target faceting model, compute the material to remove, detect planar regions, and translate that into arm movements and cut depths.

---

### Final thought

I still want to implement the **surface-detection algorithm** one day. It would be a great challenge.
