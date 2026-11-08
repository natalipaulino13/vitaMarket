# VitaMarket

**VitaMarket** es el prototipo de un supermercado online para personas con necesidades alimentarias específicas: productos veganos, vegetarianos, sin gluten, sin lactosa, ecológicos y de nutrición deportiva. Reúne estos productos en un solo lugar y muestra de forma clara sus ingredientes, alérgenos e información nutricional, para que cada persona pueda comprobar si un producto es apto antes de comprarlo.

Práctica AC2.1 «Diseña y construye tu web» del ciclo DAW. Desarrollada con HTML y CSS, sin JavaScript.

## Web publicada

🔗 https://natalipaulino13.github.io/vitaMarket/

## Páginas y recorrido recomendado

| Página | Archivo | Contenido |
|---|---|---|
| Inicio | `index.html` | Qué es VitaMarket, atajos por tipo de dieta y productos destacados |
| Catálogo | `catalogo.html` | Buscador, filtros, 6 productos y paginación |
| Detalle | `detalle.html` | Ficha de la proteína vegana: ingredientes, alérgenos e información nutricional |
| Carrito | `carrito.html` | Productos seleccionados, cantidades, subtotales y total |
| Acceso | `login.html` | Inicio de sesión de demostración |
| Formulario | `formulario.html` | Datos de entrega del pedido |

**Recorrido recomendado:**

1. **Inicio** → pulsa «Ver catálogo».
2. **Catálogo** → en la tarjeta de la proteína vegana, pulsa «Ver detalle».
3. **Detalle** → consulta la ficha y pulsa «Ver mi carrito».
4. **Carrito** → pulsa «Continuar con la entrega».
5. **Acceso** → introduce un correo y una contraseña inventados (mínimo 8 caracteres) y pulsa «Acceder y continuar».
6. **Formulario** → rellena los datos de entrega con datos ficticios y pulsa «Solicitar entrega».

## Abrir el proyecto en local

1. Clona el repositorio: git clone https://github.com/natalipaulino13/vitaMarket.git

2. Abre la carpeta `vitaMarket` y haz doble clic en `index.html` para verlo en el navegador.

No necesita instalación ni servidor: todas las rutas son relativas.

## Funciones representadas pero no implementadas

Es un **prototipo educativo**: no se realizan compras, pagos ni envíos reales. Estas funciones aparecen en la interfaz pero no funcionan, y cada página lo indica con un aviso visible:

- **Acceso:** no hay autenticación real. El formulario solo comprueba el formato del correo y la longitud de la contraseña.
- **Buscador, filtros y paginación del catálogo:** no modifican los resultados.
- **Atajos por tipo de dieta del inicio:** llevan al catálogo completo, sin aplicar el filtro.
- **Añadir al carrito, cambiar cantidades y eliminar productos:** no modifican el carrito ni los importes.
- **Carrito:** los productos y los importes son datos de ejemplo escritos en el HTML.
- **Formulario de entrega:** la validación funciona, pero la solicitud no se envía ni se guarda.
- **Fichas de producto:** solo la proteína vegana tiene página de detalle. El resto de tarjetas lo indican con «Ficha no disponible en el prototipo».

Todos los datos son ficticios.

## Dónde se utilizan Flexbox y Grid

**Flexbox**

| Componente | Uso |
|---|---|
| Cabecera y menú | Logo a la izquierda y menú a la derecha (`justify-content: space-between`) |
| Grupos de botones | `.acciones`, con `flex-wrap: wrap` |
| Atajos por tipo de dieta | 4 cajas en fila con la misma altura (`flex: 1`) |
| Tarjetas de producto | Contenido en columna (`flex-direction: column`) |
| Etiquetas | `.etiquetas`, con `flex-wrap: wrap` |
| Filas del carrito | Datos de cada producto, con `flex-wrap: wrap` |
| Pasos del pedido, paginación, migas de pan y pie | Elementos en fila |

**Grid**

| Componente | Uso |
|---|---|
| Catálogo | Rejilla de tarjetas con `repeat(auto-fill, minmax(200px, 1fr))` y `gap` |
| Productos destacados | 4 columnas. La tarjeta destacada ocupa 2 columnas y 2 filas (`span 2`) |
| Presentación del inicio | Áreas con nombre: `"texto imagen"` |
| Detalle de producto | Áreas con nombre: `"imagen info" / "texto nutricion"` |
| Catálogo, carrito y formulario | Columna principal + columna lateral (filtros o resumen del pedido) |

## Documentación de diseño y comprobación

| Documento | Contenido |
|---|---|
| [Análisis de usuarios y usabilidad](docs/analisis.md) | Propósito, usuarios, contexto, tareas, recorrido e información necesaria |
| [Bocetos](docs/bocetos/) | Bocetos de las seis páginas |
| [Revisión de los bocetos](docs/revision-bocetos.md) | Revisión con una compañera y decisiones sobre sus sugerencias |
| [Comprobaciones con DevTools](docs/comprobaciones-devtools.md) | Cascada, modelo de caja y Grid en el inspector |
| [Comprobación de accesibilidad](docs/accesibilidad.md) | Tabla de comprobación con evidencias de teclado y foco, contraste y ampliación al 200 % |
| [Comprobación a 1024 y 1440 px](docs/anchuras.md) | Comportamiento en las dos anchuras de referencia |
| [Prueba final de usabilidad](docs/prueba-final.md) | Prueba con una compañera y cambios realizados después |

## Procedencia de imágenes y recursos

- **Ilustraciones de productos, imagen de la presentación e iconos** (`img/`): ilustraciones SVG originales creadas con Claude (IA de Anthropic) para este proyecto.
- **Bocetos** (`docs/bocetos/`): diseñados en SVG con ayuda de Claude.
- **Capturas de pantalla** (`docs/`): realizadas por mí en Google Chrome sobre la web publicada. Las flechas y explicaciones se añadieron con ayuda de Claude.
- **Tipografía:** Arial, fuente del sistema. No se usan fuentes ni recursos externos.

## Herramientas de IA utilizadas

He utilizado **Claude** (Anthropic) como asistente durante el desarrollo. Así he repartido el trabajo:

**Lo que he hecho yo:**

- La idea del proyecto, el primer borrador del análisis de usuarios y las tareas principales.
- Las decisiones de diseño: elegir los perfiles de usuario, el formulario de entrega, qué página tiene ficha de detalle y qué sugerencias de la revisión incorporar o descartar.
- La primera versión del HTML de la presentación y de los atajos por tipo de dieta del inicio, y del CSS de la cabecera y el menú, que después revisé con Claude.
- La creación del repositorio, los commits y la publicación en GitHub Pages.
- Todas las pruebas sobre la web publicada: navegación con teclado, contraste, ampliación al 200 %, anchuras de 1024 y 1440 px y las comprobaciones con DevTools, incluidas las capturas.
- La revisión de los bocetos y la prueba final con mi compañera.
- Detectar problemas durante las pruebas (el ancho de las tarjetas del catálogo, los atajos al ampliar, el mensaje de error del teléfono, el texto de la paginación) y comprobar que las correcciones funcionaban.

**En lo que me ha ayudado Claude:**

- Explicarme la teoría de cada fase: HTML semántico, cascada, herencia, modelo de caja, Flexbox, Grid, accesibilidad y Git.
- Revisar mi código y mis textos y proponer correcciones.
- Proponer el código HTML y CSS del resto de páginas a partir de los bocetos y de mis decisiones. Yo lo he revisado, probado en el navegador y corregido cuando algo fallaba.
- Diseñar los bocetos y crear las ilustraciones SVG.
- Añadir anotaciones a las capturas y calcular los contrastes de color.
