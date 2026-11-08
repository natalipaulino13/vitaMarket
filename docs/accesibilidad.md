# Comprobación de accesibilidad

Revisión parcial realizada sobre la web publicada en GitHub Pages con Google Chrome. No permite afirmar que la web cumple WCAG A, AA o AAA.

## Tabla de comprobación

| Aspecto | Página o elemento revisado | Método utilizado | Resultado | Corrección realizada o problema pendiente |
|---|---|---|---|---|
| Estructura: idioma | Las 6 páginas | Revisión del código | Todas tienen `lang="es"` | Ninguna |
| Estructura: título | Las 6 páginas | Revisión del código y pestaña del navegador | Cada página tiene un `<title>` descriptivo y distinto | Ninguna |
| Estructura: encabezados | Las 6 páginas | Revisión del código | Un solo `h1` por página y sin saltos de nivel (h1 → h2 → h3) | Ninguna |
| Imágenes | Las 6 páginas | Revisión del código | Las imágenes informativas tienen `alt` descriptivo. Los iconos de «Compra según tu dieta» y las imágenes del carrito tienen `alt=""` porque el texto de al lado ya da la información | Ninguna |
| Formularios: etiquetas | Catálogo, detalle, carrito, acceso y formulario | Revisión del código y clic en cada etiqueta | Todos los campos tienen `<label for>` visible y asociado. Al pulsar la etiqueta se activa el campo | Ninguna |
| Formularios: agrupaciones e instrucciones | Catálogo y formulario | Revisión visual y del código | Filtros y formulario agrupados con `fieldset` y `legend`. Teléfono, código postal, fecha e instrucciones tienen indicación asociada con `aria-describedby`. El `placeholder` solo es un ejemplo, nunca sustituye a la etiqueta | Ninguna |
| Teclado | Las 6 páginas y recorrido completo de compra | Navegación solo con Tab, Mayús + Tab, Enter, Espacio y flechas | Se llega a todos los enlaces, botones y campos, y se pueden usar. No hay trampas de teclado | Ninguna |
| Foco | Las 6 páginas | Navegación con Tab | El foco se ve siempre (contorno azul `#1a4fa3` de 3 px; blanco en el pie, sobre fondo oscuro). El orden sigue el orden de lectura | Ninguna |
| Uso del color | Menú, pasos del pedido, paginación y etiquetas | Revisión visual | La página y el paso actuales se marcan con negrita y línea, no solo con color. Las etiquetas llevan ✓ y texto | Ninguna |
| Contraste | *(pendiente)* | | | |
| Ampliación al 200 % | *(pendiente)* | | | |

## Evidencias

### Teclado y foco

![Foco visible en el botón «Ver catálogo» y página actual marcada en el menú](accesibilidad/01-foco-navegacion.png)

![Foco visible en el campo Teléfono con su etiqueta e instrucción](accesibilidad/02-foco-formulario.png)

### Contraste

*(pendiente)*

### Ampliación al 200 %

*(pendiente)*