# Mi Blog — Actividad 1 (HTML + CSS + JS)

Proyecto de blog 100% estático construido con HTML, CSS (Bootstrap) y JS. La lista de entradas se carga desde `posts.json` y se renderiza en `index.html`. Incluye un buscador simple por título y extracto.

## URL de Producción

Reemplaza este placeholder con la URL real una vez desplegado:

- Producción: https://arvmirez-unipro.github.io/desarrollo_aplicaciones_actividad_1/

## Estructura del proyecto

```
.
├── index.html            # Página principal: lista y buscador
├── app.js                # Lógica para cargar y filtrar posts
├── posts.json            # Metadatos de las entradas (title, date, slug, excerpt)
├── posts/
│   ├── mi-primer-post/
│   │   └── index.html
│   └── otro-post/
│       └── index.html
└── favicon.svg
```

## Cómo funciona
- `index.html` incluye Bootstrap desde CDN y un input de búsqueda.
- `app.js` hace `fetch('posts.json')`, ordena por fecha descendente y renderiza tarjetas con enlaces a cada post (`/posts/{slug}/`).
- El buscador filtra por coincidencias en título y extracto en tiempo real.