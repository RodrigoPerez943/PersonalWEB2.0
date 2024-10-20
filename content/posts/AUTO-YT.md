---
title: "AUTO-YT"
date: 2024-01-12T00:00:00Z
description: "Un sistema automatizado para generar contenido en YouTube usando la API de Google y scraping."
draft: false
---

![AUTOYT](/PersonalWEB2.0/images/auto-yt.png)

Quería investigar la **monetización en YouTube** mediante la creación de un canal automatizado. Usando la **API de Google para YouTube** y algunas técnicas de **scraping**, logré generar contenido en pocos minutos, sin necesidad de edición ni búsqueda manual de contenido.

---

## ¿Cómo funciona?

Para que el sistema funcione correctamente, se requieren:

- **Credenciales de una cuenta de Instagram** para obtener vídeos de las cuentas seguidas.
- Acceso a la **cuenta de Google** del canal donde se subirán los vídeos.
- Una **cuenta de desarrollador** para autenticarse.

El programa almacena en una base de datos los identificadores de los vídeos subidos. Cuando busca nuevos vídeos, verifica si ya fueron subidos previamente para evitar duplicaciones.

---

## Opciones disponibles:

1. ### **Subir un YouTube Short**:
   El programa busca vídeos en formato vertical en las cuentas de Instagram seguidas. Los pasos son los siguientes:

   - Verifica si el vídeo ya ha sido subido a la base de datos.
   - Si el vídeo dura menos de 1 minuto y cumple con los requisitos, el sistema muestra un enlace en la consola para que el usuario lo confirme.
   - Tras la confirmación, el vídeo se sube automáticamente a **YouTube Shorts**.
   
   💡 *Es importante ajustar el nombre y la descripción del vídeo antes de subirlo.*

2. ### **Crear recopilaciones de vídeos**:
   - Permite seleccionar varios vídeos para crear una **compilación**.
   - Se puede elegir cuántos vídeos scrapear de Instagram y si se desea añadir una **intro/outro**.
   - El proceso es un poco más lento que el de los Shorts, ya que se utiliza **MoviePy** para editar y formatear los vídeos.

![AUTOYT](/PersonalWEB2.0/images/autpyt.png)


---

## ¿Te interesa ver el código?

{{< admonition info "¡Visita el proyecto!" >}}
[Visitar en GitHub - Bajo mantenimiento]
{{< /admonition >}}

