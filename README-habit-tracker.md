# 📊 Rastreador de hábitos y progreso personal

Una aplicación web para hacer seguimiento diario de tus hábitos, inspirada en las
plantillas de "Habit Tracker" mensuales pero más avanzada e interactiva. Todo vive
en **un único archivo HTML** (`habit-tracker.html`): sin servidor, sin instalar nada.

> Los gráficos usan **Chart.js desde un CDN**, así que necesitan conexión a internet.
> Si abres el archivo sin red, los gráficos muestran un aviso pero **todo lo demás
> funciona igual**: casillas, rachas, análisis, mapa de calor, notas…

---

## ▶️ Cómo abrirlo

1. Descarga o localiza el archivo **`habit-tracker.html`**.
2. Haz **doble clic** sobre él: se abrirá en tu navegador (Chrome, Edge, Firefox, Safari…).
3. ¡Listo! Viene precargado con **julio de 2026** y 10 hábitos diarios que puedes
   cambiar cuando quieras desde el botón **⚙️ Hábitos**.

---

## ✨ Qué puedes hacer

| Función | Cómo se usa |
|---|---|
| **Marcar un hábito** | Clic en la casilla del día: verde ✓ = cumplido. Otro clic lo desmarca. |
| **Cambiar de mes** | Flechas ‹ › o el selector de mes y año de la barra superior. Cada mes guarda sus propios datos. |
| **Contadores globales** | Meta total, Completados, Restantes y media diaria, junto a la dona con el % del mes. |
| **Progreso diario y semanal** | Gráficos de barras con el % de cumplimiento por día y por semana. |
| **Estado mental** | En la cuadrícula, clic en las filas **Ánimo** (😞→😄) y **Motivación** (1→5); se dibujan como líneas a lo largo del mes. |
| **Correlación** | Un gráfico de dispersión muestra cómo se relacionan ánimo y motivación con tu % de hábitos, con el coeficiente `r` explicado. |
| **Rachas** | Cada hábito muestra su racha actual 🔥 y su récord 🏆 (días seguidos, o semanas si la meta es semanal). |
| **Mapa de calor** | Calendario estilo GitHub: vista global (intensidad = % del día) o por hábito. |
| **Análisis y TOP** | Tabla por hábito (Meta, Real, Restante, barra y %) y ranking de hábitos por cumplimiento. |
| **Metas flexibles** | Cada hábito puede ser **diario**, **X veces por semana** o de **días concretos**; el % se calcula según su meta real, no siempre sobre 31 días. |
| **Categorías y filtros** | Cada hábito tiene una categoría (Rutina, Mente, Cuerpo…); los chips de arriba filtran toda la vista. |
| **Notas y reflexiones** | Nota por día (fila 📝 de la cuadrícula), reflexión por semana y reflexión del mes. Se guardan solas. |
| **Histórico** | Comparación mes a mes del % global de cumplimiento, con gráfico y tabla. |
| **Modo claro / oscuro** | Botón 🌙/☀️; también sigue el tema del sistema. |
| **Exportar / Importar** | ⬇️ JSON guarda un respaldo completo; ⬆️ Importar lo recupera. 📄 CSV exporta la tabla de análisis para Excel/Sheets. |
| **Imprimir o PDF** | Botón 🖨️ o Ctrl+P: sale una vista limpia en claro, sin botones. |
| **Móvil** | Diseño responsive; la cuadrícula se desplaza horizontalmente con la columna de hábitos fija. |

---

## ⚙️ Cómo personalizarlo (sin programar)

Botón **⚙️ Hábitos** en la barra superior. Para cada hábito puedes cambiar:

- El **emoji**, el **nombre** y la **categoría** (escribe una nueva o elige una existente).
- La **meta**: `Diario`, `X veces por semana` (elige cuántas) o `Días concretos`
  (marca L M X J V S D).
- **🗑 Borrar** un hábito o **＋ Añadir** uno nuevo.

Los cambios se aplican al pulsar **Guardar cambios** y afectan a todos los meses.

---

## 🎨 Personalización avanzada (editando el archivo)

Abre `habit-tracker.html` con un editor de texto (Bloc de notas, VS Code…).
Todo el código está **comentado en español** y las zonas fáciles de tocar llevan
la marca **`>>> PERSONALIZAR <<<`**:

- La **paleta de colores** de los temas claro y oscuro (variables CSS al inicio).
- Los **hábitos iniciales** (función `habitosPorDefecto`) — solo se usan la
  primera vez que se abre la aplicación.
- El **mes inicial** (`mesVisto` dentro de `estadoPorDefecto`).

---

## 💾 Sobre tus datos y respaldos

- Los datos se guardan en el **almacenamiento local del navegador** (`localStorage`).
  Son privados y quedan solo en tu equipo.
- Conviene **exportar un respaldo `.json`** de vez en cuando (botón ⬇️), sobre todo
  antes de cambiar de computadora o limpiar el navegador.
- Para pasar tus datos a otro equipo o navegador: **Exporta** en uno e **Importa**
  en el otro.

---

## ❓ Preguntas frecuentes

**¿Necesito internet?** Solo para los gráficos (Chart.js viene de un CDN). Las
casillas, tablas, rachas, mapa de calor y notas funcionan sin conexión.

**¿Se pierden los datos al cerrar?** No: se guardan solos en el navegador. Solo se
borrarían si limpias los datos del navegador (por eso conviene exportar respaldos).

**Marqué un hábito de "días concretos" y algunas casillas están rayadas.** Las
casillas rayadas son días en los que ese hábito no está programado, y no cuentan
ni a favor ni en contra.

**¿Cómo funciona la racha de un hábito semanal?** Se cuenta en **semanas**: cada
semana que alcanzas la cuota (por ejemplo, 3 de 3) suma 1 a la racha.

**¿Puedo empezar en otro mes?** Sí: usa el selector de mes/año. Cada mes guarda
sus marcas, ánimo, notas y reflexiones por separado, y el histórico los compara.
