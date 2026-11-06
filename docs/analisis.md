# VitaMarket: análisis de usuarios y usabilidad

## 1. Nombre y propósito

**VitaMarket** es un supermercado online especializado en productos para personas con necesidades alimentarias específicas: productos veganos, vegetarianos, sin gluten, sin lactosa, ecológicos y de nutrición deportiva.

Resuelve el problema de tener que visitar varias tiendas para encontrar estos productos y de no poder comprobar con facilidad si un producto es apto. VitaMarket los reúne en un mismo lugar y muestra de forma clara sus ingredientes, alérgenos e información nutricional.

## 2. Usuarios

Todos los perfiles están acostumbrados a comprar online, pero no conocen la tienda la primera vez que entran. Por eso, la página de inicio debe explicar claramente qué es VitaMarket.

| Perfil | Qué sabe | Qué le preocupa | Cómo afecta al diseño |
|---|---|---|---|
| **Persona celíaca o con intolerancia a la lactosa** | Lee etiquetas y alérgenos con mucha atención | Estar totalmente segura de que el producto es apto, incluidas las trazas | Alérgenos muy visibles en el detalle, filtro por "sin gluten" y "sin lactosa" |
| **Persona vegana** | Conoce qué ingredientes son de origen animal | Que no haya ingredientes animales poco evidentes | Lista de ingredientes completa, etiqueta "vegano", filtro por tipo de dieta |
| **Deportista** | Conoce las proteínas y los suplementos y compara entre marcas | La cantidad de proteína por ración y el precio | Tabla nutricional, precio y cantidad juntos para poder comparar |

## 3. Contexto de uso

Esta primera versión de la web está pensada principalmente para **ordenador** y se ha comprobado con anchuras de 1024 y 1440 px. La adaptación a móvil se desarrollará en la siguiente práctica.

La mayoría de los usuarios comprará **desde casa**, aunque algunos consultarán productos desde el trabajo, en un descanso, con poco tiempo y posibles interrupciones.

El tiempo disponible varía:

- Quien repite compra quiere **encontrar rápido** productos que ya conoce, por eso hay buscador y filtros.
- Quien prueba un producto nuevo dedica **más tiempo** a comparar ingredientes y valores nutricionales, por eso el detalle debe ser completo y ordenado.

Las características de los productos (vegano, sin gluten, sin lactosa…) se mostrarán con **etiquetas que incluyen texto**, no solo color, para que cualquier persona pueda identificarlas, incluidas las personas con dificultades para distinguir colores.

## 4. Tareas principales

1. Encontrar una **pasta sin gluten** en el catálogo y comprobar en su ficha que no contiene trazas de gluten.
2. Encontrar una **proteína vegana en polvo** y consultar en su ficha los ingredientes, la proteína por ración y el precio para decidir si le conviene.
3. **Revisar el carrito** para comprobar los productos, las cantidades y el total, y continuar hasta el formulario para elegir el tipo de entrega, la fecha y la franja horaria.

## 5. Recorrido principal

1. **Inicio**: el usuario entiende qué es VitaMarket, ve productos destacados y accede al catálogo.
2. **Catálogo**: busca un producto o filtra por tipo de dieta y precio.
3. **Detalle**: consulta ingredientes, alérgenos, información nutricional y precio, y lo añade al carrito.
4. **Carrito**: revisa los productos, las cantidades y el total, y decide si sigue comprando o continúa.
5. **Acceso**: inicia sesión para continuar con el pedido (simulado).
6. **Formulario de entrega**: introduce sus datos de contacto, elige el tipo de entrega, la fecha y la franja horaria, y solicita la entrega.

## 6. Información necesaria

| Paso | Información necesaria |
|---|---|
| Inicio | Qué es VitaMarket, a quién va dirigido, productos destacados y acceso al catálogo |
| Catálogo | Nombre, imagen, precio y etiquetas de cada producto; buscador y filtros disponibles |
| Detalle | Ingredientes, alérgenos, información nutricional, cantidad y precio |
| Carrito | Productos seleccionados, cantidades, precio unitario, subtotales y total |
| Acceso | Qué datos introducir y aviso de que es una demostración |
| Formulario de entrega | Datos de contacto, tipo de entrega, dirección, fecha, franja horaria e instrucciones para los campos con formato |

> **Nota:** esta versión es un prototipo. El acceso, la gestión del carrito y el envío del formulario están representados pero no funcionan realmente. No se solicita ningún dato de pago.