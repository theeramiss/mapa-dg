# Mapa de Diseño Gráfico, FADU UBA

Mapa interactivo de las materias de Diseño Gráfico (FADU, UBA) y sus correlativas. Marcás qué materias cursaste y aprobaste, y te muestra cuáles ya podés cursar y tu porcentaje de avance.

## Cómo usarlo

- **Online (recomendado):** abrí el link de GitHub Pages del repositorio (https://theeramiss.github.io/mapa-dg/). En el celu podés agregarla a la pantalla de inicio y se abre como una app, con su ícono, y funciona sin internet.
  - **iPhone:** en Safari tocá Compartir y después "Agregar a inicio". Conviene hacerlo: si usás la página desde Safari y no la abrís durante unos días, Safari puede borrar lo guardado. La app agregada a inicio guarda su avance aparte del de Safari; si ya habías marcado materias en Safari, pasalas con "Copiar código" y "Pegar código".
  - **Android:** en Chrome, menú ⋮ y "Agregar a la pantalla principal" o "Instalar app".
- **Archivo descargado:** descargá `index.html` y abrilo con doble clic en la compu. No necesita instalar nada. En iPhone no sirve abrirlo desde la app Archivos, porque ahí solo se ve una vista previa y no se puede marcar nada: usá la versión online.

Tiene dos temas fijos, Día y Noche, y un tercero, "Mi tema", donde elegís el color de fondo y el de acento (con opciones rápidas o cualquier color), la tipografía (Classic, Notes, Mono o Lover, con Garamond incluida en el archivo), que también cambia el estilo del tachado. La forma de los indicadores de la barra de progreso (círculo, cuadrado, corazón, estrella, luna, flor, nube, trébol, gato o pez) se elige aparte y funciona en cualquier tema. La app calcula sola el resto de los colores para que se lea bien. También hay una pestaña "Notas" para guardar links y datos sueltos. Tu avance y tus elecciones se guardan solo en tu dispositivo, no se envían a ningún lado.

## Cómo funciona

Con las pestañas "Lista" y "Mapa" cambiás de vista. En el mapa ves todas las materias por año y, al tocar una, las líneas con sus correlativas; ahí también podés cambiar su estado.

En la lista, tocá el círculo de cada materia: pendiente, final pendiente (ya cursaste y te falta rendir el final) y aprobada. Las materias de promoción directa pasan directo de pendiente a aprobada. Una materia se desbloquea cuando cumplís sus correlativas. Electivas, optativas y seminarios tienen un casillero donde elegís o escribís cuál hiciste.

## Fuente y aclaraciones

Basado en el cuadro de correlatividades y en las páginas de Diseño Gráfico de FADU. Es una herramienta no oficial hecha por una estudiante: ante cualquier duda, confirmá con la facultad. Las correlativas y las listas de materias están al principio del script en `index.html` por si el plan cambia.

## Notas, promedio y horas

Al aprobar una materia aparece un campo para cargar la nota. Arriba de todo se ven las materias aprobadas, las horas aprobadas (según la carga horaria publicada por FADU) y el promedio de las notas que cargues, que puede diferir del oficial de la facultad.

Con la casilla "Incluir el CBC en el organizador" (apagada por defecto) elegís si el CBC cuenta en todo: lista, mapa, puntitos, horas, materias y promedio. Apagada, el organizador muestra solo la carrera y da por cumplido el CBC para las correlativas.

## Pasar tu avance a otro dispositivo

Abajo de todo están "Copiar link", "Copiar código" y "Pegar código". En el dispositivo donde tenés el avance copiás el link o el código; en el otro abrís el link o tocás "Pegar código". Antes de cargarlo, la app avisa cuántas materias trae y que va a **reemplazar** todo lo que haya guardado en ese dispositivo (materias, notas, promedio y bloc de notas).

El avance viaja dentro del link o del código (comprimido). No pasa por ningún servidor. "Copiar link" funciona en la versión online; con el archivo descargado, usá el código. Si publicás la app en GitHub Pages, poné su dirección en `LINK_ONLINE`, al final del script de `index.html`, y el link también va a andar desde el archivo descargado.
