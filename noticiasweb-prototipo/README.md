# NoticiasWeb - Prototipo funcional

Prototipo web desarrollado con HTML, CSS y JavaScript puro a partir de los mockups de la Entrega 1.

## Funcionalidades

- Renderizado dinámico desde `data/noticias.json`.
- Navegación tipo SPA mediante hash routing.
- Buscador en tiempo real al enviar la consulta.
- Favoritos persistentes con `localStorage` y contador dinámico.
- Vista de inicio, listado, favoritos, detalle y contacto.
- Noticias relacionadas por categoría.
- Tiempo de lectura estimado.
- Formulario con validación de nombre, correo, asunto y mensaje.
- Diseño responsive para escritorio, tableta y móvil.

## Estructura

```text
noticiasweb-prototipo/
├── index.html
├── css/styles.css
├── js/app.js
├── data/noticias.json
├── .gitignore
└── README.md
```

## Ejecución local

El navegador bloquea `fetch()` al abrir el HTML directamente. Inicia un servidor local desde la carpeta del proyecto:

```bash
python -m http.server 5500
```

Después abre `http://localhost:5500`.

También puede usarse la extensión Live Server de Visual Studio Code.

## Publicación en GitHub

1. Crea un repositorio vacío en GitHub, por ejemplo `noticiasweb-prototipo`.
2. Desde esta carpeta ejecuta:

```bash
git init
git add .
git commit -m "Entrega prototipo funcional NoticiasWeb"
git branch -M main
git remote add origin URL_DEL_REPOSITORIO
git push -u origin main
```

3. Para GitHub Pages, abre **Settings > Pages**, selecciona **Deploy from a branch**, rama **main** y carpeta **/(root)**.

## Nota

El formulario valida la información en el navegador, pero no envía correo ni guarda datos en un servidor. Las imágenes proceden de URLs públicas de Unsplash y requieren conexión a Internet.
