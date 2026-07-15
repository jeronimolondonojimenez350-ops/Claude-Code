# 🗓️ Cronograma semanal para dos personas

Una aplicación web sencilla para planear y comparar las rutinas semanales de dos
personas (por defecto **Ana** y **Jeronimo**). Todo vive en un **único archivo
HTML autónomo**: no necesita internet, ni servidor, ni instalar nada.

> Esta versión implementa el rediseño "Modernist" creado en claude.ai/design:
> cuatro vistas, modo oscuro y bloques que se arrastran con el mouse.

---

## ▶️ Cómo abrirlo

1. Descarga o localiza el archivo **`cronograma.html`**.
2. Haz **doble clic** sobre él. Se abrirá en tu navegador (Chrome, Edge, Firefox,
   Safari…).
3. ¡Listo! La primera vez verás unos bloques de ejemplo que puedes editar o
   borrar. Si ya usabas la versión anterior, tus datos se migran solos.

> No hace falta conexión a internet. Funciona totalmente sin red.

---

## ✨ Qué puedes hacer

| Función | Cómo se usa |
|---|---|
| **Vista Semana** | Lunes a Domingo con la línea de tiempo y dos carriles por día (uno por persona). |
| **Vista Día** | Un solo día en grande, con flechas ‹ › para navegar. Ideal en el móvil. |
| **Vista Lista** | Todos los bloques en una tabla ordenada; clic en una fila para editar. |
| **Vista Resumen** | Horas planificadas por categoría de cada persona, con barras comparables. |
| **Añadir un bloque** | Botón **+ Añadir bloque**, o clic sobre un hueco vacío del calendario. |
| **Mover un bloque** | **Arrástralo** con el mouse: puedes cambiarlo de hora, de día y hasta de persona. |
| **Cambiar su duración** | Arrastra el **borde inferior** del bloque hacia arriba o abajo. |
| **Editar o eliminar** | Un clic (sin arrastrar) sobre el bloque abre el editor, con botones Eliminar y Duplicar. |
| **Copiar un día a toda la semana** | Icono 📋 en la cabecera de cada día (o el botón grande en la vista Día). |
| **Ver tiempo libre juntos** | Las franjas donde **ambos** están libres se resaltan en verde ("Libres juntos"). |
| **Línea de "ahora"** | Una línea roja marca la hora actual sobre el día de hoy (etiqueta HOY). |
| **Modo claro / oscuro** | Botón 🌙/☀️ en la barra superior; se recuerda tu elección. |
| **Guardado automático** | Todo se guarda solo en el navegador; al volver a abrir sigue ahí. |
| **Exportar / Importar** | Botones ⬇️/⬆️ para guardar y recuperar un respaldo `.json`. |
| **Imprimir o PDF** | Imprime con **Ctrl+P** (o menú del navegador): sale una vista limpia sin botones. |
| **Móvil** | La semana se desplaza horizontalmente; la vista Día es perfecta para el teléfono. |

---

## ⚙️ Cómo personalizarlo (sin programar)

Abre el botón **⚙️ Configuración** (icono de controles) en la barra superior:

- **Los nombres** de las dos personas.
- El **rango horario visible** del día (por defecto **6:00 a 23:00**).
- La **precisión** de los bloques: **15, 30 o 60 minutos** (por defecto 30).
- Las **categorías** de actividad y su **color**: añadir, renombrar, recolorear
  o eliminar.

Los cambios se aplican y guardan al pulsar **Guardar cambios**.

### Categorías por defecto

Trabajo · Ejercicio · Comidas · Sueño · Tareas del hogar · Tiempo personal ·
Tiempo en pareja · Otros

---

## 🎨 Personalización avanzada (opcional, editando el archivo)

Si abres `cronograma.html` con un editor de texto encontrarás comentarios en
español y marcas **`>>> PERSONALIZAR <<<`** en las zonas fáciles de tocar:

- La **paleta de colores** de los temas claro y oscuro (variables al inicio).
- La **densidad del calendario** (`PX_POR_MIN`: súbelo para bloques más altos).
- La **línea de "ahora"** (`LINEA_AHORA`: ponla en `false` para ocultarla).
- Los **valores por defecto** (función `configPorDefecto`).

La tipografía del diseño es *Archivo*; si la tienes instalada se usa, y si no,
se usa la fuente del sistema (así el archivo sigue sin depender de internet).

---

## 💾 Sobre tus datos y respaldos

- Los datos se guardan en el **almacenamiento local del navegador**
  (`localStorage`). Son privados y quedan en tu equipo.
- Si venías de la **versión anterior**, tus bloques y configuración se migran
  automáticamente la primera vez que abras esta versión.
- Conviene **exportar un respaldo `.json`** de vez en cuando (botón ⬇️), sobre
  todo antes de cambiar de computadora o limpiar el navegador.
- Para pasar el cronograma a otro equipo: **Exporta** en uno e **Importa** en
  el otro.

---

## ❓ Preguntas frecuentes

**¿Necesito internet?** No. Funciona totalmente sin conexión.

**¿Se pierden los datos al cerrar?** No, se guardan solos. Solo se borrarían si
limpias los datos del navegador o pulsas "Borrar todos los datos".

**¿Puedo arrastrar bloques en el celular?** El arrastre está pensado para
mouse; en el teléfono usa un toque sobre el bloque para abrir el editor y
cambiar las horas desde ahí.

**¿Cómo lo comparto con mi pareja?** Envíale el archivo `cronograma.html` (y,
si quieres, un respaldo `.json` para que importe los mismos datos).
