---
title: "Modernización Máquina de dardos"
date: 2024-10-02T10:30:39+02:00
description: "Modernización de una pantalla LED a OLED."
draft: false
toc: false
images:
pin: false
---
En una comida con mi madre conocí al **CEO de una federación de dardos** que tiene un gran stock de **máquinas de dardos antiguas**. Estas máquinas, utilizadas en competiciones y para su venta o alquiler a bares, ya están bastante desfasadas. Durante la comida, me comentó que llevaban tiempo buscando a alguien que les ayudara a **actualizar las pantallas** de las máquinas, que aún usan **displays de 7 segmentos y LEDs** de los años 80-90.

Me explicó el proyecto y, en un arranque de confianza, le dije que **podía ayudarle**. Como si no tuviese suficientes cosas que hacer entre la universidad y mi TFG… 😅 Decidí ir un día con un amigo a sus almacenes para echar un vistazo a las máquinas y hacer un **testeo inicial**.

---

### Primeras impresiones


La verdad es que las máquinas son bastante **vintage**. Estuve investigando manuales antes de ir, pero no encontré mucho, ya que parecen haber sido desarrolladas especialmente para esta federación. La **placa madre** tenía muchas opciones de testing y funcionalidades sin usar, lo que me hizo pensar que quizás no se completaron del todo o que recortaron costes dejando algunos elementos sin desarrollar. Aunque esto es solo una suposición mía.

{{< figure src="images/dardosmaquinacompleta.jpg" alt="Máquina de dardos completa" caption="Máquina de dardos completa" class="webp" loading="lazy" width="600">}}

---

### Descripción técnica

La **placa base** conecta todas las partes y botones de la máquina, pero lo que nos interesaba a nosotros era la **pantalla**, la cual está conectada mediante un **bus de 40 pines**. De estos pines:

- **17** transmiten información.
- **3** son: uno desconocido, uno de tierra y otro de corriente.
- **13** pines varían.
- **4** son constantes, todo 1's.

El proyecto está a punto de comenzar, aunque entre exámenes y TFG's está complicado sacar tiempo. 😅

{{< figure src="images/dardosdev.jpg" alt="Máquina de dardos completa" caption="Máquina de dardos abierta" class="webp" loading="lazy" >}}

---

### Plan de acción

Para hacer la **ingeniería inversa**, la idea es probar diferentes **combinaciones de botones** y ver cómo cambian los bits del bus de pines. El gran problema es que la máquina tiene muchos **modos de juego** y combinaciones, y los displays muestran tanto números como letras. 

Pensamos que el procesador solo envía los **cambios de estado**, pero no la información completa, lo que sugiere que el procesamiento de los cambios ocurre en la **placa del display**. Esto complica las cosas porque está lleno de memorias y otros componentes electrónicos que superan nuestro conocimiento actual de electrónica.

---

### Próximos pasos

Vamos a empezar probando y toqueteando los botones para ver si podemos **descifrar el significado de los bits** del bus. Luego, analizaremos el funcionamiento de la **PCB de la pantalla**. Afortunadamente, tenemos algunos documentos escritos por un ingeniero que trabajó en el proyecto, pero al leerlos me sentí como si estuviera leyendo chino. 🤯

Seguramente, este proyecto nos quede un poco grande… pero lo único que podemos perder es tiempo. ¡A ver cómo nos va!
