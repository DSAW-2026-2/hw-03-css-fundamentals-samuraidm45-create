# HW03 — CSS Fundamentals

Semana 3 · DSAW · Universidad de La Sabana

## Objetivo

Diseñar y mejorar la landing page de CineHub utilizando CSS puro y hacer que la página sea responsive sin utilizar librerías externas.

## Estructura del proyecto

El proyecto está organizado de la siguiente manera:

- `index.html` — Página principal de CineHub.
- `about.html` — Página de información del proyecto y del equipo.
- `styles/main.css` — Estilos principales de la página.
- `styles/responsive.css` — Reglas responsive para móvil, tablet y desktop.
- `REFLECTION.md` — Reflexión sobre las decisiones tomadas en CSS.
- `AI-LOG.md` — Bitácora sobre el uso de inteligencia artificial durante el desarrollo.

## CSS

Los estilos están separados en dos archivos.

### `styles/main.css`

Contiene los estilos base de la aplicación:

- Tipografía.
- Colores.
- Espaciado.
- Box model.
- Botones y formularios.
- Tarjetas de películas.
- Header y navegación.
- Footer.
- Sección de preguntas frecuentes.

### `styles/responsive.css`

Contiene las reglas para adaptar la página a diferentes tamaños de pantalla:

- Mobile: menos de 640px.
- Tablet: entre 640px y 1024px.
- Desktop: más de 1024px.

La página utiliza CSS Grid y Flexbox para organizar sus diferentes secciones.

## FAQ

La sección de preguntas frecuentes utiliza un acordeón realizado solamente con CSS.

No se utiliza JavaScript.

El funcionamiento se consigue utilizando el selector `:target`, haciendo que cada pregunta enlace a un elemento mediante su `id`.

## Responsive Design

La página cambia su distribución dependiendo del tamaño de la pantalla.

En dispositivos móviles las tarjetas se muestran en una sola columna y la navegación se organiza verticalmente.

En tablets las tarjetas utilizan dos columnas.

En pantallas grandes las tarjetas utilizan tres columnas y se aumenta el espacio disponible para el contenido.

## Tecnologías utilizadas

- HTML5
- CSS3
- CSS Grid
- Flexbox
- Media Queries
- Selector `:target`

No se utilizaron librerías CSS externas.

## Despliegue

El proyecto se despliega utilizando GitHub Pages.

No requiere ningún proceso de compilación.

## Autograding

El proyecto debe cumplir con los siguientes criterios:

- Estructura de archivos correcta.
- HTML y CSS sin errores.
- Uso de Flexbox o Grid.
- Diseño responsive.
- Breakpoint para mobile menor a 640px.
- Breakpoint para tablet entre 640px y 1024px.
- Acordeón CSS-only utilizando `:target`.
- No utilizar JavaScript para el acordeón.
- Página publicada públicamente mediante GitHub Pages.

## Entrega

La página debe estar desplegada públicamente en GitHub Pages para poder ser evaluada.