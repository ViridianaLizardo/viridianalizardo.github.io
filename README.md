# viridianalizardo.github.io

Sitio personal hecho con [Quarto](https://quarto.org). Se publica solo con cada `push` a `main`.

## Primera vez

1. Crea en GitHub el repo **`viridianalizardo.github.io`** (público) y sube esta carpeta.
2. En el repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. Espera 1–2 min (pestaña *Actions*) y abre <https://viridianalizardo.github.io>.

Para verlo en tu PC antes de subir: en RStudio abre el proyecto y corre `quarto preview` en la Terminal
(ahí sí se ven los borradores `draft: true`).

## Qué se toca para qué

| Quiero… | Archivo |
|---|---|
| Cambiar el "sobre mí" o el bloque de CV | `index.qmd` |
| Subir el CV | `cv/cv-es.pdf` y `cv/cv-en.pdf` (mismos nombres) |
| Escribir en el blog | copia `posts/2026-09-29-hola-jardin/` con otra fecha y nombre, edita `index.qmd` |
| Agregar un libro, obra o cuento (Letras) | copia `letras/mi-primer-libro/` |
| Agregar un artículo (Ciencia) | pégalo en APA bajo su año en `ciencia.qmd` |
| Agregar un tutorial | 4–6 líneas en `tutoriales.yml` |
| Agregar una curiosidad | 4–6 líneas en `curiosidades.yml` |
| Una curiosidad de un solo archivo HTML | `experimentos/nombre/index.html` y en `curiosidades.yml` pon `path: experimentos/nombre/` |
| Colores | bloque **PALETA** al inicio de `estilos.scss` |
| Menú, nombre, lema | `_parciales/cabecera.html` |
| Botones 88×31 del pie | `_parciales/pie.html` |

Notas:

- **Borradores:** `draft: true` en el encabezado de un post o ficha = no se publica. Quítalo para publicarlo.
- **Blog estilo tumblr:** lo que pongas en `description:` se ve completo en la lista. Si la entrada es corta, basta con eso.
- **Posts con código R:** renderízalos en tu PC (`quarto render posts/…/index.qmd`) y sube también la carpeta `_freeze/`. GitHub no tiene R instalado.
- **GIFs y pixel art:** guárdalos en `imagenes/` (o en la carpeta del post) y úsalos como `image:` en posts, fichas, tutoriales o curiosidades.
- **Cursor propio:** instrucciones al final de `estilos.scss`.
