# Arquitectura de Islas
La arquitectura de islas funciona renderizando la mayor parte de la página en HTML rápido y estático, añadiendo “islas” más pequeñas de JavaScript cuando se necesita interactividad o personalización en la página (un carrusel de imágenes, por ejemplo). Esto evita las cargas monolíticas de JavaScript que ralentizan la capacidad de respuesta de muchos otros marcos web modernos de JavaScript.

## ¿Qué es una isla?
En Astro, una isla es un componente de interfaz de usuario mejorado en una página HTML que, de otro modo, sería estática.

Una isla del cliente es un componente de interfaz de usuario interactivo JavaScript que se hidrata por separado del resto de la página, mientras que una isla del servidor es un componente de interfaz de usuario que renderiza en servidor su contenido dinámico por separado del resto de la página.

Ambas islas ejecutan procesos caros o lentos de forma independiente, por componente, para optimizar la carga de las páginas.

## Islas del cliente
Las islas del cliente son componentes de interfaz de usuario que se hidratan en el navegador. Esto significa que el componente se renderiza en el servidor y luego se envía al navegador como HTML estático. Una vez que el HTML estático llega al navegador, el JavaScript del componente se carga y ejecuta, lo que permite la interactividad.

