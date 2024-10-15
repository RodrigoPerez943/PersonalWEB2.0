---
title: "SPO32"
date: 2024-06-12T00:00:00Z
description: "Un proyecto que unifica varias aplicaciones en un solo dispositivo, incluyendo un reloj digital y un controlador de Spotify."
draft: false
---

![SPO32](/PersonalWEB2.0/images/SPO32.png)

Este proyecto es el más complejo y extenso que he realizado. La idea surgió porque quería unificar varias acciones que realizaba todos los días en diferentes aplicaciones en un único dispositivo. Me molestaba bastnate cambiar de ventana en el portatil siempre que quería cambia de canción en Spotify o ver el tiempo que hacía. Las funcionalidades implementadas son las siguientes:

- **Reloj digital** con la temperatura actual, máxima y mínima del día.
- **Controlador de Spotify** que muestra el tiempo restante de la canción en reproducción, la información de la canción, permite cambiarla, ir a la anterior y pausarla. 

El primer gran problema que tuve, fue que quería usar dos pantallas. Pero al parecer los registros que usan las pantallas LCD suelen ser el mismo por lo que no se pueden unir las dos a la vez al mismo ESP, por lo que tuve que usar un multiplexor. El ESP-32 se conecta por WI-FI a un API de la cual obtiene el tiempo en mi ubicación, otra API de la cual obtiene la hora actual y por último a la API de Spotify para poder controlar la música. Para el cambio de panatalla uso un botón y para el cambio de los controles utilizo un Rotatory Encoder. Échale un vistazo al vídeo de demostración o visítalo en GitHub!
 
[Ver Video](https://drive.google.com/file/d/1mFgUo-aFKgUav3_NED-ebNgKQcrPmU-6/preview)

{{< admonition info "¡Visita el proyecto!" >}}
[Visitar en Github](https://github.com/RodrigoPerez943/ESPO32)
{{< /admonition >}}


