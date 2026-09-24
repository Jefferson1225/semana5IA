# AppleCheck — detector de estado de manzanas

Frontend estático para clasificar fotografías de manzanas como **buen estado** o **deterioradas**.

## Funcionamiento

El archivo original `project.tm` contiene 20 imágenes de entrenamiento (11 buenas y 9 deterioradas), pero no incluye los pesos exportados de un modelo de Teachable Machine. Para poder ejecutarlo directamente en GitHub Pages, esta versión:

- extrae 74 características visuales por imagen (color, HSV, brillo y textura);
- normaliza esas características con el conjunto del proyecto;
- usa un clasificador logístico ligero calibrado con esas 20 imágenes;
- ejecuta todo localmente en el navegador: las fotos no se suben a un servidor.

## Uso

Abre la web, carga una imagen y pulsa **Analizar imagen**. También puedes probar las cuatro imágenes de muestra incluidas.

> Proyecto académico/experimental. Con un conjunto tan pequeño, la predicción puede fallar con otros fondos, iluminaciones o variedades de manzana.
