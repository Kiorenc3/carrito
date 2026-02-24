🛒 Carrito Pro - Tienda Tech



Descripción

Carrito Pro es una aplicación web que simula el flujo básico de un carrito de compras de una tienda en línea. Permite al usuario agregar productos, modificar cantidades, eliminar artículos, ver el subtotal y persistir el carrito usando LocalStorage. El proyecto fue desarrollado completamente con tecnologías web nativas (HTML, CSS y JavaScript puro) y cuenta con pruebas unitarias automatizadas para la lógica del carrito usando Jest.

Tecnologías utilizadas

HTML5

CSS3

JavaScript (Vanilla)

Node.js

Jest (para pruebas unitarias)

Funcionalidades

Mostrar productos en tarjetas con imagen, nombre y precio.

Agregar productos al carrito.

Incrementar y disminuir la cantidad de productos en el carrito.

Eliminar productos cuando la cantidad llega a cero.

Cálculo automático del subtotal del carrito.

Persistencia del carrito utilizando LocalStorage.

Contador dinámico de productos en la interfaz.

Diseño visual mejorado con tarjetas, botones y animaciones.

Pruebas automatizadas con cobertura del 100% para la lógica del carrito.

Estructura del proyecto
carrito/
│
├── assets/                # Imágenes de productos
├── css/
│   └── styles.css         # Estilos principales
├── js/
│   ├── cart.js            # Lógica pura del carrito
│   └── app.js             # Conexión con DOM y LocalStorage
├── public/
│   └── index.html         # Página principal
├── __tests__/
│   └── cart.test.js       # Pruebas unitarias
├── package.json
└── README.md
Instalación y ejecución

Clonar el repositorio

git clone https://github.com/Kiorenc3/carrito.git

Ingresar al proyecto

cd carrito

Instalar dependencias

npm install

Correr pruebas unitarias

npm test

Ver cobertura de pruebas

npm run coverage
Ejecutar la aplicación

Abrir la carpeta public/

Ejecutar el archivo index.html con Live Server o similar

Interactuar con la tienda agregando o quitando productos

Detalles técnicos
Lógica del carrito

La lógica del carrito está separada en un módulo independiente (cart.js) para facilitar pruebas unitarias y asegurar que los cambios de estado no dependen directamente del DOM. Esto permite:

Testear la lógica con Jest sin necesidad de un navegador.

Mantener el código limpio, reutilizable y modular.

Pruebas automatizadas

Las pruebas se encuentran en __tests__/cart.test.js y cubren:

Agregar un producto nuevo.

Incrementar cantidad de producto existente.

Incrementar y mantener cantidades correctamente cuando hay múltiples productos.

Eliminar un producto.

Calcular subtotal con diferentes combinaciones.

Manejo de carrito vacío.

Validación de eliminación y re-renderizado.

La cobertura global es del 100% para líneas, funciones, declaraciones y ramas.

Mejoras realizadas

Integración con LocalStorage para persistencia.

Contador dinámico de productos en el DOM.

Diseño visual con tarjetas y animaciones.

Componentización lógica vs interfaz.

Botones para aumentar y disminuir cantidad.

Mejoras futuras recomendadas

Implementar un “checkout” simulado.

Integración con backend real y base de datos.

Gestión de stocks por producto.

Notificaciones (toast) cuando se agrega o elimina producto.
