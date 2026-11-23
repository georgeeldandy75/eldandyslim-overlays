# Overlays de @eldandyslim — TikTok LIVE Studio

Estos archivos HTML se copiaron de los cuatro archivos que proporcionaste, preservando su diseño y código. El paquete **no está publicado** en internet todavía.

## Archivos y tamaños recomendados de la fuente Enlace

| Archivo | Función | Ancho × alto |
|---|---|---|
| `noticias.html` | Cintilla editable | 1920 × 100 |
| `live.html` | Badge LIVE animado | 184 × 62 |
| `redes.html` | Seis redes sociales en deslizamiento | 342 × 116 |
| `top-likers.html` | Top Likers desde TikFinity | 230 × 188 |

## Publicar con GitHub Pages

1. Crea un **repositorio nuevo y público**, por ejemplo `eldandyslim-overlays`. No uses un repositorio privado de otros proyectos.
2. Sube **el contenido de esta carpeta** a la raíz del repositorio (`index.html`, `noticias.html`, etc.). También puedes subir los archivos usando la interfaz de GitHub.
3. Abre **Settings → Pages** en el repositorio y selecciona **Deploy from a branch**, rama `main`, carpeta `/ (root)`; guarda.
4. Una vez que GitHub publique la página, la base será `https://TU_USUARIO.github.io/eldandyslim-overlays/` (cambia `TU_USUARIO` por tu usuario real y usa el nombre real del repositorio).
5. En TikTok LIVE Studio agrega una Fuente **Enlace** por overlay, con URL directa `.../live.html`, `.../redes.html`, `.../noticias.html` o `.../top-likers.html`. Configura ancho y alto según la tabla.
6. Si tu fuente no ofrece tamaño exacto, ajusta sus propiedades y escala/recorta en la escena. Si modificas un HTML, vuelve a subirlo al repositorio y actualiza la fuente para borrar la caché.

## Editar contenido

- `noticias.html`: busca `const CONFIG` para modificar `titulo`, `mensajes`, `velocidad`, colores.
- `top-likers.html`: busca `--ancho-overlay`, `escalaTikfinity` y `urlWidgetPublico`. Si cambias el ancho, usa el mismo en TikTok LIVE Studio.
- `live.html`: busca variables CSS en `:root`, para tamaños y colores. El archivo recibido tiene panel oscuro *dentro del badge*, pero transparencia alrededor.
- `redes.html`: conserva la secuencia y el nombre `@eldandyslim` del original.

## Privacidad y compatibilidad

**Atención:** el archivo `top-likers.html` contiene una URL de widget TikFinity ya configurada en el archivo que enviaste. Si publicas este paquete en GitHub Pages, cualquier persona podrá inspeccionar ese enlace en el código fuente. Confirma que se trata de una URL pública destinada a incrustarse; si no, elimina el valor antes de publicar o utiliza la fuente Enlace de TikFinity por separado. Nunca publiques cookies, contraseñas o claves API.

La fuente externa de TikFinity usa un `iframe`: su carga y tamaño dentro de TikTok LIVE Studio no se pueden garantizar sin pruebas en tu cuenta. Los otros tres overlays son HTML/CSS/JS autónomos y no requieren TikFinity.

Si posteriormente agregas Top Gifters, súbelo como `top-gifters.html` y agrégalo a `index.html`.
