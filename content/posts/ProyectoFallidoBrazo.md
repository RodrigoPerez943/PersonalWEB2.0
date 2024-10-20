---
title: "Proyecto Fallido, Brazo Robótico"
date: 2024-08-13T10:30:39+02:00
description: "Diseño, impresión y programación de un brazo robótico para el pulido de piedras preciosas."
draft: false
toc: false
images:
pin: false
---

Estaba viendo un día **reels** en YouTube y me salió un video de un tío puliendo piedras preciosas y su facetación. Todo era manual, y se me ocurrió la idea de hacer un brazo robótico que, mediante un algoritmo, pudiera facetear la piedra preciosa según un modelo en 3D.

No tenía ni idea de diseño de piezas por ordenador, así que hice un curso corto de **CAD** para aprender. ¡Y me puse manos a la obra con el proyecto!

---

## La idea general:

1. **Brazo robótico** que sostiene la piedra, con **tres ejes**:
    * Dos ejes para el movimiento vertical.
    * Uno con mayor radio de giro.
    * Otro con menor radio para ajustes finos.
    * Un eje final de rotación circular para poder girar la piedra.
    
2. **Base abrasiva giratoria** que quitaría las capas de la piedra a medida que el brazo ajusta su posición.

3. **Algoritmo de control** para el movimiento del brazo.


![Brazo](/PersonalWEB2.0/images/brazo.gif)

---

## Mi workflow:

1. **Compré los servos** en AliExpress.
2. **Diseñé el brazo robótico** en base a los servos comprados. Aquí me encontré con un problema importante: los servos baratos tenían muchas **holguras** y **muy poco torque**, lo que los hacía **inconsistentes** y **poco precisos**. 😓
3. Comencé a **programar en Arduino**, pero los servos no eran lo suficientemente potentes. Decidí que no quería gastar más dinero en nuevos servos (unos 15€ por cada uno), así que dejé el proyecto pausado... hasta que consiga unos servos decentes o me apetezca gastar el dinero. 💸

{{< figure src="images/brazo.jpg" alt="brazo" caption="Brazo Impreso en 3D" class="webp" loading="lazy" width="600">}}

---

## El Algoritmo (que no llegué a desarrollar):

A continuación, te explico la idea básica del algoritmo que planeaba utilizar para calcular los movimientos del brazo robótico:

1. **Suponer un cubo** con dimensiones \(x \times x \times x\) y representarlo con una **matriz tridimensional**. El número de filas y columnas dependería de la resolución deseada, representando la piedra antes de los cortes.

2. Tener **modelos de los cortes** en formato de matriz tridimensional con la misma resolución que la del cubo original.

3. **Generar una nueva matriz** que contenga los puntos de diferencia entre las dos matrices (el cubo final y el original sin cortes).

4. Esta nueva matriz representaría los **puntos a eliminar** mediante cortes superficiales planos.

5. **Búsqueda de superficies**: Mediante vectores directores, el algoritmo buscaría puntos contiguos que compartieran el mismo vector para identificar superficies planas. Después de eso, calcularía la **distancia** a eliminar desde el punto central de la superficie hasta el punto más lejano a eliminar.

6. Finalmente, se tendría un **listado de superficies y distancias** a eliminar, y el siguiente paso sería diseñar el algoritmo que controlaría el movimiento del brazo robótico, tomando en cuenta su posición en el espacio y la posición de la base abrasiva.

---

### Reflexión final:

Me estoy planteando realizar el **algoritmo para calcular las superficies** a eliminar... ¡sería un buen reto! 💡
