# 🗓️ Cronograma semanal para dos personas

Una aplicación web sencilla para planear y comparar las rutinas semanales de dos
personas (por defecto **Ana** y **Jeronimo**). Todo vive en un **único archivo
HTML autónomo**: no necesita internet, ni servidor, ni instalar nada.

---

## ▶️ Cómo abrirlo

1. Descarga o localiza el archivo **`cronograma.html`**.
2. Haz **doble clic** sobre él. Se abrirá en tu navegador (Chrome, Edge, Firefox,
   Safari…).
3. ¡Listo! Ya puedes empezar a usarlo.

> No hace falta conexión a internet. Puedes usarlo sin problema estando sin red.

---

## ✨ Qué puedes hacer

| Función | Cómo se usa |
|---|---|
| **Ver la semana completa** | Lunes a Domingo, con una línea de tiempo por día. |
| **Comparar dos rutinas** | Cada día tiene dos carriles lado a lado, uno por persona. |
| **Añadir un bloque** | Botón **➕ Añadir bloque**, o haz clic sobre un hueco vacío del día/persona. |
| **Editar o eliminar** | Haz clic sobre un bloque ya creado. |
| **Duplicar un bloque** | Dentro de la edición del bloque, botón **⧉ Duplicar**. |
| **Copiar un día a toda la semana** | Botón **📋 a semana** en la cabecera de cada día. |
| **Ver tiempo libre juntos** | Las franjas en las que **ambos** están libres se resaltan en verde ("Libres juntos"). Ideal para planear tiempo en pareja. |
| **Guardado automático** | Todo se guarda solo en el navegador. Al cerrar y volver a abrir, tus datos siguen ahí. |
| **Exportar / Importar** | Botones **⬇️ Exportar** (guarda un respaldo `.json`) y **⬆️ Importar** (recupera un respaldo). |
| **Imprimir o guardar en PDF** | Botón **🖨️ Imprimir / PDF**: se genera una vista limpia sin botones. |
| **Móvil** | El diseño se adapta: en el teléfono los días se apilan uno debajo de otro. |

---

## ⚙️ Cómo personalizarlo (sin programar)

Abre el botón **⚙️ Configuración** en la parte superior. Desde ahí puedes cambiar:

- **Los nombres** de las dos personas.
- El **rango horario visible** del día (por defecto **5:30 a 22:30**).
- La **granularidad** de los bloques: **30 o 60 minutos** (por defecto 30).
- Las **categorías** de actividad y su **color**: puedes añadir, renombrar,
  cambiar el color o eliminar categorías.

Los cambios se aplican y se guardan al pulsar **Guardar cambios**.

### Categorías por defecto

Trabajo · Ejercicio · Comidas · Sueño · Tareas del hogar · Tiempo personal ·
Tiempo en pareja · Otros

---

## 🎨 Personalización avanzada (opcional, editando el archivo)

Si te animas a abrir `cronograma.html` con un editor de texto, encontrarás
comentarios en español y varias marcas **`>>> PERSONALIZAR <<<`** que señalan las
zonas fáciles de tocar, por ejemplo:

- La **paleta de colores** de la interfaz (al inicio, dentro de `:root`).
- La **altura de los bloques** (variable `--px-por-minuto`: súbela para bloques
  más altos, bájala para una vista más compacta).
- Los **valores por defecto** (función `configPorDefecto`), que se usan si alguna
  vez pulsas "Borrar todos los datos".

---

## 💾 Sobre tus datos y respaldos

- Los datos se guardan en el **almacenamiento local del navegador**
  (`localStorage`). Son privados y quedan en tu equipo.
- Como están ligados a ese navegador, conviene **exportar un respaldo `.json`**
  de vez en cuando (botón **⬇️ Exportar**), sobre todo antes de cambiar de
  computadora o de limpiar el navegador.
- Para pasar el cronograma a otro equipo: **Exporta** en uno e **Importa** en el
  otro.

---

## ❓ Preguntas frecuentes

**¿Necesito internet?** No. Funciona totalmente sin conexión.

**¿Se pierden los datos al cerrar?** No, se guardan solos. Solo se borrarían si
limpias los datos del navegador o pulsas "Borrar todos los datos".

**¿Puedo usarlo en el celular?** Sí, ábrelo en el navegador del teléfono. También
puedes exportar el `.json` y abrirlo en otro dispositivo importándolo.

**¿Cómo lo comparto con mi pareja?** Envíale el archivo `cronograma.html` (y, si
quieres, un respaldo `.json` para que tenga los mismos datos e lo importe).
