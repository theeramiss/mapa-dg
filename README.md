# Mapa de Diseño Gráfico, FADU UBA

Mapa interactivo de las materias de Diseño Gráfico (FADU, UBA) y sus correlativas. Marcás qué materias cursaste y aprobaste, y te muestra cuáles ya podés cursar y tu porcentaje de avance.

## Cómo usarlo

- **Online (recomendado):** abrí el link de GitHub Pages del repositorio, [theeramiss.github.io/mapa-dg](https://theeramiss.github.io/mapa-dg/) . En el celu podés agregarla a la pantalla de inicio y se abre como una app, con su ícono, y funciona sin internet.
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

## Publicarla en GitHub Pages

Subí a la misma carpeta del repositorio `index.html`, `manifest.webmanifest`, `sw.js` y los íconos (`icon-180.png`, `icon-192.png`, `icon-512.png`). Los últimos tres archivos de código solo hacen falta para la versión online: permiten agregarla a la pantalla de inicio y usarla sin internet. Cuando subas una versión nueva de `index.html`, quien ya la tenga la recibe la siguiente vez que la abra con conexión.

## Adaptarlo a otra carrera

Podés hacer tu propia versión para otra carrera, de FADU o de otra facultad, sin saber programar. La idea es hacerlo con ayuda de un asistente de IA (Claude, ChatGPT, Gemini u otro): vos le pasás los datos de tu carrera y el archivo, y la IA hace los cambios.

### 1. Hacé tu copia en GitHub

1. Creá una cuenta en GitHub si no tenés.
2. Entrá a este repositorio y tocá **Fork**, arriba a la derecha. Se crea una copia en tu cuenta. Si querés cambiarle el nombre (por ejemplo, `mapa-arquitectura`), lo hacés en Settings.
3. Activá GitHub Pages en tu copia: Settings → Pages → Branch `main`, carpeta `/ (root)` → Save. En un par de minutos te aparece tu link, del estilo `https://tuusuario.github.io/nombre-del-repo/`. Anotalo.
4. Descargá `index.html` y `manifest.webmanifest` desde tu copia: abrí cada archivo y tocá el botón de descarga, arriba a la derecha.

### 2. Juntá la información de tu carrera

- El **cuadro de correlatividades** de tu plan, en PDF, como foto o copiado como texto.
- La **carga horaria** de cada materia y si es anual o cuatrimestral (suele estar en la página de la carrera o en el plan de estudios).
- Cuáles materias son de **promoción directa** (sin final).
- Si hay electivas, optativas o seminarios: la **lista de materias** que se pueden elegir en cada caso.

### 3. Pedile los cambios a la IA

Abrí una conversación nueva, adjuntá `index.html`, `manifest.webmanifest` y la información del paso anterior, y copiá el mensaje que está más abajo.

> [!IMPORTANT]
> Antes de mandarlo, cambiá las dos partes que están entre corchetes: el nombre de tu carrera, la facultad y el plan (por ejemplo, Arquitectura, FADU UBA, Plan 2023), y tu link de GitHub Pages, el que anotaste en el paso 1.

**Mensaje para copiar:**

> Este `index.html` es un mapa interactivo de materias y correlativas hecho para Diseño Gráfico (FADU, UBA). Quiero adaptarlo a mi carrera: **[nombre de la carrera, facultad y plan]**. Te adjunto el cuadro de correlatividades, la carga horaria y la lista de electivas/optativas.
>
> Cambiá solo los datos, sin tocar el diseño ni el resto de la lógica:
> - El bloque que empieza con `/* ---- DATOS: editá acá si cambia el plan ---- */`: las listas de materias para elegir, `BASE` y `Y` (años y materias con sus correlativas), siguiendo el mismo formato.
> - `DIRECT` (promoción directa) y `HS` (horas y si es anual "A" o cuatrimestral "C"). Todas las materias de `Y` tienen que estar en `HS`.
> - El `<title>` y el subtítulo (`<p class="sub">`).
> - `KEY` (en `var LAST=null,KEY=...`): un nombre nuevo para mi carrera, por ejemplo `"mapa-arq-v1"`.
> - `LINK_ONLINE`: **[tu link de GitHub Pages]**.
> - En `manifest.webmanifest`: `name` y `short_name`.
>
> Ojo con estas partes hechas a medida de Diseño Gráfico: el primer año de `Y` se trata como CBC (códigos `c1` a `c9`); el último año se muestra más ancho, en columnas; los casilleros con código `OP` o `SE` tienen la opción "Otra"; y hay reglas propias para `FI` y para "Estética". Adaptalas o quitalas si mi carrera no las necesita. Si algo del cuadro no está claro, preguntame antes de inventar.
>
> Devolveme los dos archivos completos y una lista de lo que cambiaste.

### 4. Subí los archivos y revisá

1. En tu copia de GitHub, tocá "Add file" → "Upload files", subí los dos archivos que te devolvió la IA y tocá "Commit changes".
2. Esperá uno o dos minutos y abrí tu link.
3. **Revisá las correlativas contra el cuadro oficial**: la IA se puede equivocar. Probá marcar algunas materias y fijate si se desbloquean las que corresponden. En la vista Mapa, al tocar una materia, se ven sus correlativas.

Si la página queda en blanco o algo no funciona, volvé a la misma conversación con la IA y contale qué pasa. Si podés, sumá una captura, o el mensaje de error que aparece en la consola del navegador (F12 → Consola).
