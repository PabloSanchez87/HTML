# Favicon
- Un favicon (abreviatura de **favorite icon**) es un pequeño icono gráfico que representa un sitio web o una página web específica. 
- Se utiliza principalmente para identificar visualmente una página web en las pestañas del navegador, en los marcadores (favoritos) y en otras áreas del navegador donde se hace referencia al sitio web.

## Características de un Favicon
### Tamaño
- Generalmente, los favicons son pequeños, con un tamaño común de 16x16 píxeles. 
- Sin embargo, se pueden usar diferentes tamaños (32x32, 48x48, 64x64, etc.) para diferentes contextos y dispositivos.

### Formato
- Los formatos de archivo más comunes para favicons son ICO, PNG, GIF y SVG. 
- El formato ICO es el más tradicional, pero PNG es muy popular debido a su soporte para transparencia.

### Ubicación
- Los favicons se colocan normalmente en la raíz del directorio del sitio web 
    - `(/favicon.ico)`
    - También se pueden especificar en el código HTML.

## Cómo se Implementa un Favicon
- Para añadir un favicon a una página web, se utiliza la etiqueta `<link>` en el `<head>` del documento HTML. 
- Aquí hay algunos ejemplos de cómo hacerlo:

### Favicon en formato ICO
```html
<head>
    <link rel="icon" href="/favicon.ico" type="image/x-icon">
</head>
```

### Favicon en formato PNG
```html
<head>
    <link rel="icon" href="/favicon.png" type="image/png">
</head>
```

### Favicons en diferentes tamaños
- Para manejar diferentes dispositivos y tamaños de pantalla, se pueden especificar múltiples favicons de diferentes tamaños.
```html
<head>
    <link rel="icon" href="/favicon-32x32.png" sizes="32x32" type="image/png">
    <link rel="icon" href="/favicon-16x16.png" sizes="16x16" type="image/png">
</head>
```

## Importancia de los Favicons
- **Identificación Visual**
    - Ayudan a los usuarios a identificar rápidamente la página web entre múltiples pestañas abiertas.
- **Profesionalismo**
    - Un favicon bien diseñado contribuye a una imagen profesional del sitio web.
- **Accesibilidad**
    - Facilita el acceso a los favoritos y a la barra de direcciones.


## Crear un Favicon
- Para crear un favicon, se puede utilizar cualquier editor gráfico que permita guardar imágenes en los formatos requeridos (ICO, PNG, etc.). 
- Algunos pasos básicos son:
    - **Diseño**

            Crear un diseño simple y reconocible. Debido a su tamaño pequeño, es importante que el diseño sea claro y legible.

    - **Guardar** 
     
            Guardar el archivo en el formato y tamaño adecuados.

    - **Conversión**
        
            Si es necesario, convertir el archivo a formato ICO usando herramientas en línea o software especializado.

## Herramientas en Línea para Crear Favicons
- [Link favicon-generator](https://www.favicon-generator.org/)
    - Herramienta en línea que permite convertir imágenes en favicons.
- [Link real favicon generator](https://realfavicongenerator.net/)
    - Permite crear favicons en múltiples tamaños y obtener el código HTML necesario.
