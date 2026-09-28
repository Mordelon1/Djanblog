# Cómo subir esta versión a GitHub (paso a paso)

*Versión del 27-09-2026. Repositorio: `mordelon1/Djanblog`. Dominio: djantercapital.cl.*

## Qué NO se sube

| No subir | Por qué |
|---|---|
| `_interno/` | Documentos internos (este archivo y el plan SEO) |
| `desktop.ini` | Archivo que crea Windows; no sirve en la web |
| `LEEME.md` | Nota interna |

Todo lo demás de la carpeta `web2` sí se sube.

## Antes de subir: limpia lo antiguo en GitHub

En la versión anterior existía el archivo `_plantilla/entrada.html`. Ahora la plantilla está en `_plantilla/entrada/index.html`.

1. En GitHub, entra a la carpeta `_plantilla`.
2. Abre `entrada.html` → ícono de los tres puntos (…) → **Delete file** → **Commit changes**.

## Subir los archivos

1. Abre **github.com/mordelon1/Djanblog**.
2. Botón **Add file** → **Upload files**.
3. Abre en otra ventana tu carpeta `Documentos\Djanter\web2`.
4. Selecciona y **arrastra** a la página de GitHub:
   - las carpetas: `blog`, `capacitaciones`, `consultoria`, `descripcion-de-cargos`, `estudio-clima-laboral`, `evaluacion-psicolaboral`, `nosotros`, `people-analytics`, `privacidad`, `recursos`, `seleccion-de-personal`, `_plantilla`
   - los archivos: `index.html`, `404.html`, `robots.txt`, `sitemap.xml`, `og-djanter.jpg`, `favicon.ico`, `apple-touch-icon.png`, `logo-djanter-512.png`, `.nojekyll`
   
   > Importante: **arrastra**. El botón "choose your files" no sube carpetas.
   > `.nojekyll` es un archivo oculto. Si no lo ves en Windows: Explorador → **Vista** → **Mostrar** → **Elementos ocultos**. Si ya está en GitHub, no hace falta volver a subirlo.
5. Espera a que termine la lista de archivos (pueden ser más de 30).
6. Abajo, en **Commit changes**, escribe: `Nueva arquitectura: servicios, consultoría, recursos y blog`.
7. Pulsa **Commit changes**.

## Comprobar (espera 1 a 3 minutos)

Abre estas direcciones y revisa que se vean con diseño:

- https://djantercapital.cl/
- https://djantercapital.cl/seleccion-de-personal/
- https://djantercapital.cl/consultoria/ley-karin/
- https://djantercapital.cl/recursos/calculadora-costo-reemplazo/ (prueba cambiar un número)
- https://djantercapital.cl/recursos/indicadores-rrhh/ (prueba descargar el Excel)
- https://djantercapital.cl/blog/
- https://djantercapital.cl/una-pagina-que-no-existe/ (debe mostrar la página 404 de Djanter)

Si alguna se ve sin diseño o da error 404, casi siempre es una carpeta que no se subió: repite el paso 4 solo con esa carpeta.

## Avisar a Google (Search Console)

1. Entra a **search.google.com/search-console** → propiedad `djantercapital.cl`.
2. Menú **Sitemaps** → escribe `sitemap.xml` → **Enviar**. (Si ya estaba, vuelve a enviarlo: ahora tiene 26 direcciones.)
3. Menú **Inspección de URLs** → pega cada una de estas y pulsa **Solicitar indexación** (hay un límite diario; reparte en 2 o 3 días):
   1. https://djantercapital.cl/
   2. https://djantercapital.cl/seleccion-de-personal/
   3. https://djantercapital.cl/evaluacion-psicolaboral/
   4. https://djantercapital.cl/estudio-clima-laboral/
   5. https://djantercapital.cl/capacitaciones/
   6. https://djantercapital.cl/consultoria/
   7. https://djantercapital.cl/people-analytics/
   8. https://djantercapital.cl/descripcion-de-cargos/
   9. https://djantercapital.cl/recursos/calculadora-costo-reemplazo/
   10. https://djantercapital.cl/recursos/checklist-ley-karin/

## Cuando quieras una entrada nueva

Pídeme el artículo: te entrego la carpeta lista y los archivos que cambian (listado del blog, portada y sitemap). Si lo haces tú, las instrucciones están al inicio de `_plantilla/entrada/index.html`.
