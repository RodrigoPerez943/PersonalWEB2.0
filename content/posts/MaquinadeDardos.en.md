---
title: "Dart Machine Modernization"
date: 2024-10-02T10:30:39+02:00
description: "Upgrading an old LED display system to OLED."
draft: false
toc: false
images:
pin: false
---
At a lunch with my mother, I met the **CEO of a darts federation** that owns a large stock of old **dart machines**. They have been looking for someone to help **upgrade the displays**, which still rely on **7-segment displays and LEDs** from the 80s and 90s.

I said I could help and visited the warehouse with a friend for initial testing.

---

### First impressions

The machines are very **vintage**. I searched for manuals beforehand but found very little, likely because they were custom-developed for that federation.

{{< figure src="images/dardosmaquinacompleta.jpg" alt="Full dart machine" caption="Full dart machine" class="webp" loading="lazy" width="600">}}

---

### Technical description

The **main board** connects all machine parts and buttons. The display is connected through a **40-pin bus**.

- **17 pins** carry information.
- **3 pins** are: one unknown, one ground, and one power.
- **13 pins** vary.
- **4 pins** are constant, all 1s.

{{< figure src="images/dardosdev.jpg" alt="Open dart machine" caption="Open dart machine" class="webp" loading="lazy" >}}

---

### Action plan

For **reverse engineering**, we will try different **button combinations** and observe how bus bits change. We suspect the processor sends state changes rather than full data, meaning part of the processing happens on the **display board**.

---

### Next steps

We will start by decoding the bus bit meanings, then analyze the display PCB in detail.
