---
title: "AUTO-YT"
date: 2024-01-12T00:00:00Z
description: "Un sistema automatizado para generar contenido en YouTube usando la API de Google y scraping."
draft: false
---
![AUTOYT](/PersonalWEB2.0/images/auto-yt.png)

Quería investigar la monetización en **YouTube** mediante la creación de un canal automatizado. Utilizando la **API de Google para YouTube** y algunas técnicas de **scraping**, logré generar contenido en pocos minutos, sin necesidad de edición ni búsqueda manual de contenido.

### Funcionamiento

Para su correcto funcionamiento, se deben incluir las credenciales de una cuenta de **Instagram** para obtener vídeos de las cuentas seguidas. También es necesario tener acceso a la **cuenta de Google** del canal en el que se subirán los vídeos, además de una **cuenta de desarrollador** para autenticarse. El programa guarda en una base de datos los identificadores de los vídeos subidos, y cuando se buscan nuevos vídeos para subir, se verifica si ya han sido subidos previamente.

### Opciones disponibles

1. **Subir un YouTube Short**:  
   El programa busca vídeos en formato vertical en las cuentas de Instagram seguidas. Se obtiene el nombre del vídeo y se verifica en la base de datos si ya ha sido subido. Si el vídeo dura menos de 1 minuto y cumple con los requisitos, se muestra un enlace en la consola para que el usuario confirme si desea subirlo. Tras la confirmación, el vídeo se sube automáticamente a **YouTube Shorts**. Es importante ajustar el nombre y la descripción del vídeo antes de la subida.

2. **Crear recopilaciones de vídeos**:  
   Esta opción permite seleccionar varios vídeos para crear una compilación. Puedes elegir cuántos vídeos scrapear de las cuentas seguidas en Instagram, y si deseas añadir una intro/outro al vídeo, lo indicas en los ajustes del programa. El proceso es similar al de los Shorts, pero un poco más lento, ya que la edición y el formateo de los vídeos se realiza con **MoviePy**, una librería que, aunque funcional, no es la más rápida.

Visítalo en **GitHub** y echa un vistazo al código!

![AUTOYT](/PersonalWEB2.0/images/autpyt.png)

{{< admonition info "¡Visita el proyecto!" >}}
[Visitar en Github - Bajo mantenimiento]
{{< /admonition >}}
