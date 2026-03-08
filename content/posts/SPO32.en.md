---
title: "SPO32"
date: 2024-06-12T00:00:00Z
description: "A project that combines multiple daily tools in one device, including a digital clock and Spotify controller."
draft: false
---

![SPO32](/PersonalWEB2.0/images/SPO32.png)

This is the most **complex** project I have built so far. I wanted to combine several everyday tasks in a single device so I would not have to switch windows constantly.

Implemented features include:

- A **digital clock** showing current, maximum, and minimum daily temperature.
- A **Spotify controller** with track info, remaining time, and playback control.

---

### Challenges and solutions

The first big challenge was using **two LCD screens** at once. Their registers conflicted, so both could not be connected directly to the same **ESP32**. I solved this using a **multiplexer**.

The ESP32 connects to multiple APIs: weather, time, and Spotify.

Screen switching is done with a **button**, and music control uses a **rotary encoder**.

---

Take a look at the demo video or the GitHub repository.

[Watch video](https://drive.google.com/file/d/1mFgUo-aFKgUav3_NED-ebNgKQcrPmU-6/preview)

{{< admonition info "Visit the project" >}}
[View on GitHub](https://github.com/RodrigoPerez943/ESPO32)
{{< /admonition >}}
