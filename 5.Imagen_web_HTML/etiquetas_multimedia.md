# Etiquetas multimedia

## Etiquetas de contenido incrustado
- Normalmente se usarán para cargar contenido externo.
- También se puede cargar contenido de la misma web.
- Es una referencia a un recurso almacenado en otra ubicación
- Al estar enlazado, garantiza que si el original cambia, nuestra web mostrará la versión actualizada.
- Podemos incrustar contenido como objetos multimedia, bloques de código HTML con contenidos diseñados por terceros e incluso webs enteras.
- Usaremos dos tipos de etiquetas:
    - `<embed>`
    - `<iframe>`

## Etiqueta `<embed>` (desuso)
- Podemos incrustar casi cualquier tipo de recurso.
    - Documentos html -> mejor usar `<iframe>`
    - Imágenes -> mejor usar `<img>`
    - Vídeos -> mejor usar `<videp>`
    - Audio -> mejor usar `<audio>`
    - Flash -> En desuso.
    - Controles ActiveX
### Atributos
- `src`: la URI del recurso que será incrustado y reproducido o ejecutado por el pulg-in.
- `type`: tipo de contenido (también conocido como tipo de medio de internet o tipo MIME)
- `width` y ` height`: determinan el tamaño del contenedor en el que se va a mostrar el contenido.

- [Ver documentación `<embed>` W3C](https://www.w3schools.com/tags/tag_embed.asp)

## Etiqueta `<iframe>`
- Representa un contexto de navegación anidado.
- Es una ventana que permite acceder a un recurso que se encuentra ubicado en un contexto distinto a la página que se está mostrando en el navegador.
- Básicamente, permite incrustar un documento o parte de un documento dentro de una página HTML.

### Atributos
- `src`: la URI del recurso incrustado.
- `sredoc`: contiene el código HTML que mostrar dentro del elemento `<iframe>`. Si existe este atributo, se impone a la referencia proporcionada por el atributo src.
- `sandbox`: permite proporcionar restricciones al documento incrustado en el elemento `<iframe>` con objeto de mejorar la seguridad de la página.
- `<allow>`: directivas referentes a permisos de acceso o determinados elementos del dispositivo físico, tales como el acelerómetro, la cámara o la geolocalización.
- `<allowfullscreen>`: si existe, permite al contenido incrustado ocupar la pantalla completa.
- `<width y height>`: permite indicar el ancho y el alto en píxeles.
- `<loading>`: con el valor `lazy` el contenido se carga cuando se haga visible, con el valor `eager`(valor por defecto) el contenido se cargará inmediatamente.

>![NOTE]
> ¿Pero qué ocurre si queremos colocar contenido de una web externa?
> Por ejemplo, servicios como Youtube, Vimeo, SoundCloud, SlideShare u otros sitios similares.
> Se trata de servicios que ofrecen contenido externo para incrustar en nuestras páginas web, pero lo que nos proporcionan no son imágenes, video o audios en formato que reconozca el navegdor, sino un enlace con contenido HTML muy diverso, que puede incluir JavaScript, CSS, imágenes , videos y muchos otros recursos.

#### Content - Security - Policy (CSP)
- El CSP es una medida de protección que se activa en los servidores del sitio web, en el cual se acepta o rechaza determinados llamados que vienen desde fuera, como interacciones entre servicios.
- Establece que un sitio web pueda o no ser embebida en otro sitio web.
- [Ver documentación CSP W3C](https://www.w3.org/TR/CSP3/)

---
#### Ejemplos


- [Ver código iframe externo](html/iframe/ejercicio4.html)

- [Ver código iframe interno](html/iframe/ejercicio5.html)

- [Ver código iframe Youtube](html/iframe/ejercicio6.html)

- [Ver código iframe Google Maps](html/iframe/ejercicio6.html)
---





