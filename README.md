# AppleCheck — detector de estado de manzanas

Frontend estático para clasificar fotografías de manzanas como **buen estado** o **deterioradas**.

## Funcionamiento

El archivo original `project.tm` contiene 20 imágenes de entrenamiento (11 buenas y 9 deterioradas), pero no incluye los pesos exportados de un modelo de Teachable Machine. Para que el proyecto pueda ejecutarse directamente en GitHub Pages, esta versión:

- extrae 74 características visuales de cada imagen (color, HSV, brillo, proporciones y textura);
- normaliza esas características con el conjunto de entrenamiento;
- usa k-NN (`k = 3`) para estimar la clase;
- ejecuta todo localmente en el navegador.

## Uso

Abre `index.html`, carga una imagen y pulsa **Analizar imagen**. También puedes usar las cuatro imágenes de muestra integradas.

> Proyecto académico/experimental. La predicción no sustituye una inspección real de la fruta.
