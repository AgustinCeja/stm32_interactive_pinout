# 🚀 STM32 Interactive Pinout 🇦🇷

¡Buenas! Hice este mapa interactivo sobre los pines de una **STM32F407VGTA6** debido a la necesidad que tenía de tener una referencia clara y precisa sobre los pines de la placa para otro proyecto.

---

## 📁 Estructura de Archivos

* `index.html`: El chasis de la aplicación y el motor visual.
* `pines.js`: La base de datos pura donde vive la información de cada pad.
* `STM32_V0.4.svg`: El diseño original vectorizado en Inkscape. Lo subo limpio (con sus capas y textos editables), por si alguien quiere usarlo de plantilla para otra placa.

---

## 🚀 Cómo usarlo

Es una herramienta local. No necesitás instalar nada, ni tener conexión a internet:
1. Descargás el repositorio (o te bajás el ZIP).
2. Hacés doble clic en `index.html`.
3. Listo, a jugar.

---

## 💡 Tip de Portabilidad (Versión Monolítica)

Si quisieran hacerlo 100% portable y que funcione con **un solo archivo**, pueden prescindir del archivo separado de datos siguiendo estos pasos:

1. Abran el archivo `pines.js`, copien todo su contenido.
2. Peguen esos datos dentro del `index.html`, abajo de todo, entre las etiquetas `<script> ... </script>` como primera línea de código (para que sea lo primero que llame el navegador).
3. Borren la línea de código `<script src="pines.js"></script>` que se encuentra arriba en el `index.html` antes de la etiqueta `<style>` (así evitan que la página intente llamar a un archivo externo que ya no necesitan).

