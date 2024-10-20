---
title: "SPO32"
date: 2024-06-12T00:00:00Z
description: "Un proyecto que unifica varias aplicaciones en un solo dispositivo, incluyendo un reloj digital y un controlador de Spotify."
draft: false
---

![SPO32](/PersonalWEB2.0/images/SPO32.png)

Este proyecto es el más **complejo y extenso** que he realizado hasta ahora. La idea surgió de la necesidad de **unificar varias tareas** que realizaba a diario en diferentes aplicaciones en un único dispositivo. Me resultaba incómodo cambiar de ventana en el portátil cada vez que quería cambiar de canción en **Spotify** o consultar el clima. Las funcionalidades implementadas incluyen:

- Un **reloj digital** que muestra la **temperatura actual**, junto con las temperaturas máxima y mínima del día.
- Un **controlador de Spotify** que muestra el tiempo restante de la canción en reproducción, información detallada de la canción, y permite cambiar, retroceder o pausar la reproducción.

---

### Desafíos y Soluciones

El primer gran desafío fue usar **dos pantallas LCD** simultáneamente. Descubrí que los registros de las pantallas eran los mismos, por lo que no podían conectarse al mismo **ESP32** al mismo tiempo. La solución fue usar un **multiplexor** para gestionarlo.

El **ESP32** se conecta a varias **APIs**: una para obtener el clima de mi ubicación, otra para la hora actual, y finalmente la API de **Spotify** para controlar la música.

El cambio entre las pantallas se realiza mediante un **botón**, y para controlar la música utilizo un **Rotary Encoder**.

---

Te invito a echar un vistazo al **video de demostración** o visitar el proyecto en **GitHub**.

[Ver Vídeo](https://drive.google.com/file/d/1mFgUo-aFKgUav3_NED-ebNgKQcrPmU-6/preview)

{{< admonition info "¡Visita el proyecto!" >}}
[Ver en GitHub](https://github.com/RodrigoPerez943/ESPO32)
{{< /admonition >}}

