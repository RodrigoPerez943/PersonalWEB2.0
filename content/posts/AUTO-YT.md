---
title: "AUTO-YT"
date: 2024-01-12T00:00:00Z
description: "Un sistema automatizado para generar contenido en YouTube usando la API de Google y scraping."
draft: false
---
![AUTOYT](/PersonalWEB2.0/images/auto-yt.png)

Quería investigar la monetización de YouTube mediante la creación de un canal automatizado. Con la API de Google para YouTube y algo de scraping, conseguí generar contenido en pocos minutos, sin necesidad de editar ni buscar contenido. 

Para su funcionamineto se debe incluir tus credenciales de una cuenta de instagram para poder obtener los videos de las cuentas a las que se sigues.También es necesaria la cuenta de Google del canal en el que queremos subir los vídeos, siendo necesaria una cuenta de desarrolador. El programa guarda en una base de datos los identificadores para los vídeos subidos, al obtener los posibles vídeos a subir se checkean con la base de datos para ver si con anterioridad se han subido.

Hay dos opciones: 

- **Subir un YouTube Short**: El programa se inicia y busca los vídeos de formato vertical en las cuentas seguidas, obtiene nombres y checkea con la base de datos a ver si han sido subidos a Shorts o a una compilación de vídeos. Es importante que no duren más de 1 minuto, por lo que tengan mayor duración también se descartaran. Puedes ser que no haya ningun vídeo nuevo, por lo que el programa acabará su ejecución. Después de encontrar un vídeo que haya pasado todas las normas, se pasará al ususrio un link por consola para confirmar que ese vídeo le parece bien. Una vez confirmado se procede a la subida del vídeo. Es importante modificar los diferentes ajustes para modificar el nombre, generarlo de forma automática o modificar su descripcción. Un vez acabado este proceso el Short se subirá en cuestión de segundos.

- **Crear recopilaciones de vídeos**: Si elegimos esta opción, elegiremos el número de videos que queremos scrapear de las cuentas que seguimos en Instagram, en caso de que queramos añadir un intro/outro a la compilación lo inidicaremos en los ajustes del programa. Al igual que con los shorts, debemos indicar o generar de forma automática los nombres de los vídeos y sus descripcciones. El proceso es práticamente idéntico, un poco más lento ya que el montaje de los vídeos y el formateado se lleva a cabo con la librería MoviePy, la cual no es especialmente eficiente.

Visítalo en GitHub y echa un vistazo al código!

![AUTOYT](/PersonalWEB2.0/images/autpyt.png)

{{< admonition info "¡Visita el proyecto!" >}}
[Visitar en Github - Bajo mantenimiento]
{{< /admonition >}}

