# Reflexión — Decisiones de CSS

## Grid para las tarjetas de películas, Flexbox para todo lo demás

Usé **CSS Grid** para `.movie-grid` y `.team-grid`, pero **Flexbox** para el header, el formulario de búsqueda y el formulario de registro. La diferencia no es arbitraria: las tarjetas de película son una colección de elementos del mismo tipo que necesita alinearse en **dos dimensiones** a la vez (filas y columnas deben quedar parejas cuando hay 3 tarjetas por fila en desktop), mientras que el header y los formularios son secuencias de elementos en **una sola dirección** (una fila de navegación, o una columna de campos de formulario).

Si hubiera usado Flexbox para las tarjetas de películas con `flex-wrap: wrap`, el resultado habría sido que la tercera tarjeta de la última fila incompleta se estirara o quedara desalineada respecto a las columnas de la fila de arriba, porque Flexbox no sabe nada sobre la fila anterior — cada fila se ajusta de forma independiente. Con `grid-template-columns: repeat(3, 1fr)`, en cambio, las columnas quedan definidas de una sola vez para todo el contenedor, así que aunque falte una tarjeta para completar la fila, las que sí existen se mantienen alineadas con las columnas de arriba. Elegí Grid específicamente por eso: necesitaba que la cuadrícula se comportara como una cuadrícula real, no como una fila que se envuelve.

Para el header, en cambio, Flexbox fue la opción correcta porque solo necesito distribuir el logo y la navegación en un eje (`justify-content: space-between` en desktop), sin preocuparme por alinear columnas con ninguna otra fila — ahí Grid habría sido una herramienta más compleja de la que el problema realmente pedía.
