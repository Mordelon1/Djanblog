# web2 — Sitio Djanter Capital con blog (27-09-2026)

## Qué hay aquí

| Archivo / carpeta | Qué es |
|---|---|
| `index.html` | Tu página actual, con el mismo diseño. Cambios: enlace **Blog** en el menú y el pie, sección "Blog" antes de las preguntas frecuentes, título y datos para Google, contacto escrito en el HTML, corrección de un error con "reducir movimiento" |
| `blog/index.html` | Portada del blog (listado de entradas) |
| `blog/people-analytics-para-pymes/index.html` | Primera entrada |
| `_plantilla/entrada.html` | Plantilla para nuevas entradas (Google no la indexa) |
| `robots.txt`, `sitemap.xml` | Para Google |
| `og-djanter.jpg` | Imagen que aparece al compartir en WhatsApp/LinkedIn |
| `favicon.ico`, `apple-touch-icon.png`, `logo-djanter-512.png` | Íconos y logo para Google |

## Cómo subirlo a GitHub

1. Sube **todo el contenido** de esta carpeta a la raíz del repo, reemplazando `index.html`.
2. **Arrastra las carpetas** `blog` y `_plantilla` (no uses "choose your files": no sube carpetas).
3. No borres tu `wrangler.jsonc` actual.
4. Comprueba: `tu-sitio/blog/` y `tu-sitio/blog/people-analytics-para-pymes/`.
5. En Search Console, envía `sitemap.xml`.

## Cómo agregar una entrada nueva

Lo más simple: pídeme el artículo y te entrego la carpeta lista, con el listado, la portada y el sitemap actualizados.

Si lo haces tú, las instrucciones están al inicio de `_plantilla/entrada.html`. En resumen:
1. Crea `blog/nombre-de-la-entrada/index.html` a partir de la plantilla.
2. Reemplaza los textos en MAYÚSCULAS y escribe el artículo.
3. Agrega la tarjeta en `blog/index.html` y en la sección Blog de `index.html`.
4. Agrega la dirección en `sitemap.xml`.
