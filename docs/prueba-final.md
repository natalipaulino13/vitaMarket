# Prueba final de usabilidad

**Participante:** Mia (compañera de clase), la misma persona que revisó los bocetos.
**Fecha:** 08/11/2026
**Método:** Mia repitió las tres tareas de la revisión inicial sobre la web publicada en GitHub Pages, sin recibir instrucciones sobre dónde pulsar. Se le pidió que pensara en voz alta mientras las realizaba.

## Resultados

| Tarea | Resultado | Qué hizo | Dificultades observadas |
|---|---|---|---|
| 1. Encontrar un producto sin gluten y consultar sus características | **Autónoma** | Desde el inicio pulsó el atajo «Ver productos sin gluten». En el catálogo identificó los productos aptos por sus etiquetas y consultó su información | Esperaba que el atajo mostrara solo productos sin gluten, pero aparecían todos. Dijo: «Pensaba que aquí solamente aparecerían los productos sin gluten, pero veo que están todos. Voy a fijarme en las etiquetas» |
| 2. Localizar el carrito e identificar cómo continuar | **Autónoma** | Entró al carrito desde el menú, revisó productos, cantidades, precios y total, y localizó «Continuar con la entrega» | Ninguna. Al entrar en la web tardó unos segundos en familiarizarse con la página antes de decidir dónde pulsar |
| 3. Localizar el formulario y comprender qué información debe introducir | **Autónoma** | Pasó por el acceso con datos inventados y rellenó el formulario de entrega | Escribió un teléfono con menos cifras de las necesarias. El navegador mostró «Utiliza un formato que coincida con el solicitado» y lo corrigió, aunque el mensaje no decía qué formato se esperaba |

**Comprensión del formulario:** Mia entendió qué datos se pedían, cuáles eran obligatorios y que debía usar datos ficticios. Valoró el aviso de que no se realiza ningún pago.

**Funciones no implementadas:** al pulsar opciones sin funcionamiento real (filtros y otras herramientas del catálogo), leyó los avisos de prototipo y entendió que eran limitaciones de la demostración, no fallos de navegación.

## Comprobación de los cambios de la revisión inicial

| Cambio realizado tras la revisión de los bocetos | Resultado en la prueba final |
|---|---|
| Botón «Ver catálogo» más destacado | Lo encontró fácilmente |
| Atajos por tipo de dieta con texto descriptivo | Lo encontró y lo usó, aunque esperaba que filtrara los productos |
| «Añadir al carrito» junto al precio | Bien situado |
| Indicadores «Paso X de 3» | Le ayudaron a saber en qué parte del pedido estaba |
| Aviso de que no se realiza ningún pago | Identificó que era un prototipo |

## Valoración de las observaciones

| # | Observación | Tipo | Decisión |
|---|---|---|---|
| 1 | El atajo «Ver productos sin gluten» lleva al catálogo completo y Mia esperaba ver solo esos productos | **Función no implementada** (los filtros), que genera una expectativa de uso | **Se incorpora una mejora.** El filtro no puede funcionar sin programación, pero se añade debajo de los atajos un aviso que explica que llevan al catálogo completo y que hay que identificar los productos por sus etiquetas. Así la limitación se comunica antes de pulsar |
| 2 | El mensaje de error del teléfono es genérico y no indica el formato esperado | **Problema de uso** | **Se corrige.** Se añade el atributo `title` al teléfono y al código postal. El navegador lo incluye en el mensaje de error, que ahora indica el formato: «9 cifras sin espacios, por ejemplo 612345678» |
| 3 | Al entrar en la web tardó unos segundos en decidir dónde pulsar | Observación sin problema | **No se cambia.** Fueron solo unos segundos en una primera visita y encontró «Ver catálogo» sin ayuda. La página de inicio ya explica qué es VitaMarket y destaca la acción principal |

## Cambios realizados después de la prueba

- `index.html`: aviso debajo de «Compra según tu dieta» sobre el funcionamiento de los atajos en el prototipo.
- `formulario.html`: atributo `title` en los campos de teléfono y código postal.

## Conclusión

Mia completó las tres tareas de forma autónoma. Los cambios hechos tras la revisión de los bocetos funcionaron: encontró el catálogo, el carrito y el formulario sin ayuda y se orientó con los pasos del pedido. Las dos observaciones detectadas eran de detalle y se han corregido con cambios pequeños. La opinión de Mia: «Quizás haría que el acceso de productos sin gluten mostrase directamente esos productos, pero en general me ha resultado fácil utilizar la página».