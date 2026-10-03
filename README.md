# Jade-Games

Sitio estático publicado con GitHub Pages. La página principal es `index.html` y la etiqueta NFC debe apuntar a la URL estable del sitio.

## Agregar un juego

1. Coloca en `games/` una ROM que tengas derecho a alojar. Para Zelda: The Minish Cap, el nombre esperado es `games/zelda-minish-cap.gba`.
2. En `index.html`, agrega el identificador, el core y la ruta en el objeto `games`.
3. Configura la etiqueta NFC con la URL del juego. La página no muestra un selector de juegos.
4. Publica los cambios del repositorio.

## URLs para las etiquetas

- Mario: `https://irustub.github.io/` (también acepta `?game=mario`).
- Zelda: `https://irustub.github.io/?game=zelda`.

La página valida que exista el archivo solicitado y no carga otro juego como sustituto.

La página carga EmulatorJS desde `https://cdn.emulatorjs.org/stable/data/`; por tanto, la página y los juegos pueden estar en este repositorio, pero los archivos del emulador todavía se sirven desde el CDN. Para que todo sea del mismo origen habría que alojar también esa distribución en el proyecto.

No publiques ROMs protegidas por derechos de autor sin autorización. Los archivos de `games/` de un sitio público quedan accesibles para cualquier visitante.