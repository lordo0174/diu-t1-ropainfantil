# Documentación de la interfaz — Pequeños Pasos

## 1. Justificación del diseño

### 1.1 Importancia del diseño centrado en el usuario

Para diseñar Pequeños Pasos he intentado pensar principalmente en las personas que van a utilizar la aplicación. La idea es que comprar ropa infantil desde el móvil sea un proceso sencillo y que el usuario no tenga que dar muchas vueltas para encontrar lo que busca.

Por eso, desde la pantalla de inicio se puede acceder rápidamente a las categorías de Bebé, Niña y Niño. También se ha añadido un buscador y una sección de novedades para facilitar la búsqueda de productos.

El proceso de compra se ha organizado de una forma bastante directa:

**Inicio → Catálogo → Detalle → Carrito → Checkout → Confirmación**

De esta forma, el usuario puede ir avanzando paso a paso hasta terminar la compra.

También he intentado que los botones y elementos importantes sean fáciles de localizar y que las pantallas tengan una estructura parecida entre ellas para que la navegación resulte más intuitiva.

### 1.2 Objetivos del proyecto

Los principales objetivos que nos he marcado para la aplicación son:

- Conseguir que un usuario pueda encontrar una prenda en menos de 2 minutos.
- Permitir seleccionar una talla y añadir un producto al carrito de forma rápida.
- Conseguir que el proceso completo de compra pueda realizarse en menos de 3 minutos.
- Hacer que las diferentes secciones de la aplicación sean fáciles de encontrar.
- Mostrar claramente el precio final antes de confirmar un pedido.

### 1.3 Beneficios esperados

Con este diseño buscamos que el usuario pueda comprar ropa infantil sin complicaciones.

Para el usuario, la aplicación permite buscar productos, utilizar filtros, seleccionar una talla, revisar el carrito y completar una compra desde el móvil.

Para el negocio, una navegación sencilla puede ayudar a que los usuarios encuentren los productos que buscan y lleguen con mayor facilidad al proceso de compra.

---

# 2. Investigación y análisis de usuarios

## 2.1 Datos demográficos y segmentación

Pequeños Pasos está pensada principalmente para personas que compran ropa para niños y niñas de entre 0 y 14 años.

El público principal estaría formado por:

- Padres y madres.
- Familiares que compran ropa para niños.
- Personas que quieren comprar un regalo.
- Personas que prefieren realizar sus compras desde el móvil.

No todos los usuarios tienen el mismo nivel de experiencia utilizando aplicaciones de compra, por lo que he intentado mantener una interfaz sencilla y fácil de entender.

## 2.2 Personas

### Persona 1: Laura

**Edad:** 34 años

Laura es madre de dos hijos y compra ropa infantil varias veces al año. Normalmente utiliza el móvil para realizar este tipo de compras porque le resulta más cómodo.

**Lo que busca:**

- Encontrar ropa rápidamente.
- Filtrar los productos por edad y talla.
- Ver el precio de los productos.
- Poder realizar todo el proceso desde el móvil.

**Problemas que puede encontrar:**

- Tener demasiados productos entre los que elegir.
- No encontrar fácilmente una talla.
- Tener que pasar por demasiadas pantallas para comprar.
- No saber claramente cuánto va a pagar al final.

Por este motivo, en la aplicación he incluido categorías, filtros, un selector de talla y un resumen del pedido.

### Persona 2: Carlos

**Edad:** 52 años

Carlos compra ropa infantil de vez en cuando, principalmente cuando quiere hacer un regalo a sus nietos. No compra ropa infantil habitualmente, por lo que no siempre tiene claro qué talla debe elegir.

**Lo que busca:**

- Encontrar fácilmente un producto.
- Ver las tallas disponibles.
- Entender rápidamente cómo funciona la aplicación.
- Saber cuánto cuesta el pedido antes de comprar.

**Problemas que puede encontrar:**

- No saber qué talla elegir.
- No encontrar fácilmente el carrito.
- Encontrarse con demasiadas opciones.
- Tener dificultades con procesos de compra demasiado largos.

Por eso he intentado que las acciones principales estén visibles y que la navegación inferior se mantenga en las diferentes pantallas.

## 2.3 Análisis de la competencia

Para tener algunas referencias a la hora de diseñar la aplicación he tenido en cuenta aplicaciones conocidas de venta de ropa.

| Aplicación | Aspectos positivos | Aspectos que pueden resultar mejorables | Qué he tenido en cuenta |
|---|---|---|---|
| Zara | Buena organización de los productos y categorías | Puede haber muchas opciones | Organización visual de los productos |
| H&M | Tiene filtros y diferentes categorías | La cantidad de productos puede hacer que la búsqueda sea más larga | Uso de filtros |
| Kiabi | Está muy orientada a ropa familiar e infantil | Tiene muchos productos y categorías | Categorías y búsqueda sencilla |

A partir de esta comparación decidimos que Pequeños Pasos debía centrarse en una navegación sencilla y en facilitar la búsqueda de productos.

## 2.4 Insights y decisiones de diseño

### Insight 1

Los usuarios pueden querer comprar ropa para una edad concreta.

**Decisión:** en la pantalla de Inicio he colocado las categorías **Bebé, Niña y Niño** directamente en la pantalla principal.

### Insight 2

Cuando hay muchos productos, encontrar uno concreto puede ser más complicado.

**Decisión:** en el Catálogo he añadido filtros de **Talla, Color, Edad y Precio**.

### Insight 3

Elegir la talla puede ser una de las partes más importantes de la compra.

**Decisión:** en la pantalla de Detalle he colocado un selector de talla antes del botón de añadir al carrito.

### Insight 4

El usuario necesita saber cuánto va a pagar antes de terminar la compra.

**Decisión:** en el Carrito mostramos por separado el subtotal, el envío y el total.

### Insight 5

El usuario necesita saber si la compra se ha realizado correctamente.

**Decisión:** he creado una pantalla de Confirmación donde aparece el mensaje de pedido realizado, el número de pedido y el importe total.

---

# 3. Diseño de la interfaz

## 3.1 Mapa de navegación

El flujo principal de la aplicación es el siguiente:

```mermaid
flowchart TD
    A[Inicio] --> B[Catálogo]
    B --> C[Detalle de producto]
    C --> D[Carrito]
    D --> E[Checkout]
    E --> F[Confirmación]
    F --> A

    A --> G[Perfil]
    B --> G
    C --> G
    D --> G
    E --> G
    F --> G